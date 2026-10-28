# Airport Management Database — Schema Notes

This is a documentation-level schema reference based on the supplied Access database metadata and object strings. Confirm field definitions, data types, primary keys, and exact relationship settings inside Microsoft Access before treating it as a formal schema export.

## Core tables and fields identified

| Table | Fields identified | Purpose |
|---|---|---|
| Flights | FlightID, FlightNumber, AircraftID, GateID, Airline, Origin, Destination, DepartureTime, ArrivalTime, Status | Flight schedule and status |
| Passengers | PassengerID, FirstName, LastName, PassportNumber, Nationality, ContactNumber | Passenger details |
| Employees | EmployeeID, GateID, FirstName, LastName, Position, Department, HireDate, ContactNumber, Currency | Employee, role, and gate details |
| Aircrafts | AircraftID, AircraftType, Capacity, AirlineID, RegistrationNumber | Aircraft details and airline reference |
| Baggage | BaggageID, PassengerID, FlightID, Weight, Status | Baggage linked to passenger/flight |
| Gates | GateID, Terminal, GateNumber, Status | Gate and terminal details |
| Bookings | BookingID, PassengerID, FlightID, SeatNumber, BookingDate, Class, Price | Passenger flight bookings |
| Airlines | AirlineID, AirlineName, ContactInfo, Country | Airline details |

## Relationships indicated by database metadata

- Flights.AircraftID → Aircrafts.AircraftID
- Flights.GateID → Gates.GateID
- Aircrafts.AirlineID → Airlines.AirlineID
- Bookings.PassengerID → Passengers.PassengerID
- Bookings.FlightID → Flights.FlightID
- Baggage.PassengerID → Passengers.PassengerID
- Baggage.FlightID → Flights.FlightID
- Employees.GateID → Gates.GateID

The source also includes a field named Airline in Flights; its data type and intended role should be verified in Access rather than assumed to be a foreign key.

## Access objects

The available object metadata indicates forms, saved queries, and reports for several operational views. Confirm the exact object counts, names, and behavior from the Access Navigation Pane before including them in a formal technical specification.

## Privacy

The Passengers table includes a PassportNumber field, and passenger/employee records include contact fields. Do not publish the original records until the team has confirmed they are synthetic or replaced personal values with synthetic examples.

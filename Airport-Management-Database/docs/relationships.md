# Airport Management Database — Relationship Sketch

> This diagram is a documentation sketch based on database metadata. Confirm exact Access relationship settings before treating it as a verified ER diagram.

    erDiagram
        AIRLINES ||--o{ AIRCRAFTS : operates
        AIRCRAFTS ||--o{ FLIGHTS : assigned_to
        GATES ||--o{ FLIGHTS : schedules_at
        PASSENGERS ||--o{ BOOKINGS : makes
        FLIGHTS ||--o{ BOOKINGS : includes
        PASSENGERS ||--o{ BAGGAGE : owns
        FLIGHTS ||--o{ BAGGAGE : carries
        GATES ||--o{ EMPLOYEES : assigned_to

        AIRLINES {
            int AirlineID PK
            string AirlineName
            string ContactInfo
            string Country
        }
        AIRCRAFTS {
            int AircraftID PK
            string AircraftType
            int Capacity
            int AirlineID FK
            string RegistrationNumber
        }
        FLIGHTS {
            int FlightID PK
            string FlightNumber
            int AircraftID FK
            int GateID FK
            string Airline
            string Origin
            string Destination
            datetime DepartureTime
            datetime ArrivalTime
            string Status
        }
        GATES {
            int GateID PK
            string Terminal
            string GateNumber
            string Status
        }
        PASSENGERS {
            int PassengerID PK
            string FirstName
            string LastName
            string PassportNumber
            string Nationality
            string ContactNumber
        }
        BOOKINGS {
            int BookingID PK
            int PassengerID FK
            int FlightID FK
            string SeatNumber
            date BookingDate
            string Class
            decimal Price
        }
        BAGGAGE {
            int BaggageID PK
            int PassengerID FK
            int FlightID FK
            decimal Weight
            string Status
        }
        EMPLOYEES {
            int EmployeeID PK
            int GateID FK
            string FirstName
            string LastName
            string Position
            string Department
            date HireDate
            string ContactNumber
            decimal Currency
        }

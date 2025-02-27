
```python
class Caregiver:
    def __init__(self, name, specialization, contact):
        self.name = name
        self.specialization = specialization
        self.contact = contact

    def __str__(self):
        return f"Caregiver: {self.name} | Specialization: {self.specialization} | Contact: {self.contact}"


class HomecareService:
    def __init__(self, service_name, description, price):
        self.service_name = service_name
        self.description = description
        self.price = price

    def __str__(self):
        return f"Service: {self.service_name} | Description: {self.description} | Price: KES {self.price}"


class NairobiComfortCareService:
    def __init__(self):
        self.caregivers = []
        self.services = []
        self.bookings = []

    def add_caregiver(self, caregiver):
        self.caregivers.append(caregiver)
        print(f"Caregiver {caregiver.name} added successfully!")

    def add_service(self, service):
        self.services.append(service)
        print(f"Service {service.service_name} added successfully!")

    def book_service(self, service_name, caregiver_name, client_name, date):
        service = next((s for s in self.services if s.service_name == service_name), None)
        caregiver = next((c for c in self.caregivers if c.name == caregiver_name), None)

        if service and caregiver:
            booking = {
                "service": service,
                "caregiver": caregiver,
                "client_name": client_name,
                "date": date
            }
            self.bookings.append(booking)
            print(f"Service booked successfully for {client_name} on {date}!")
        else:
            print("Service or caregiver not found. Please check the details.")

    def display_caregivers(self):
        print("\n--- Available Caregivers ---")
        for caregiver in self.caregivers:
            print(caregiver)

    def display_services(self):
        print("\n--- Available Services ---")
        for service in self.services:
            print(service)

    def display_bookings(self):
        print("\n--- Bookings ---")
        for booking in self.bookings:
            print(f"Client: {booking['client_name']} | Service: {booking['service'].service_name} | Caregiver: {booking['caregiver'].name} | Date: {booking['date']}")


# Example Usage
if __name__ == "__main__":
    nairobi_care = NairobiComfortCareService()

    # Adding caregivers
    caregiver1 = Caregiver("John Doe", "Elderly Care", "0712345678")
    caregiver2 = Caregiver("Jane Smith", "Post-Surgery Care", "0723456789")
    nairobi_care.add_caregiver(caregiver1)
    nairobi_care.add_caregiver(caregiver2)

    # Adding services
    service1 = HomecareService("Elderly Care", "Comprehensive care for the elderly", 1500)
    service2 = HomecareService("Post-Surgery Care", "Specialized care for post-surgery patients", 2000)
    nairobi_care.add_service(service1)
    nairobi_care.add_service(service2)

    # Displaying caregivers and services
    nairobi_care.display_caregivers()
    nairobi_care.display_services()

    # Booking a service
    nairobi_care.book_service("Elderly Care", "John Doe", "Mary Johnson", "2025-03-01")

    # Displaying bookings
    nairobi_care.display_bookings()

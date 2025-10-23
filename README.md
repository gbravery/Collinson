**Architecture Overview:
**
I am showing this as a web application, under the assumption that it could be reactive, and therefore function as an app just as well on a mobile device.
Obviously, the screen needs to be tuned for the application use case - in a larger web page data could be better spread out, with more graphics and text.

**PCI Compliance
**
The solution has the potential to be PCI compliant, although that will depend on how payment needs to be taken when the "Confirm Booking" button is pressed.
If it is corporate level, with some sort of charge to account, that will be fine - simply use the existing chargeback process that exists.
If the card is stored on file somehow, PCI can be maintained and but is outside of scope of this application - we simply invoice that other system and it would perform the charge.
If taken in realtime, the web application would have to incorporate payment gateway functionality to make it compliant.
Backend systems would have to track the financial transactions being raised and reconcilled, but that is outside of the application.
However, presentation of any relevant  receipts would be useful here (especially for expense type situations).

**Omissions / Trade Offs
**
I've assumed the application has GPS tracking turned on (to show the estimated time to airport information).
It would also need internet access to obtain realtime flight information and to perform bookings.
I have also assumed a user is already logged in and has entered a flight - this data capture would need to be created.

I have desinged a very simple flight information screen - this could be significantly polished.
The focus is on the departure aspect of the application - similar functionality could be provided on the arrivals side.
I have also focused on showing and booking Taxis in the application. Theoretically, there could be similar processes for booking a Lounge.
These detail regions could be collapsable, to give more of the screen estate to other functionality that may be required.

I have somewhat glossed over how "Book Travel" screen could work - although it would use either an address picker with type ahead and/or determine the address from the GPS location selected.
The time entry should also apply constraints - e.g. if the travel time would result in something after the flight has closed, we shouldn't accept the booking.
There should be a calculation and presentation of the fare once the "From" location is selected.
Payment would also have to be taken - with appropriate screens designed to produce a secure transaction.

I have made assumptions about what level of integration I can make into the Taxi application, and the functionality it would provide.
One key assumption would be that we can track the vehicle and show its GPS location.
Other polish might be that click on the drivers details starts a phone call (for example).
There could also be a chat function with the driver.


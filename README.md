# booking-app

## Introduction
This is a React Native application developed for handling bookings. Built with Expo and React Native, it allows users to view, create, update, and delete bookings. The app showcases user bookings in a list and enables interactions such as sorting and filtering.

## Getting Started

### Prerequisites
- Node.js (v14 or later)
- Expo CLI
- Expo Go app for iOS or Android for testing on a physical device, or iOS Simulator/Android Emulator for testing on a virtual device.

### Setup
1. **Clone the repository:**
   ```bash
   git clone https://github.com/belulok/booking-app.git
   ```
   ```
   cd bookings-app
   ```

2. **Install dependencies:**
    ```
    npm install
    ```

3. **Start the Expo development server:**
    ```
    npm start
    ```

#### Optional - If using WSL2 like me
    ```
    npm start -- --tunnel
    ```

This will ask to install the @expo/ngrok package. Once that is done, you'll see the Metro is waiting message has a full URL instead of just an IP address. Scan the QR code and Expo Go will connect through the tunnel. This works because the tunnel is exposed to the internet, instead of just your local network.

WSL2, on the other hand, is a virtualized environment, using a virtual NIC behind a virtual Hyper-V switch. The WSL2 network is NAT'd behind/inside the Windows network, which is why you can't see it from other devices on the network.

WSL2 does provide a feature known as "local forwarding" that allows the Windows host itself to access WSL2 through the localhost address. However, that doesn't extend to other devices on the network.

**Running the App**
On a Physical Device: Open the Expo Go app and scan the QR code provided in the terminal.
On an Emulator/Simulator: With the Expo development server running, press i to open the iOS Simulator or a to open the Android Emulator.

**Features**
- User Bookings Page: Displays bookings associated with the hardcoded user, organized in a list.
- All Bookings Page: Shows all bookings in the system.
- User Profile Page: Presents details about the user.
- Create Booking Page: Allows users to create new bookings.
- Booking Detail Page: Offers detailed information about a specific booking.

**Optional Features**
- Sorting and Filtering: Users can sort bookings by price, check-in, or check-out date and filter by deposit paid.
- Updating and Deleting Bookings: Enables users to modify or remove their bookings.
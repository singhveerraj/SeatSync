# SeatSync — Smart Study Space Finder

A polished, frontend-first hackathon prototype for discovering and reserving study seats. The pilot is inspired by a campus library use case; all floor layouts, occupancy figures, bookings and user records are illustrative demo data, not verified TIET information.

## Run locally

```bash
cd frontend
npm install
npm run dev
```

Open the local URL printed by Vite. For a production bundle, run `npm run build`.

## Student experience
- Browse a clickable 48-seat illustrative layout with availability states.
- Switch between three configurable pilot-area views and filter by zone, seat type, power outlet, window seat and seat ID.
- Use Smart Pick to surface available individual seats with power outlets.
- Reserve for 1, 2 or 3 hours; a 10-minute demo hold expires automatically unless checked in.
- Open a reservation pass with a visual QR-style demo code and simulate a successful scan.
- Cancel a reservation or join a seat waitlist.

## Staff and admin experience
- Verify a reservation by code and confirm a student's check-in.
- Update seat availability and clear waitlist requests.
- View live-in-this-browser seat counts, zone occupancy, illustrative peak-hour trends and recent reservations.

## Prototype boundaries
- React + Vite frontend; data is stored in the browser's localStorage.
- The QR-style pass is a visual simulation, not a real encoded QR credential; no camera/scanner is connected.
- Student and staff views share state only in the same browser profile. There is no backend, real authentication, database, multi-device sync, hardware sensor feed, or verified campus floor plan.
- Waitlist promotion and automatic end-of-session enforcement are not implemented.
- Any charts and sample records are clearly illustrative and must not be presented as measured campus data.

# Project-Collab

We are creating an evenet management app and this is the first push from Roshan to check the Connection. 


                             ┌────────────┐
                             │  Start App │
                             └─────┬──────┘
                                   │
                         ┌────────▼─────────┐
                         │ Login or Sign Up │
                         └─────┬──────┬─────┘
                               │      │
                      ┌────────▼──┐ ┌─▼────────┐
                      │  Login    │ │ Sign Up  │
                      └────┬──────┘ └────┬─────┘
                           │             │
                    ┌──────▼──────┐      │
                    │ Validate    │      │
                    │ User (CSV)  │      │
                    └──────┬──────┘      │
                           │             │
                    ┌──────▼──────┐      │
                    │ User found? │◄─────┘
                    └─────┬───────┘
                    Yes   │   No
                         ▼
               ┌───────────────┐
               │ Load user role│
               └──────┬────────┘
                      │
          ┌───────────▼─────────────┐
          │ Is role == "admin"?     │
          └──────┬──────────┬───────┘
               Yes          No
               ▼            ▼
       ┌────────────┐ ┌───────────────┐
       │ Admin Panel│ │ User Panel    │
       └────┬───────┘ └─────┬─────────┘
            │               │
  ┌─────────▼──────┐ ┌──────▼────────────┐
  │ Create Event   │ │ View Events       │
  │ Edit Event     │ │ Book Event        │
  │ Delete Event   │ │ View My Bookings  │
  │ View Bookings  │ └──────┬────────────┘
  └──────┬─────────┘        │
         ▼                  ▼
   ┌────────────┐     ┌─────────────┐
   │ Logout/Exit│     │ Logout/Exit │
   └────────────┘     └─────────────┘

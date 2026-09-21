# print-by-sprint MVP execution plan

Generated on 2026-09-20
Project: 8.8 Events
Source plan: 8.8 Events Business Plan.md

## Purpose

This document turns the 8.8 Events MVP plan into a sprint-by-sprint execution backlog for developers, designers, and no-code builders.

The MVP should prove one thing first: customers can find verified event vendors, request quotes, book with confidence, and receive admin support when needed.

## MVP Build Principle

Build the platform as a controlled pilot, not the full national marketplace.

The first version should include:

- Public website.
- Customer account and dashboard.
- Vendor account and dashboard.
- Admin dashboard.
- Vendor verification.
- Vendor profiles and service listings.
- Event request and quote flow.
- Booking records.
- Payment-provider or payment-link workflow.
- Support and dispute tracking.
- Basic feedback after event completion.

The first version should not include:

- Mobile app.
- AI recommendations.
- Ticketing marketplace.
- Full event planning tools.
- Advanced subscriptions.
- Complex automated payouts.
- Nationwide launch automation.

## Confirmed Product Decisions

- Product model: hybrid marketplace with self-service plus admin support.
- Launch locations: Abuja/FCT, Kano, Lagos, plus one additional state to be selected.
- Vendor categories: MC, DJ, Catering and Food, Event Planning Services, Makeup and Styling, Printing and Branding, Fashion Designers for wedding gowns, suits, and event outfits.
- Payment direction: use licensed Nigerian payment providers such as Paystack or Flutterwave. Do not operate informal direct escrow in the MVP.
- Core surfaces: public website, customer dashboard, vendor dashboard, admin dashboard.

## Roles

Customer:

- Searches vendors.
- Submits event requests.
- Requests quotes.
- Books vendors.
- Pays through approved payment flow.
- Requests admin support.
- Opens disputes if needed.
- Leaves post-event feedback.

Vendor:

- Registers business.
- Applies for verification.
- Creates profile.
- Adds services and portfolio.
- Responds to quote requests.
- Manages bookings.
- Tracks payment and payout status.

Admin:

- Approves vendors.
- Reviews event requests.
- Monitors quotes and bookings.
- Supports customers and vendors.
- Handles disputes.
- Tracks payments and refunds.
- Manages categories, states, and platform settings.

## Sprint 0: Setup And Product Finalization

Duration: 1 week

Goal:

Prepare the team, tools, product rules, and technical foundation before feature development starts.

Tasks:

- Confirm the fourth launch state.
- Confirm whether Paystack or Flutterwave is the primary payment provider.
- Confirm initial refund, cancellation, dispute, and payout rules.
- Create product repository and project board.
- Choose build path: custom code, no-code, or hybrid.
- Finalize brand basics: logo direction, colors, typography, and tone.
- Create environment structure: development, staging, production.
- Define user roles and permissions.
- Define MVP database tables.
- Define API or no-code data collections.
- Create wireframe list for all MVP screens.

Deliverables:

- Final MVP scope.
- Product backlog.
- Technical stack decision.
- Database or no-code data model draft.
- Screen inventory.
- Payment provider decision.
- Launch-state decision.

Acceptance criteria:

- Team knows exactly what is in MVP and what is out.
- Product board has epics and tasks.
- Database model covers users, vendors, services, event requests, quotes, bookings, payments, support tickets, disputes, and reviews or feedback.
- Payment/refund rules are documented before payment integration starts.

## Sprint 1: Project Foundation And Authentication

Duration: 1 to 2 weeks

Goal:

Create the basic app foundation with authentication, roles, navigation, and shared layout.

Developer tasks:

- Set up frontend application.
- Set up backend or no-code backend.
- Set up database.
- Create authentication for customer, vendor, and admin users.
- Add login, register, forgot password, and logout.
- Create role-based routing.
- Create base layouts for public site, customer dashboard, vendor dashboard, and admin dashboard.
- Add basic profile settings.
- Add audit log structure for admin-sensitive actions.

Designer tasks:

- Create low-fidelity layouts for public site, dashboards, forms, and admin screens.
- Define reusable components: buttons, form fields, cards, status labels, tables, modals, and empty states.

No-code builder tasks:

- Create user tables or collections.
- Configure role permissions.
- Build login and registration flows.
- Create dashboard navigation shells.

Acceptance criteria:

- Customer can register and log in.
- Vendor can register and log in.
- Admin can log in.
- Each role lands on the correct dashboard.
- Users cannot access dashboards for other roles.
- App has base navigation and protected routes.

## Sprint 2: Vendor Profiles And Category Setup

Duration: 1 to 2 weeks

Goal:

Allow vendors to create profiles and services, while admins can manage categories and approve vendors.

Developer tasks:

- Create vendor profile form.
- Create service catalog form.
- Add media upload for portfolio images.
- Add launch locations: Abuja/FCT, Kano, Lagos, and placeholder for fourth state.
- Add vendor categories: MC, DJ, Catering and Food, Event Planning Services, Makeup and Styling, Printing and Branding, Fashion Designers.
- Add category-specific fields.
- Build vendor profile preview.
- Build admin vendor verification queue.
- Build approve, reject, suspend, and request-changes actions.

Designer tasks:

- Design vendor onboarding flow.
- Design vendor public profile.
- Design admin verification queue.
- Design status states for pending, approved, rejected, suspended, and changes requested.

No-code builder tasks:

- Create vendor profile database.
- Create service catalog database.
- Add file upload fields.
- Build admin approval workflow.

Acceptance criteria:

- Vendor can create and save business profile.
- Vendor can add at least one service.
- Vendor can upload portfolio images.
- Admin can approve or reject vendor.
- Only approved vendors appear publicly.
- Category and state filters exist in the data model.

## Sprint 3: Public Website And Vendor Discovery

Duration: 1 to 2 weeks

Goal:

Build the public discovery experience so customers can browse vendors and understand how 8.8 Events works.

Developer tasks:

- Build homepage.
- Build vendor search page.
- Build vendor profile page.
- Build category pages.
- Add filters for category and location.
- Add search by vendor name or service keyword.
- Add featured vendor placeholders.
- Add how-it-works content.
- Add public vendor registration call to action.
- Add basic SEO metadata for launch categories and locations.

Designer tasks:

- Design homepage.
- Design search results grid/list.
- Design vendor profile page.
- Design category landing page.
- Design empty states for no vendors found.

No-code builder tasks:

- Create public vendor directory.
- Connect filters to vendor data.
- Build category and location pages.

Acceptance criteria:

- Public users can browse approved vendors.
- Public users can filter vendors by category and location.
- Public users can open vendor profile pages.
- Unapproved vendors are not visible publicly.
- Vendor registration call to action is clear.

## Sprint 4: Customer Event Requests And Quote Flow

Duration: 1 to 2 weeks

Goal:

Allow customers to submit event needs and allow vendors or admins to respond with quotes.

Developer tasks:

- Build event request form.
- Add fields for event type, date, location, budget, services needed, notes, and support requested.
- Create customer event request dashboard.
- Create vendor incoming request view.
- Create quote response form.
- Create quote status flow: requested, sent, accepted, declined, expired.
- Add admin view of all event requests and quotes.
- Add notifications for new request and quote response.

Designer tasks:

- Design event request form.
- Design customer request dashboard.
- Design vendor quote response screen.
- Design admin request monitoring screen.

No-code builder tasks:

- Create event request collection.
- Create quote collection.
- Build automations for new request notifications.
- Build admin request list.

Acceptance criteria:

- Customer can submit event request.
- Vendor can view relevant request.
- Vendor can send quote.
- Customer can view quotes.
- Admin can view all requests and quotes.
- Customer can request admin assistance.

## Sprint 5: Booking Flow And Booking Management

Duration: 1 to 2 weeks

Goal:

Turn accepted quotes into booking records with visible status for customer, vendor, and admin.

Developer tasks:

- Create booking record from accepted quote.
- Add booking statuses.
- Build customer booking detail page.
- Build vendor booking detail page.
- Build admin booking management page.
- Add cancellation request action.
- Add completion confirmation action.
- Add booking notes.
- Add booking timeline.

Recommended booking statuses:

- draft_request.
- quote_requested.
- quote_sent.
- customer_reviewing.
- booking_pending_payment.
- payment_pending_verification.
- booked.
- vendor_confirmed.
- in_progress.
- completed_pending_customer_confirmation.
- completed.
- cancelled_by_customer.
- cancelled_by_vendor.
- disputed.
- refunded.
- expired.

Designer tasks:

- Design booking detail page.
- Design booking timeline.
- Design booking status labels.
- Design cancellation and completion confirmation prompts.

No-code builder tasks:

- Create booking collection.
- Add status workflow.
- Connect quote acceptance to booking creation.
- Build booking dashboards for each role.

Acceptance criteria:

- Accepted quote can create a booking.
- Customer, vendor, and admin can see booking status.
- Booking record includes customer, vendor, event date, amount, service, and terms.
- Admin can update booking status.
- Cancellation and completion actions are tracked.

## Sprint 6: Payment Provider Workflow

Duration: 1 to 2 weeks

Goal:

Add safe payment handling through an approved Nigerian payment provider or payment-link workflow.

Developer tasks:

- Integrate Paystack, Flutterwave, or payment-link flow.
- Add payment initialization.
- Add payment verification.
- Add payment webhook endpoint if using API integration.
- Store transaction reference.
- Tie payment to booking record.
- Add payment status to customer, vendor, and admin dashboards.
- Add admin reconciliation screen.
- Add refund tracking fields.

Recommended payment statuses:

- unpaid.
- payment_initialized.
- paid.
- partially_paid.
- payout_pending.
- payout_released.
- refund_pending.
- refunded.
- failed.

Designer tasks:

- Design checkout page.
- Design payment confirmation page.
- Design failed payment state.
- Design admin payment status table.

No-code builder tasks:

- Connect payment provider.
- Save transaction references.
- Create payment status automations.
- Add admin payment review dashboard.

Acceptance criteria:

- Customer can pay for a booking through payment provider or payment link.
- Payment reference is stored.
- Payment verification updates booking/payment status.
- Admin can see payment records.
- Vendor can see whether payment is pending, confirmed, or payout pending.
- Refunds are tracked even if processed manually in provider dashboard.

## Sprint 7: Support, Disputes, And Admin Intervention

Duration: 1 to 2 weeks

Goal:

Give customers, vendors, and admins a structured way to resolve problems.

Developer tasks:

- Build support ticket creation.
- Build dispute creation from booking page.
- Add dispute statuses.
- Add evidence upload or evidence notes.
- Add admin dispute review page.
- Add admin notes.
- Add resolution actions.
- Add urgent flag for payment-provider chargebacks.

Recommended dispute statuses:

- no_dispute.
- dispute_opened.
- evidence_requested.
- under_admin_review.
- resolved_customer_refund.
- resolved_vendor_payout.
- resolved_split.
- closed_no_action.

Designer tasks:

- Design support ticket form.
- Design dispute form.
- Design admin dispute review screen.
- Design evidence and resolution states.

No-code builder tasks:

- Create support ticket collection.
- Create dispute collection.
- Build admin notification workflow.
- Add evidence upload fields or notes.

Acceptance criteria:

- Customer can open support ticket.
- Customer or vendor can open dispute from booking.
- Admin can review dispute.
- Admin can add notes and update status.
- Dispute outcome is visible on booking record.

## Sprint 8: Reviews, Feedback, Notifications, And Metrics

Duration: 1 to 2 weeks

Goal:

Close the service loop with feedback, notifications, and basic marketplace metrics.

Developer tasks:

- Add post-event feedback or review form.
- Add vendor rating display if approved for public use.
- Add email notifications for key events.
- Add admin metrics dashboard.
- Track vendor response time.
- Track quote-to-booking conversion.
- Track completed bookings.
- Track disputes and refunds.

Designer tasks:

- Design review form.
- Design notification templates.
- Design admin metrics cards.

No-code builder tasks:

- Create feedback collection.
- Build notification automations.
- Build basic dashboard views.

Acceptance criteria:

- Customer can leave feedback after completion.
- Admin can see core metrics.
- Vendor response and booking completion can be measured.
- Notifications are sent for key events.

## Sprint 9: Pilot Launch Readiness

Duration: 1 week

Goal:

Prepare for a controlled launch with real vendors and customers.

Tasks:

- Test all customer flows.
- Test all vendor flows.
- Test all admin flows.
- Test payment flow with small live or test transactions.
- Test refund tracking process.
- Test dispute workflow.
- Load first verified vendors.
- Add final terms, privacy, refund, and cancellation content.
- Create launch checklist.
- Create support playbook.
- Create vendor onboarding guide.
- Create admin operating guide.

Acceptance criteria:

- At least 20 verified vendors are ready in each active launch location, or the team explicitly approves a smaller soft launch.
- Customer can discover, request quote, book, pay, and get support.
- Vendor can receive request, quote, confirm booking, and track status.
- Admin can monitor every critical step.
- Payment and support workflows have been tested.
- No P0 blocker remains open.

## Sprint 10: Controlled Pilot And Iteration

Duration: 2 to 4 weeks

Goal:

Run real customer requests through the platform and measure whether the marketplace works.

Tasks:

- Launch to a controlled customer group.
- Process first 20 to 50 event requests.
- Monitor vendor response times.
- Monitor booking conversion.
- Track support requests.
- Track disputes, cancellations, and refunds.
- Interview customers after completed bookings.
- Interview vendors after first quote or booking.
- Fix confusing flows.
- Remove unreliable vendors.
- Improve category and location supply.

Success metrics:

- 80 to 120 verified vendors across launch locations.
- 100 customer event requests.
- 25 completed bookings.
- Vendor response rate above 70%.
- Completed booking satisfaction above 80%.
- Dispute rate low enough for manual admin support to manage.

Acceptance criteria:

- Team knows which categories have real demand.
- Team knows which locations have enough vendor supply.
- Team knows where users drop off.
- Team has evidence to decide whether to expand, narrow, or rebuild parts of the flow.

## Backlog By Epic

### Epic 1: Authentication And Roles

- Customer registration.
- Vendor registration.
- Admin login.
- Password reset.
- Role-based access.
- Profile settings.

### Epic 2: Vendor Marketplace Supply

- Vendor profile.
- Service catalog.
- Portfolio uploads.
- Category-specific fields.
- Verification documents.
- Admin approval.
- Vendor suspension.

### Epic 3: Discovery

- Homepage.
- Vendor search.
- Category pages.
- Location filters.
- Vendor profile pages.
- Featured vendors.

### Epic 4: Event Requests And Quotes

- Event request form.
- Customer request dashboard.
- Vendor incoming requests.
- Quote response form.
- Quote status workflow.
- Admin quote monitoring.

### Epic 5: Bookings

- Booking creation.
- Booking detail page.
- Booking statuses.
- Booking timeline.
- Cancellation request.
- Completion confirmation.
- Admin booking oversight.

### Epic 6: Payments

- Payment initialization.
- Payment verification.
- Payment status tracking.
- Transaction references.
- Admin reconciliation.
- Refund tracking.
- Payout status tracking.

### Epic 7: Support And Disputes

- Support tickets.
- Dispute creation.
- Evidence upload or notes.
- Admin dispute review.
- Resolution tracking.
- Chargeback urgency flag.

### Epic 8: Reviews And Trust

- Post-event feedback.
- Vendor ratings.
- Verified badges.
- Vendor response metrics.
- Vendor reliability indicators.

### Epic 9: Admin Operations

- Admin overview.
- User management.
- Vendor management.
- Booking management.
- Payment management.
- Dispute management.
- Category and location settings.
- Audit logs.

### Epic 10: Launch Operations

- Vendor onboarding guide.
- Admin playbook.
- Customer support scripts.
- Terms and refund policy.
- Pilot metrics dashboard.
- Launch checklist.

## MVP Data Model Checklist

Required tables or collections:

- users.
- vendors.
- vendor_services.
- categories.
- event_requests.
- quotes.
- bookings.
- payments.
- messages or message_threads.
- support_tickets.
- disputes.
- reviews or feedback.
- vendor_documents.
- notifications.
- audit_logs.

## MVP API Checklist

Authentication:

- POST /api/auth/register.
- POST /api/auth/login.
- POST /api/auth/refresh.
- POST /api/auth/forgot-password.
- POST /api/auth/logout.

Vendors:

- GET /api/vendors.
- GET /api/vendors/:id.
- POST /api/vendors.
- PUT /api/vendors/:id.
- GET /api/vendors/:id/services.
- POST /api/vendors/:id/services.
- PUT /api/vendors/:id/services/:serviceId.
- GET /api/vendors/:id/reviews.
- POST /api/vendors/:id/documents.

Event requests and quotes:

- POST /api/event-requests.
- GET /api/event-requests.
- GET /api/event-requests/:id.
- POST /api/event-requests/:id/quotes.
- GET /api/event-requests/:id/quotes.
- PUT /api/quotes/:id/status.

Bookings:

- POST /api/bookings.
- GET /api/bookings.
- GET /api/bookings/:id.
- PUT /api/bookings/:id/status.
- POST /api/bookings/:id/cancel.
- POST /api/bookings/:id/complete.

Payments:

- POST /api/payments/initialize.
- POST /api/payments/verify.
- GET /api/payments/history.
- POST /api/payments/webhook/paystack.
- POST /api/payments/webhook/flutterwave.

Support and disputes:

- POST /api/support-tickets.
- GET /api/support-tickets.
- GET /api/support-tickets/:id.
- POST /api/disputes.
- GET /api/disputes.
- PUT /api/disputes/:id/status.

Admin:

- GET /api/admin/dashboard.
- GET /api/admin/users.
- GET /api/admin/vendors/pending.
- PUT /api/admin/vendors/:id/verification.
- GET /api/admin/bookings.
- GET /api/admin/payments.
- GET /api/admin/disputes.
- PUT /api/admin/disputes/:id/resolve.
- GET /api/admin/reports/revenue.
- GET /api/admin/audit-logs.

## Definition Of Done For MVP

The MVP is ready for controlled pilot when:

- Customers can browse verified vendors.
- Customers can submit event requests.
- Vendors can create profiles and respond to quote requests.
- Admins can approve vendors and monitor marketplace activity.
- Customers can accept a quote and create a booking.
- Payments are recorded through an approved payment-provider workflow.
- Support and dispute workflows exist.
- Admin can see bookings, payments, vendors, users, disputes, and core metrics.
- At least one full booking has been tested end to end.
- Terms, privacy, refund, cancellation, and dispute policies are visible before payment.

## Immediate Next Actions

1. Pick the fourth launch state.
2. Choose Paystack or Flutterwave as the primary payment provider.
3. Decide whether the first build will be custom code, no-code, or hybrid.
4. Create wireframes for the public site, customer dashboard, vendor dashboard, and admin dashboard.
5. Begin Sprint 0 setup.

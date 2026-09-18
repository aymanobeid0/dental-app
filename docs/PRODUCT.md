# Product definition

## Purpose

A dental clinic management web application for dentists, staff, and the clinic owner in Mauritania.

The product connects patient records, appointments, treatment plans, procedures, payments, expenses, and compensation. Its longer-term direction is a business intelligence platform for clinics.

## Users

- **Owner:** manages clinic finances, reports, compensation, and configuration. Can read patient clinical records but cannot edit them.
- **Doctor:** provides treatment, maintains clinical records, prescribes medicines, records payments, and views their own financial information.
- **Staff:** manages registration, appointments, payments, and treatment coordination with limited clinical access.

## Core workflows

### New patient

1. Staff registers the patient with name and phone number.
2. The consultation fee is collected and a doctor assigned.
3. An appointment is booked, including an available slot for a walk-in.
4. Staff or the assigned doctor marks the patient as arrived.
5. The doctor records findings and proposes treatment with prices and discounts.
6. The doctor records the patient's acceptance per procedure.
7. The patient receives a printed treatment plan and books subsequent visits.

### Continuing treatment

1. The patient attends an appointment.
2. The doctor starts or continues a procedure.
3. Clinical notes and actual visit times are recorded.
4. The procedure remains in progress, is completed, or is stopped.
5. Staff or the doctor records payment.
6. Excess payment becomes credit, pays another eligible procedure, or is refunded.

### Clinic management

The owner reviews collections, debts, expenses, doctor earnings, salaries, staff wages, and payouts.

## Product boundaries

- One clinic at launch.
- Future support for multiple clinics and organizations.
- Responsive web application suitable for computer, tablet, and phone browsers.
- Arabic, French, and English interface.
- French printed documents for the MVP.
- One owner-selected currency label for all amounts, without currency conversion.
- Read-only access to previously loaded information during internet outages.

## Guiding requirements

- Planned treatment does not create patient debt.
- Started treatment creates an obligation, reduced by allocated payments.
- Completed or stopped treatment can still have unpaid debt.
- Patients may have several treating doctors and simultaneous treatment plans.
- Clinical history is shared among authorized doctors; financial visibility remains doctor-specific.
- Historical financial and clinical changes must remain traceable where required by the business rules.

## Unresolved product constraints

Budget, launch date, expected scale, hosting, backup requirements, account setup, data retention, and advanced business intelligence metrics have not been agreed.

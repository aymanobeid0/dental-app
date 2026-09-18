# Business rules

## Patient registration and clinical access

- **PAT-01:** Name and phone number are mandatory; other patient information is optional.
- **PAT-02:** Duplicate phone numbers are allowed with a warning and family-member note.
- **ACC-01:** Booking or assignment alone does not open initial clinical access. Staff or the assigned doctor must mark arrival.
- **ACC-02:** After consultation, a doctor retains access to the patient's clinical history. Planned or completed procedures also establish continuing access.
- **ACC-03:** Authorized doctors can read shared clinical history but see only their own financial activity.
- **ACC-04:** Doctors edit only their own clinical entries, except shared medical information.
- **ACC-05:** Any authorized treating doctor can update allergies and conditions, with author and time recorded.
- **ACC-06:** Staff can see treatment plans and procedures for coordination, but not medical conditions or clinical notes.
- **ACC-07:** Owner clinical access is read-only.
- **ACC-08:** Staff can preview an X-ray once during upload; afterward they see filename and confirmation only.

## Treatment

- **TRT-01:** A patient may have multiple simultaneous plans from different doctors.
- **TRT-02:** Doctors may use catalog procedures or custom entries.
- **TRT-03:** A procedure can cover one tooth, several teeth, or the whole mouth with one total price.
- **TRT-04:** Acceptance is recorded per procedure without requiring payment. Accepted procedures become planned.
- **TRT-05:** Planned procedures create no debt.
- **TRT-06:** Starting a procedure makes its price owed regardless of the plan's status. Existing allocated payments reduce the unpaid amount.
- **TRT-07:** A doctor may start a standalone procedure outside a plan.
- **TRT-08:** One doctor handles each procedure in the MVP; a procedure can span multiple visits.
- **TRT-09:** Completion leaves any unpaid amount as debt.
- **TRT-10:** Stopping treatment preserves only the unpaid remainder. The same procedure can later resume.
- **TRT-11:** Notes lock after the visit; subsequent corrections are dated amendments.
- **TRT-12:** Attachments may belong to the general file or be linked to procedures and visits.
- **TRT-13:** Prescriptions use the shared medicine list or free text. Newly entered drugs may optionally be saved.
- **TRT-14:** Prescriptions use clinic branding and a footer with doctor name and phone.

## Scheduling

- **APT-01:** Scheduling reserves doctor time, not rooms or chairs.
- **APT-02:** Each doctor has individual hours, breaks, and time off.
- **APT-03:** Owner manages all doctor schedules; doctors manage their own.
- **APT-04:** Staff or doctor chooses and can adjust appointment duration, subject to the no-overlap rule.
- **APT-05:** Reserved periods are grayed out and unavailable, with a warning.
- **APT-06:** Actual visit times are separate from booked times. An overrun does not automatically change reservations.
- **APT-07:** Actual timing supports start/finish buttons and manual corrections.
- **APT-08:** Walk-ins require an available booking slot.
- **APT-09:** Availability changes preserve existing bookings and flag affected appointments.
- **APT-10:** WhatsApp reminders are manually reviewed and sent in the MVP.

## Payments and pricing

- **FIN-01:** Doctors and owner can adjust prices and discounts. Changes after treatment starts or payments exist require a reason and preserved history.
- **FIN-02:** Installments are flexible, without scheduled amounts or due dates.
- **FIN-03:** Payments default to the current procedure; staff may change allocation.
- **FIN-04:** Staff and doctors can record cash and manually verified mobile money payments.
- **FIN-05:** Owner manages the mobile money app list.
- **FIN-06:** Excess payments can become credit, go to another eligible procedure, or be refunded.
- **FIN-07:** Credit stays with the original doctor and cannot fund another doctor's procedure.
- **FIN-08:** Owner, doctor, and staff can issue refunds with recorded reason and history.
- **FIN-09:** Staff and owner require approval from the doctor linked to the payment for corrections or voids.
- **FIN-10:** Doctors can correct their own payment entries with a reason. Original information remains in history.
- **FIN-11:** A receipt is issued after each payment. Procedure receipts show amount, procedure, method, and remaining balance.
- **FIN-12:** Optional invoices include only fully paid, completed procedures.
- **FIN-13:** Owner chooses a common consultation fee or doctor-specific fees.
- **FIN-14:** Staff applies or waives returning consultation fees after speaking with the doctor; no system approval is required for that decision.
- **FIN-15:** One currency label applies throughout; no currency conversion.

## Compensation

- **CMP-01:** Doctor compensation can be salary, percentage, or both.
- **CMP-02:** Salaries and staff wages are fixed monthly amounts.
- **CMP-03:** Percentage earnings are based on payments received, including consultation payments.
- **CMP-04:** Owner selects gross or after-cost basis per doctor.
- **CMP-05:** Eligible costs are deducted before calculating the percentage.
- **CMP-06:** Owner chooses a common doctor rate or rates by procedure type.
- **CMP-07:** Owner, treating doctor, and staff can record lab and material costs.
- **CMP-08:** Costs exceeding receipts carry forward against later receipts for the same procedure.
- **CMP-09:** Earnings, payouts, and unpaid compensation are tracked separately.
- **CMP-10:** Doctors see their own earnings, deductions, payouts, and remaining amounts owed.
- **CMP-11:** Refunds reverse related earnings. Already-paid earnings are adjusted against future payouts.
- **CMP-12:** Money held as credit earns compensation immediately at the original procedure's rate.
- **CMP-13:** Later credit use creates no second earnings and does not change the original rate.
- **CMP-14:** Opening debt has a doctor, a historical percentage rate, and remaining unpaid doctor compensation, but no procedure.
- **CMP-15:** Payments against opening debt earn the historical percentage only until remaining doctor compensation is settled. Previously settled compensation earns nothing further.

## Examples

- Started procedure: 2,000. Planned procedure: 3,000. Payment toward started procedure: 500. **Patient debt: 1,500.**
- Receipt: 1,000. Deductible cost: 200. Rate: 40%. **Doctor earnings: 320.**
- Completed procedure with 400 unpaid: **400 remains debt.**

## Unresolved rules

- Who enters and corrects opening debts.
- Financial treatment of advances and receiving-procedure costs when credit already earned compensation.
- Late cost entry, partial refunds, rounding, and compensation-rate changes.
- Consultation-origin credit rates.
- Approval when the linked doctor is unavailable.
- Payroll periods, proration, and payout-entry permissions.
- Exact report formulas and document numbering.
- Plan-level statuses and declined/undecided procedure representation.
- Exact single-preview enforcement and offline cache policy.

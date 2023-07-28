Bug Report:-

On the job details form when the user submits the form it doesn’t go to the next step even when there are no errors on the screen.

I have fixed this error, this was happening because of the extra "jobPosition: Yup.string().required("Job position is required")" validationSchema we are using from formik.
I have commented out this line 31, file name JobDetailsForm.tsx.
// jobPosition: Yup.string().required("Job position is required"),

I have also added Validation on  the interview settings form.

//

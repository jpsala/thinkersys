<div className="message-container">

              {formSubmitted && !isFormValid() &&

                enqueueSnackbar('Missing required fields. Please validate before submitting again.',

                  { variant: 'warning' })

              }

              {formSubmitted && error && (

                <Snackbar open={snackbar.open} onClose={handleClose}>

                  <Alert variant="filled" severity="error">

                    There was an error processing the account request.

                  </Alert>

                </Snackbar>

              )}

              {!isFormValid() && error && (

                <Snackbar open={snackbar.open} onClose={handleClose}>

                  <Alert variant="filled" severity="error">

                    Please fill in missing required fields.

                  </Alert>

                </Snackbar>

              )}

              {formSubmitted && success && (

                <Snackbar open={snackbar.open} onClose={handleClose}>

                  <Alert variant="filled" severity="success">

                    Account Request saved succesfully.

                  </Alert>

                </Snackbar>

              )}

            </div>
# QR Codes and TOTP Authentication Demo

Collects several notebook examples for QR-code creation and time-based one-time-password authentication. The final example hashes passwords with bcrypt and combines password verification with Google Authenticator.

## Workflow

1. Generate QR codes from text or URLs.
2. Create a TOTP secret and provisioning URI.
3. Verify a six-digit Authenticator code.
4. Register an in-memory demo user with a bcrypt password hash.
5. Require both the password and current OTP at login.

## Data Requirements

- No external dataset is required.

Datasets and generated artifacts are not included unless they are embedded directly in the notebook.

## Requirements

- qrcode
- Pillow
- pyotp
- bcrypt
- IPython

Install missing packages in your Jupyter or Google Colab environment before running the notebook.

## Running the Notebook

1. Open [`QRCodeAndOTP.ipynb`](QRCodeAndOTP.ipynb) in Jupyter Notebook or Google Colab.
2. Place any required data files in the path expected by the notebook.
3. Update local or Google Drive paths where needed.
4. Run the cells from top to bottom.

## Outputs

- Displayed QR codes
- TOTP verification messages
- In-memory demo authentication result

## Security and Responsible Use

This is a teaching demonstration, not a production identity system. Public-copy outputs and personal sample contact values were sanitized; generated secrets must still be treated as credentials.

## Repository Contents

```text
.
|-- README.md
`-- QRCodeAndOTP.ipynb
```

## Notes

- This repository preserves the analysis as a notebook-first educational project.
- Results may vary with dataset versions, random splits, package versions, and available hardware.
- Review file paths and runtime-specific commands before executing outside Google Colab.

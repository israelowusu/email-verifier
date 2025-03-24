# Email Domain Verifier

A command-line tool written in Go that verifies email domain configurations by checking MX, SPF, and DMARC records.

## Features

- Checks for MX (Mail Exchange) records
- Verifies SPF (Sender Policy Framework) records
- Validates DMARC (Domain-based Message Authentication, Reporting, and Conformance) configuration
- Outputs results in CSV format

## Usage

1. Build the project:
```sh
go build
```

2. Run the program:
```sh
./email-verifier
```

3. Enter domain names (one per line) and press Enter. For example:
```
gmail.com
yahoo.com
```

The program will output results in CSV format with the following columns:
- domain: The domain name being checked
- hasMX: Whether the domain has MX records
- hasSPF: Whether the domain has SPF records
- spfRecord: The actual SPF record if found
- hasDMARC: Whether the domain has DMARC records
- dmarcRecord: The actual DMARC record if found

## Requirements

- Go 1.24.1 or higher

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author

israelowusu
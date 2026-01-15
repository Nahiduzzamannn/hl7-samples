# Commure Take-Home Assessment – HL7 SIU Message Parser

# Candidate Information

  Name: Md. Nahiduzzaman  
  Contact: 01521799011  
  Email: Nahiduzzaman1106@gmail.com  



# Problem Overview
The objective of this assessment is to design and implement a "robust HL7 SIU (Scheduling Information Unsolicited) message parser".

The parser should:
  Validate that the message is an SIU type
  Extract appointment, patient, and provider information
  Handle missing or optional segments gracefully
  Raise meaningful errors for invalid or incomplete messages
  Be testable, readable, and production-ready



# Solution Summary
I implemented a clean, modular Python-based HL7 SIU parser that processes HL7 messages as a list of segments.

# Key Features
  Validates message type using the `MSH` segment
  Extracts appointment details from the `SCH` segment
  Extracts patient information from the `PID` segment
  Optionally extracts provider information from the `PV1` segment
  Raises custom exceptions for:
  Unsupported message types
  Missing required segments
  Includes unit tests using `pytest`
  Dockerized for consistent execution



## Project Structure

# Resource Management Platform (RMP)

The Resource Management Platform (RMP) is a robust, modular, and extensible system designed to manage resources efficiently across various domains. Initially developed as a general-purpose resource management solution, RMP provides a foundational framework for building domain-specific applications, including healthcare, education, logistics, and more.

## Vision

RMP aims to be the foundational platform for efficient resource management, capable of scaling from small businesses to large enterprises. While its core is domain-agnostic, it includes the flexibility to create specialized add-ons tailored for specific industries. The first planned add-on will focus on healthcare, creating a Health Resource Management Platform (HRMP).

## Features

- **Modular Architecture**: Easily extend functionality with custom modules.
- **Scalability**: Built to handle growing user bases and data loads.
- **Interoperability**: Designed with interoperability standards to integrate seamlessly with existing systems.
- **Real-Time Communication**: Ensures efficient and up-to-date interactions.
- **Privacy and Security**: Implements best practices for compliance with global data protection regulations.
- **Domain-Specific Add-Ons**: Health-focused features leveraging FHIR resources and anonymized test data from Synthea.

## Technologies

- **Backend**: .NET + Aspire
- **Frontend**: Blazor for real-time, dynamic interfaces
- **Workflow**: Elsa 3 for customizable workflows
- **Messaging**: MassTransit for inter-service communication
- **Data Standards**: FHIR (healthcare add-on)
- **Cloud Platform**: Microsoft Azure
- **Test Data Generation**: Synthea for healthcare scenarios

## Repository Structure

```plaintext
- src/
  - Core/                # Core platform services
  - Modules/             # Add-on modules (e.g., healthcare)
  - Frontend/            # Blazor frontend
  - Integration/         # Integration and API services
- tests/
  - UnitTests/           # Core platform unit tests
  - ModuleTests/         # Add-on module-specific tests
- docs/
  - Architecture.md      # System architecture details
  - HealthcareAddOn.md   # Specifics of the healthcare module
- tools/
  - Scripts/             # Helper scripts for deployment and maintenance
```

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch for your feature or fix.
3. Submit a pull request with a clear description of the changes.

### Code Style

Please adhere to the project’s code style guidelines, which can be found in `docs/CodeStyle.md`.

## Roadmap

1. Finalize the core platform.
2. Develop the first healthcare-specific add-on (HRMP).
3. Expand to other domains with modular add-ons.

## License

This project is licensed under the Apache License 2.0. See `LICENSE` for details.


# Data Acquisition Package
Provides safe and secure storage of medical data; serves as an interface for other packages to access this data using the FHIR standard; and offers data governance that complies with data protection laws. Facilitates data compilation for many modalities; registers data and metadata; offers a federated data catalogue and data governance; ingests data; and manages patient consent information. 

## Metadata

The **Data Acquisition Package** leverages a metadata-driven approach to ensure the efficient and compliant handling of medical data. Metadata plays a pivotal role in organizing, cataloging, and governing data while maintaining interoperability across diverse systems. 

### Integration with the Croissant Metadata Standard

The **Croissant metadata format** serves as the foundation for the Data Acquisition Package's metadata structure. Its flexibility and extensibility make it an ideal choice for describing complex medical data. By adopting Croissant, the package ensures:

- **Interoperability**: Seamless integration with other systems and packages that utilize the Croissant format. 
- **Clarity**: A standardized, human-readable representation of metadata for medical datasets.
- **Scalability**: The ability to manage metadata for large-scale, multi-modality datasets in distributed environments.

### Extending Croissant for Health Data

To accommodate the unique requirements of health data, the Croissant format can be extended with custom attributes and domain-specific schemas. Examples include:

1. **Health Topics Metadata**: Introducing new attributes to classify data by health topics such as cardiology, oncology, pediatrics, and more. This allows for precise organization and retrieval of domain-specific datasets.
   - **Example fields**: `health_topic`, `clinical_specialty`, `ICD_code`.

2. **Patient Consent Metadata**: Adding attributes to manage and track patient consent related to data usage, ensuring compliance with laws like GDPR and HIPAA.
   - **Example fields**: `consent_id`, `consent_scope`, `consent_expiration_date`.

3. **Federated Data Cataloging**: Enhancing metadata to describe relationships between datasets in a federated system, supporting data discovery and access control.
   - **Example fields**: `dataset_origin`, `access_control_policy`, `federation_id`.

4. **FHIR Standard Integration**: Embedding FHIR-specific metadata for compatibility with the Fast Healthcare Interoperability Resources (FHIR) framework.
   - **Example fields**: `fhir_resource_type`, `fhir_version`, `patient_reference`.

By building upon the Croissant metadata standard, the Data Acquisition Package creates a robust framework for managing medical data across various modalities and health domains. This ensures scalability, regulatory compliance, and ease of data exchange in healthcare ecosystems.

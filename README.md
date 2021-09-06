
# 1. Introduction

The eDelivery building block is constantly evaluated by organisations across the EU as an option for projects that require secure and reliable communication.

An observation from the feedback collected is that, while the eDelivery AS4 profile is a good fit for many of the above-mentioned projects, several others, with a growing diversity of requirements, would welcome the extension of the eDelivery building block with a profile to cater for the REST API architectural style. What is common to these potential projects is that at least one party to the data exchange would operate in a light context, loosely defined as a set of constraints and circumstances applying to organisations or individuals looking to consume a business service with a relatively small technical footprint. Such constraints could be linked to non-availability of any combination of human, financial, knowledge, technical or power resources, whether at design, installation or run-time.

A profile for a harmonised use of the REST API architectural style is thus proposed here to respond to this need, as part of the 2020 ISA2 Innovative Public Services (IPS) action. If successful, the profile could, as a next step, be added to the eDelivery building block.

# 2. Scope and Goals

The aim of this specification is to create a profile of several HTTP and REST specifications catering for the “light context”. The profile is built on top of the HTTP/REST architectural pattern and will adopt technology to support this pattern based on existing standards, including standardised specifications, IETF Draft RFCs, RFCs etc. Its scope is to provide:

 - Standardised data exchange
 - Business-agnostic data exchange
 - Secure data exchange

Focusing on the light context, the profile would enable the implementation of eDelivery-compliant data exchange benefiting from:

 - Ease of deployment/installation
 - Economy of resources on the client side
 - Operation on mobile/personal environments
 - Updated options for the data exchange patterns

The specification profiles also aspects of an HTTP / REST API ecosystem that are not part of the implementation itself, such as:

 - Delegated Authentication Patterns
 - Delegated Authorization Patterns
 - Lifecycle management
 - API Discoverability

# 3. Notation

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "NOT RECOMMENDED", "MAY", and "OPTIONAL" in this document are to be interpreted as described in [BCP14] ([RFC2119] and [RFC8174]) when, and only when, they appear in all capitals, as shown here.

# 4. Document Structure

The document consists of three main sections and two profile enhancements. The main sections of the profile are the API Core Profile, the API Documentation and Messaging API Specification. The two profile enhancements are the High-Security Enhancement and the Discoverability Enhancement.


# 4.1. Profile Sections

The ISA² IPS REST API profile consists of three hierarchical sections, each subsequent section depending on the preceding one. The API Core Profile (Level 1) is considered the baseline and mandatory part of the REST API Profile from a conformance perspective. The API Documentation goes one step further and defines how an OpenAPI Document should be structured for an API in order to be conformant (Level 2). An API conformant to Level 2 is an API that inherently conforms to Level 1 and also provides an OpenAPI Document according to the specification of Level 2. The final section provides a REST Messaging API Specification, itself conformant to Levels 1 and 2 of the profile, to be reused as a messaging specification in a light context, architecturally comparable to, but feature-different from the eDelivery AS4 profile.

# 4.1.1. Level 1: API Core Profile

The API Core Profile provides the baseline of the HTTP technologies that are profiled as part of the ISA² IPS REST API profile, covering the following major aspects of a REST API:

 - Authentication
 - Authorization
 - Transport, message and payload level security
 - Lifecycle management
 - Common semantics on REST API design, resource representations, HTTP methods and error representations
 - Documentation and discoverability

In the API Core Profile, several RFCs and Internet-Drafts from the IETF together with standards provided from organisations like W3C, ISA and ETSI are being selected and profiled to meet the requirements.

# 4.1.2. Level 2: API Documentation

Level 2 of the profile provides an extra layer of conformance, applicable for the documentation of the API. It profiles the OpenAPI Specification v3 and provides both predefined components that can be reused and extensions to the OpenAPI Specification for aspects not currently supported such as the lifecycle definition of an API.

# 4.1.3. Messaging API

The Messaging API Specification is an API specification that is based on both the API Core Profile and the API Documentation specifications and that makes use of the High-Security Enhancement of the profile. Its aim is to provide a common REST API Specification for messaging aligned with the scope and goals stated in the above section.

# 4.2. Profile Enhancements

Requirements expected to be common in many, but not all environments, are captured separately as Profile Enhancements. This avoids the need for all conformant implementations to be aligned to a highest common denominator, while still providing a standardised approach where necessary by allowing projects or organisations to mandate the use of the core profile sections in combination with a specific selection of enhancements.

The Profile Enhancements MUST be used in conjunction with the REST API Profile. The two currently defined Profile Enhancements are mutually compatible, so they MAY be used in combination.

# 4.2.1. High-Security Enhancement

The API Core Profile defines guidelines on how Message Level and Payload Security MUST be implemented, if needed. The High-Security Enhancement makes their implementation mandatory, further restricting the algorithms that can be used.
# 4.2.2. Discoverability Enhancement

The API Core Profile defines a minimal set of guidelines on how APIs should support discoverability. The Discoverability Enhancement extends this set to mandate further discoverability guidelines. Thus, an API conforming to the Discoverability Enhancement MUST implement both the guidelines defined in the Discoverability section of the API Core Profile, by providing all the OpenAPI attributes prescribed therein, and the additional ones defined in the Discoverability Enhancement.

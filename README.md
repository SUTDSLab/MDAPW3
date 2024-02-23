# MDAPW3: MDA-Based Development of Blockchain-Enabled Decentralized Applications 
## Table of Contents
1. [Project Specification](#project-specification)
2. [Case Study and Examples](#case-study-and-examples)
3. [Project Structrue](#project-Structrue)
4. [Development Environment Setup](#development-environment-setup)
    1. [Setting Up Eclipse IDE](#setting-up-eclipse-ide)
    2. [Installing Dependencies](#installing-dependencies)
5. [Setting Up The Project](#setting-up-the-project) 
6. [How to Cite This Project](#how-to-cite-this-project)

## Project Specification 
This repository hosts full implementation of MDAPW3 approach. MDAPW3 is a Model Drivent Development (MDD) approach based on OMG Model Driven Architecture (MDA) standard, which we are proposed in our latest research for developing Web3.0 DApps. As states in our research paper, we used Eclipse Epsilon framework to implement MDAPW3 which are include model-to-model transformations algorithms, mode-to-text (code generation) algorithms and also models verfication and validations scripts. you may intersted to read our research paper in the following link:
- [TODO: link to our paper will be added here](./#)
## Case Study and Examples
You could find the Land leasing case study in [https://github.com/SUTDSLab/MDAPW3/CaseStudy](https://github.com/SUTDSLab/MDAPW3-CaseStudy)
## Project Structrue
- META-INF: icludes the project definitions and depedencies of the project. Eclipse IDE use this directory content configuration files to properly load the project dependencies.
- src/mdapw3: This directory includes the implementation of all the MDAPW3 meta-models transformations, code-generation and verification/valdiation codes.
    - metamodels: includes all of the MDAPW3 metamodels
        - cim: this directory includes the following files
            - mdapw3cim.ecore : computational independent meta-model in EMF (.ecore) compatiable format.
            - mdapw3cim.emf : computational independent meta-model, implemented in EMF format. from this code, .ecore meta-model could be generated and vice versa.
            - mdapw3cim.emf.picto : this file includes codes which is used to generated visualized diagram of the mdapw3cim meta-model which could be rendered by picto tool.
        - pim: this directory includes the following files
            - mdapw3pim.ecore : platform independent meta-model in EMF (.ecore) compatiable format.
            - mdapw3pim.emf : platform independent meta-model, implemented in EMF format. from this code, .ecore meta-model could be generated and vice versa.
            - mdapw3pim.emf.picto : this file includes codes which is used to generated visualized diagram of the mdapw3pim meta-model which could be rendered by picto tool.
        - psm: this directory includes the following files
            - mdapw3psm.ecore : platform specific meta-model in EMF (.ecore) compatiable format.
            - mdapw3psm.emf : platform specific meta-model, implemented in EMF format. from this model .ecore meta-model could be generated and vice versa.
            - mdapw3psm.emf.picto : this file includes codes which is used to generated visualized diagram of the mdapw3psm meta-model which could be rendered by picto tool.
    - transformations: includes implementations of the model-to-model transformations algorithms
        - bpmn2chor_to_mdapw3cim.etl : impelemtaion of the BPMN2.0 Choregraphy model to MDAPW3 CIM transformation alogrithm using Epsilon Transformation Language (ETL)
        - mdapw3cim_to_mdapw3pim.etl : impelemtaion of the MDAPW3 CIM model to MDAPW3 PIM transformation alogrithm using ETL
        - mdapw3pim_to_mdapw3psm.etl : impelemtaion of the MDAPW3 PIM model to MDAPW3 PSM transformation alogrithm using ETL
        - mdapw3psm_to_mdapw3code.etl : impelemtaion of the MDAPW3 PSM model to Web3.0 DApp Code-base transformation alogrithm using ETL. this transformation algorithm use code generation algorithms which are written in .egl
    - codegenerations: includes implementations of the model-to-text (code generations) algorithms
        - mdapw3contract.egl : implementaion of smart contract code generation algorithm using Epsilon Generation Language (EGL). generated codes are in solidity language.
        - mdapw3dappui.egl : implementaion of DApp UI code generation algorithm using EGL. the generated codes are in JavaScript language.
        - mdapw3webserver.egl : implementaion of web server adapters code generation algorithm using EGL. the generated codes are in JavaScript language.
        - mdapw3oracleserver.egl : implementaion of oracle server adapters code generation algorithm using EGL. the generated codes are in JavaScript language.
        - mdapw3dbms.egl : implementaion of DBMS adapters code generation algorithm using EGL. the generated codes are in JavaScript language.
        - mdapw3p2pdms.egl : implementaion of P2PDBMS like IPFS adapters code generation algorithm using EGL. the generated codes are in JavaScript language.
        - mdapw3config.egl : implementaion of build and deployment code generation algorithm using EGL. the generated codes are in JSON and YMAL languages.
    - verfication_validation: includes implementations of model verfications and validations algorithms. these algorithms implemented using Epsilon Validation Language (EVL) and Epsilon Comparison Language (ECL).


## Development Environment Setup

### Setting Up Eclipse IDE
TODO: IDE setup instructions will be added here
### Installing Dependencies
TODO: Dependencies installation instructions will be added here
## Setting Up The Project
TODO: Project setup instructions will be added here
## How to Cite This Project
TODO: paper citation record will be added here
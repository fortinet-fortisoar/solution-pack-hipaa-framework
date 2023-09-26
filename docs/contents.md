| [Home](../README.md) |
 | -------------------------------------------- |

  # Contents

The **HIPAA Framework** solution pack contains the following resources.


## Picklists

| Name                           |
|:-------------------------------|
| ClinicalPHIType                |
| Contact Title                  |
| DemographicPHIType             |
| FinancialPHIType               |
| GDPRDataBreachType             |
| GDPREUCountryList              |
| GDPRReminderStatus             |
| PHIBreachLocation              |
| PHIBreachResponseActions       |
| PHISafeguardType               |
| ProtectedHealthInformationType |
| RegulatoryBody                 |

## Module Schema

| Name             | Description                                                                                                                     |
|:-----------------|:--------------------------------------------------------------------------------------------------------------------------------|
| Contacts         | Collects contacts of HIPAA Security Officer(HSO), Covered Entity(CE) and individuals affected by the PHI breach                 |
| Data Compliances | Collects PHI breach Details                                                                                                     |
| Key Store        | Contains a record-set with key-value as *HIPAA* to indicate that **HIPAA Framework** solution pack is installed on the system |


## Connectors

| Name                | Description                                                                                                                                                                                                    |
|:--------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| CSV Data Management | CSV Data management can perform different operations on CSV files like read file, perform deduplication, merge two CSV files, join two CSV files, concatenate two CSV files and return well formatted dataset. |

## Roles

|Name|Description|
| :- | :- |
| Full App Permissions | Essentially the root user, use carefully |

## Report

| Name | Description |
| :- | :- |
| HIPAA Assessment Report | Contains PHI breach risk assessment details |

## Key Store Record Set 

| Name | Description |
| :- | :- |
| HIPAA | This keystore record denotes the name of the solution pack which is deployed on the FortiSOAR |

## Playbook Collection

| 10 - SP - HIPAA Framework |
|:-------------------------:|

| Playbook Name                               | Description                                                                                                                                                                                     |
|:--------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Set Breach Notification SLA                 | Captures the breach notification SLA once incident is resolved                                                                                                                                  |
| Create List of Affected Users               | Creates and links contact information of the individuals affected by the breach to the compliance record.                                                                                       |
| Perform Actions to Apply Technical Fix      | Initiates and carry out the necessary actions to apply the technical fix.                                                                                                                       |
| Get Covered Entity and HSO Contact          | Collects the contact information for the HIPAA Security Officer (HSO) and the address details of the Covered Entity(CE) or Business Associate(BA).                                              |
| Update Description of Compliance Record     | Update Data Compliance Record description when 'Notify Breach to the Secretary of HHS' Task is marked as Completed.                                                                             |
| Reminder for SLA Breach                     | Sends reminder for the notification SLA Breach                                                                                                                                                  |
| Create Data Compliance Record               | Create a data compliance record and link it with a corresponding task and to the parent incident.                                                                                               |
| Notify Individuals Affected by PHI Breach   | Sends email notification to the individuals who have been affected by the PHI breach.                                                                                                           |
| Create Tasks to Notify Affected Individuals | Creates Tasks to Notify Affected Individuals                                                                                                                                                    |
| Report PHI Breach to Law Enforcement Agency | Reports a PHI breach to the Law Enforcement Agency.                                                                                                                                             |
| Get HIPAA Risk Assessment Information       | Collects HIPAA assessment details and completes the corresponding task                                                                                                                          |
| PHI Breach Risk Assessment by HSO           | Sends PHI risk assessment information to HSO (HIPAA Security Officer) for review and receives confirmation on whether the breach is reportable to relevant federal or law enforcement agencies. |
| Confirm Law Enforcement Delay Request       | Confirms law enforcement's delay request for breach notification to affected individuals and pauses breach notification SLA until approval.                                                     |
| Check for SLA violation                     | Checks for breach notification violation and update SLA status to Missed                                                                                                                        |
| Create HIPAA Assessment Tasks               | Creates tasks for HIPAA Assessment and link to HIPAA compliance record                                                                                                                          |

## System View

| Name             | Description                                            |
|:-----------------|:-------------------------------------------------------|
| Data Compliances | Contains menu to access Data Compliance module records |

<table>
    <tr>
        <th>WARNING</th>
        <td>We recommend that you clone these playbooks before customizing to avoid loss of information while upgrading the solution pack.</td>
    </tr>
</table>

# Next Steps
| [Installation](./setup.md#installation) | [Configuration](./setup.md#configuration) | [Usage](./usage.md) |
|-----------------------------------------|-------------------------------------------|---------------------|
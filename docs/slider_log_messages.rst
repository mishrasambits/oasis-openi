.. _warning_messages:

Warning Messages
==========================

General
--------

=================================================================================================================== ====    =====
Message                                                                                                             Code    Level
=================================================================================================================== ====    =====
Observable Expressions should not contain placeholders                                                              201     Error
Both console and output log have disabled messages                                                                  202     Warn
silent option is not compatible with a policy                                                                       203     Warn
options not initialized                                                                                             204     Warn
Comparison Expressions in pattern of *[id]* should only have one type *[root-types]*                                205     Error
=================================================================================================================== ====    =====

Possible issue in original STIX 2.x content
--------------------------------------------------

============================================================================================================== ====    =====
Message                                                                                                        Code    Level
============================================================================================================== ====    =====
No source object exists for *[id]*. Dropping the relationship *[relationship]*                                 301     Warn
Unknown hash type *[hash_type]* used in *[id]*                                                                 302     Warn
NOT ASSIGNED                                                                                                   303
Unknown address type *[type]* used in *[id]*                                                                   304     Warn
ref type *[type]* in *[id]* is not known                                                                       305     Warn
*[cyber_observable_id]* is not found. See *[id]*                                                               306     Warn
No object *[id]* is found to add the reference to                                                              307     Warn
*[id1]* is not in this bundle.  Referenced from *[id2]*                                                        308     Warn
``is_encrypted`` in *[id]* is true, but no ``encryption_algorithm`` is given                                   309     Info
``is_encrypted`` in *[id]* is false, but ``encryption_algorithm`` is given                                     310     Info
``is_encrypted`` in *[id]* is true, but no ``decryption_key`` is given                                         311     Info
``is_encrypted`` in *[id]* is false, but ``decryption_key`` is given                                           312     Info
The *[property1]* property in *[id]* should be '*[boolean]*' if the *[property2]* property is [not] present    313     Warn
Cannot convert *[id]* because it doesn't contain both a source_ref and a target_ref                            314     Warn
No *[ref_property]* object exists for *[id]* in relationship *[rel-id]*                                        315     Warn
ref type *[type]* in *[id]* is not known                                                                       316     Warn
*[id]* referenced in *[id]* is not found                                                                       317     Warn
*[phase_name]* is not part of the Lockheed-Martin Kill Chain - see *[id]*                                      318     Warn
============================================================================================================== ====    =====

Multiple values are not supported in STIX 1.x
----------------------------------------------------

======================================================================================================================== ====    =====
Message                                                                                                                  Code    Level
======================================================================================================================== ====    =====
*[type]* in STIX 2.x has multiple *[property]*, only one is allowed in STIX 1.x. Using first in list - *[value]* omitted  401     Warn
Only one dll can be represented in STIX 1.x for *[id]*, using first one - ignoring *[value]*                              402     Warn
======================================================================================================================== ====    =====

Dropping Content not supported in STIX 1.x
---------------------------------------------------

============================================================================================================================ ====   =====
Message                                                                                                                      Code    Level
============================================================================================================================ ====   =====
The *[relationship]* relationship between *[id1]* and *[id2]* is not supported in STIX 1.x                                   501     Warn
Multiple File Extensions in *[id]* not supported yet                                                                         502     Warn
*[property]* is not representable in a STIX 1.x *[type]*.  Found in *[id]*                                                   503     Warn
*[property]* not representable in a STIX 1.x *[type]*.  Found in the pattern of *[id]*                                       504     Warn
*[op]* cannot be converted to a STIX 1.x operator in the pattern of *[id]*                                                   505     Warn
``account_type`` property of *[id]* in STIX 2.x is not directly represented as a property in STIX 1.x                        506     Warn
Received Line *[line]* in *[id]* has a prefix that is not representable in STIX 1.x                                          507     Warn
Unable to convert STIX 2.x sighting *[id]* because it doesn't refer to an indicator                                          508     Warn
Ignoring *[id]*, because a *[type]* object cannot be represented in STIX 1.1.1                                               509     Warn
Identity has no property to store ``external-references`` from *[id]*                                                        510     Warn
pe_type SYS in *[id]* is valid in STIX 2.x, but not in STIX 1.x                                                              511     Warn
pe_type [pe_type] in *[id]* is allowed in STIX 2.x, but not in STIX 1.x                                                      512     Warn
*[property]* is an XML attribute of *[cybox object type]* in STIX 1.x, so the operator 'equals' is assumed in *[id]*         513     Warn
Order may not be maintained for ``pdfids`` in *[id]*                                                                         514     Warn
The ``groups`` property of ``unix-account-ext`` contains strings, but the STIX 1.x property expects integers in *[property]* 515     Warn
No file name provided for ``binary_ref`` of *[id]*, therefore it cannot be represented in the STIX 1.x ``Process`` object    516     Warn
Hashes of the ``binary_ref`` of *[id]* process cannot be represented in the STIX 1.x ``Process`` object                      517     Warn
resolves_to_refs in *[id]* not representable in STIX 1.x                                                                     518     Warn
Multiple Network Traffic extensions in *[id]* not supported yet                                                              519     Warn
The user_id property of *[id]* in STIX 2.x is only represented as a property in STIX 1.x on ``UnixUserAccount`` objects      520     Warn
The ``path`` property in *[id]* is the only directory property supportable in STIX 1.x. *[property]* is ignored              521     Warn
Nested Archive Files in *[id]* not handled yet                                                                               522     Warn
STIX 1.x can only store the body and headers of an email message in *[id]* independently                                     523     Warn
*[type]* pattern type in *[id]* cannot be represented in STIX 1.x                                                            524     Warn
*[id]* is not explicitly a member of a STIX 1.x ``Report``                                                                   525     Warn
*[id]* cannot be represented in STIX 1.x                                                                                     526     Warn
Relationship between *[id]* and a location is not supported in STIX 1.x                                                      527     Warn
Ignoring *[id]*, because a *[type]* object cannot be represented in STIX 1.x                                                 528     Warn
Unable to populate sub-property *[property]* of *[id]*, therefore *[property]* cannot be represented in the STIX 1.x object  529     Warn
Extensions in *[id]* not supported in STIX 1.x                                                                               530     Warn
Custom extension *[extension name]* of STIX 2.1 in *[id]* are not supported                                                  531     Warn
*[id]* does not support descriptions, so the external reference has been dropped                                             532     Warn
Ignoring *[id]*, because only new-sco extensions are supported                                                               533     Warn
Ignoring *[id]*, because (deprecated) custom objects are not supported                                                       534     Warn
The user account type *[type]* can not be explicitly represented in a STIX 1.x Account. See *[id]*                           535     Warn
============================================================================================================================ ====   =====

STIX Slider currently doesn't process this content
-----------------------------------------------------------
=================================================================================================================== ====    =====
Message                                                                                                             Code    Level
=================================================================================================================== ====    =====
The *[property]* property in *[id]* can refer to any object, so it is not handled yet.                              601     Warn
number indicies in *[id]* not handled, yet                                                                          602     Warn
Unable to determine STIX 1.x type for *[id]*                                                                        603     Error
Granular Markings present in *[id]* are not supported by stix2slider                                                604     Warn
Source name *[name]* in external references of *[id]* not handled, yet                                              605     Warn
*[property]* property in *[id]* not handled yet                                                                     606     Warn
``contains_refs`` in *[id]* not handled                                                                             607     Warn
``protocols`` property in *[id]* not handled, yet                                                                   608     Warn
``tcp-ext`` in *[id]* not handled, yet                                                                              609     Warn
Operator for ``Artifact.Raw_Artifact`` in *[id]* not handled yet                                                    610     Warn
Nested extensions and references in patterns are not handled, yet.  Found in pattern of *[id]*                      611     Warn
*[ref_id]* in *[id]* cannot be represented in STIX 1.x                                                              612     Warn
Multiple extensions in *[id]* are not handled, yet                                                                  613     Warn
*[property]* is an illegal or custom property in the pattern of *[id]*, which is not handled, yet"                  614     Warn
=================================================================================================================== ====    =====

STIX Slider conversion based on assumptions
----------------------------------------------------

=================================================================================================================== ====    =====
Message                                                                                                             Code    Level
=================================================================================================================== ====    =====
Assuming imcp packet in *[id]* is v4                                                                                701     Info
``InformationSource`` descriptions order or content in may not correspond to the references in *[id]*               702     Info
*[ref_id]* in *[id]* cannot be represented explicitly as a member of a STIX 1.x report                              703     Info
=================================================================================================================== ====    =====

<?xml version="1.0" encoding="utf-8"?>
<!-- Created with Liquid Studio 2019 (https://www.liquid-technologies.com) -->
<xs:schema attributeFormDefault="unqualified" elementFormDefault="qualified" xmlns:xs="http://www.w3.org/2001/XMLSchema">
  <xs:element name="xrType">
    <xs:complexType mixed="true">
      <xs:sequence>
        <xs:element minOccurs="0" name="xrInteractiveLevel" type="xs:string" />
        <xs:element minOccurs="0" name="PoI">
          <xs:complexType>
            <xs:attribute name="PoIID" type="xs:string" use="optional" />
          </xs:complexType>
        </xs:element>
        <xs:element minOccurs="0" name="cognitive">
          <xs:complexType>
            <xs:sequence>
              <xs:element minOccurs="0" name="recognitionData" type="xs:string" />
            </xs:sequence>
          </xs:complexType>
        </xs:element>
        <xs:element minOccurs="0" name="creation">
          <xs:complexType>
            <xs:sequence>
              <xs:element minOccurs="0" name="datacite.Creator" type="xs:string" />
              <xs:element minOccurs="0" name="datacite.ContributorType" type="xs:string" />
              <xs:element minOccurs="0" name="creationTitle" type="xs:string" />
              <xs:element minOccurs="0" name="creationFileFormat" type="xs:string" />
              <xs:element minOccurs="0" name="creationFileSize" type="xs:string" />
              <xs:element minOccurs="0" name="creationDate" type="xs:dateTime" />
              <xs:element minOccurs="0" name="creationRights" type="xs:string" />
            </xs:sequence>
            <xs:attribute name="dc.identifier" type="xs:string" use="optional" />
          </xs:complexType>
        </xs:element>
        <xs:element minOccurs="0" name="description">
          <xs:complexType mixed="true">
            <xs:sequence>
              <xs:element minOccurs="0" name="descriptionSubject" type="xs:string" />
              <xs:element minOccurs="0" name="descriptionGeoLocation" type="xs:unsignedInt" />
            </xs:sequence>
            <xs:attribute name="language" type="xs:string" use="optional" />
          </xs:complexType>
        </xs:element>
        <xs:element minOccurs="0" name="usage">
          <xs:complexType>
            <xs:sequence>
              <xs:element minOccurs="0" name="usageAudience" type="xs:string" />
              <xs:element minOccurs="0" name="usageSoftware" type="xs:string" />
              <xs:element minOccurs="0" name="usageMediation" type="xs:string" />
            </xs:sequence>
            <xs:attribute name="usagePurpose" type="xs:string" use="optional" />
          </xs:complexType>
        </xs:element>
        <xs:element minOccurs="0" name="note" type="xs:string" />
        <xs:element minOccurs="0" name="related">
          <xs:complexType>
            <xs:sequence>
              <xs:element minOccurs="0" name="relatedSource" type="xs:string" />
            </xs:sequence>
          </xs:complexType>
        </xs:element>
      </xs:sequence>
      <xs:attribute name="xrFeature" type="xs:string" use="optional" />
    </xs:complexType>
  </xs:element>
</xs:schema>

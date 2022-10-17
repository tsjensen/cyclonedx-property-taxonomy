# Siemens CycloneDX Property Taxonomy, v1.0.0

This is the official Siemens property taxonomy for CycloneDX.

For more information about CycloneDX property taxonomies, refer to
their [official documentation](https://github.com/CycloneDX/cyclonedx-property-taxonomy).

<table>
<thead>
    <tr>
        <th>Property</th>
        <th>Description</th>
    </tr>
</thead>
<tbody>
    <tr style="vertical-align: top;">
        <td><b>siemens:direct</b></td>
        <td>A flag indicating whether the component is a direct dependency (<code>true</code>) or a transitive
            dependency (<code>false</code>).</td>
    </tr>
    <tr style="vertical-align: top;">
        <td><b>siemens:filename</b></td>
        <td>The simple file name of the component, without path. For example, the simple name of a JAR file.</td>
    </tr>
    <tr style="vertical-align: top;">
        <td><b>siemens:legalRemark</b></td>
        <td>Pass-through free text for legal remarks that need to be included in attribution information. A "legal
            remark" is provided by the people creating the SBOM, normally the team behind the product described by
            the SBOM.</td>
    </tr>
    <tr style="vertical-align: top;">
        <td><b>siemens:primaryLanguage</b></td>
        <td>Indicates the primary programming language the artifact is written in.</td>
    </tr>
    <tr style="vertical-align: top;">
        <td><b>siemens:thirdPartyNotices</b></td>
        <td>The contents of all third-party notices found for the component, if any. Note that this is <i>not</i> the
            path to the notice files, but the actual notice text (which may be quite a lot of text). Third-party
            notices are provided by the component's author.<br>
            Since CycloneDX allows only a single String value for this, we separate different notice files by two
            consecutive line feeds.</td>
    </tr>
    <tr style="vertical-align: top;">
        <td><b>siemens:vcsClean</b></td>
        <td>A flag (<code>true</code> or <code>false</code>) indicating whether the Git workspace was clean when the
            SBOM was created, i.e. all changes had been committed.</td>
    </tr>
    <tr style="vertical-align: top;">
        <td><b>siemens:vcsRevision</b></td>
        <td>The most recent VCS hash, for example a Git commit hash. Together with <code>siemens:vcsClean</code>, this
            additional value allows ensuring accurate reproducibility of the SBOM.</td>
    </tr>
</tbody>
</table>


## Contributing

These properties are maintained by Siemens. Feel free to raise an issue if you have any questions.


## License

Copyright 2022 Siemens AG.

Licensed under [Apache License 2.0](./LICENSE).

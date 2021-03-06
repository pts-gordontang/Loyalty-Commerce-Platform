## Loyalty Programs (LPs)

A loyalty program (LP) allows applications to perform member validations, debits, and credits against the loyalty program’s member database. Loyalty programs are found under the `/lps` endpoint.

#### Properties

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>createdAt</td>
            <td>The <a href="http://en.wikipedia.org/wiki/ISO_8601">ISO 8601</a> time when the resource was created.</td>
        </tr>
        <tr>
            <td>creditType</td>
            <td>Indicates whether the LP requires base and bonus points to be fulfilled as one credit or as two separate credits.</td>
        </tr>
        <tr>
            <td>defaultLanguage</td>
            <td>The default language of the loyalty program. The name, partnerName, and rewardCurrency properties are in this language. <a href="http://en.wikipedia.org/wiki/IETF_language_tag">IETF language tags</a> are used.</td>
        </tr>
        <tr>
            <td>hidden</td>
            <td>Flag indicating whether the LP is shown in the list of LPs.</td>
        </tr>
        <tr>
            <td>name</td>
            <td>The name of the loyalty program.</td>
        </tr>
        <tr>
            <td>partnerId</td>
            <td>A four character string uniquely identifying the loyalty program.</td>
        </tr>
        <tr>
            <td>partnerName</td>
            <td>The partner associated with the loyalty program.</td>
        </tr>
        <tr>
            <td>rewardCurrency</td>
            <td>The name of the reward currency (e.g. points or miles).</td>
        </tr>
        <tr>
            <td>translations</td>
            <td>A set of language translations for the name, partnerName, and rewardCurrency properties. <a href="http://en.wikipedia.org/wiki/IETF_language_tag">IETF language tags</a> are used.</td>
        </tr>
        <tr>
            <td>type</td>
            <td>The type of resource.</td>
        </tr>
        <tr>
            <td>updatedAt</td>
            <td>The <a href="http://en.wikipedia.org/wiki/ISO_8601">ISO 8601</a> time when the resource was last updated.</td>
        </tr>
    </tbody>
</table>















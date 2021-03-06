### Create an MV Delegate

A loyalty program creates an MV delegate to pass an authenticated user to another application. To create an MV delegate, provide all the member information that is normally included in an MV request and response as well as the application that should have access to the MV. As a side effect, the LCP creates an MV using the provided member information and gives the other application read access to the MV. The LCP creates the MV without contacting the loyalty program since the creator of the MV delegate is considered a trusted source of member information. Only loyalty program applications can create MV delegates.

The MV delegate response contains a link to the created MV. The loyalty program should redirect the user to the other application and pass the MV link to the other application. The other application then retrieves the MV and the member information. Using this method, the application does not have to collect member credentials to create its own MV. Instead, the application can immediately use the MV for debits and credits since the loyalty program has already validated the member’s credentials.

#### Parameters

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>lp-id</td>
            <td>The identifier of the <a href="#loyalty-programs">loyalty program</a> (LP) making the request.</td>
        </tr>
        <tr>
            <td>application</td>
            <td>The application that will have permission to access the member validation.</td>
        </tr>
        <tr>
            <td>identifyingFactors</td>
            <td>Dictionary of fields that identify the loyalty program member (e.g., firstName, lastName, memberId). Varies based on the LP’s <a href="#mv-request-schema">MV request schema</a>.</td>
        </tr>
        <tr>
            <td>authenticatingFactors</td>
            <td>Dictionary of fields that authenticate the loyalty program member (e.g., password, pin). These fields are not displayed. Varies based on the LP’s <a href="#mv-request-schema">MV request schema</a>.</td>
        </tr>
        <tr>
            <td>balance</td>
            <td>The balance in the loyalty program member’s account.</td>
        </tr>
        <tr>
            <td>order</td>
            <td>Link to the order that this member validation belongs to (optional).</td>
        </tr>
    </tbody>
</table>

#### Returns

The MV delegate object if it was created successfully. Returns an [error](./?doc=reference-manual#errors) if any of the required MV request and response fields for the given LP are not provided.



















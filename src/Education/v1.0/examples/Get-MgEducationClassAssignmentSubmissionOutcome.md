### Example 1: Update a feedback outcome

```powershellImport-Module Microsoft.Graph.Education

$params = @{
	"@odata.type" = "#microsoft.graph.educationFeedbackOutcome"
}

Update-MgEducationClassAssignmentSubmissionOutcome -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -EducationSubmissionId $educationSubmissionId -EducationOutcomeId $educationOutcomeId -BodyParameter $params
```
This example shows how to use the Get-MgEducationClassAssignmentSubmissionOutcome Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

### Example 2: Update a points outcome

```powershellImport-Module Microsoft.Graph.Education

$params = @{
	"@odata.type" = "#microsoft.graph.educationPointsOutcome"
	points = @{
		"@odata.type" = "#microsoft.graph.educationAssignmentPointsGrade"
		points = 
	}
}

Update-MgEducationClassAssignmentSubmissionOutcome -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -EducationSubmissionId $educationSubmissionId -EducationOutcomeId $educationOutcomeId -BodyParameter $params
```
This example shows how to use the Get-MgEducationClassAssignmentSubmissionOutcome Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

### Example 3: Update a rubric outcome

```powershellImport-Module Microsoft.Graph.Education

$params = @{
	"@odata.type" = "#microsoft.graph.educationRubricOutcome"
	rubricQualityFeedback = @(
	)
	rubricQualitySelectedLevels = @(
	)
}

Update-MgEducationClassAssignmentSubmissionOutcome -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -EducationSubmissionId $educationSubmissionId -EducationOutcomeId $educationOutcomeId -BodyParameter $params
```
This example shows how to use the Get-MgEducationClassAssignmentSubmissionOutcome Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).


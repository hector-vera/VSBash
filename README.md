# VSBash
curl -O -L https://downloads.veracode.com/securityscan/pipeline-scan-LATEST.zip
unzip -o pipeline-scan-LATEST.zip
java -jar pipeline-scan.jar --veracode_api_id "${VERACODE_API_ID}" --veracode_api_key "${VERACODE_API_KEY}" --issue_details true --file app/target/verademo.war --fail_on_severity="Very High, High"

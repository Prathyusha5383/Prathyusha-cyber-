# Cybersecurity Asset Risk Management

assets = [
    {
        "assetID": "A101",
        "assetName": "HR-PC-01",
        "assetType": "Workstation",
        "ipAddress": "192.168.1.10",
        "operatingSystem": "Windows 11",
        "department": "HR",
        "riskLevel": "Medium",
        "securityStatus": "Secure"
    },
    {
        "assetID": "A102",
        "assetName": "Web-Server",
        "assetType": "Server",
        "ipAddress": "192.168.1.20",
        "operatingSystem": "Ubuntu",
        "department": "IT",
        "riskLevel": "Critical",
        "securityStatus": "Vulnerable"
    },
    {
        "assetID": "A103",
        "assetName": "Core-Router",
        "assetType": "Router",
        "ipAddress": "192.168.1.1",
        "operatingSystem": "Cisco IOS",
        "department": "Network",
        "riskLevel": "High",
        "securityStatus": "Warning"
    }
]


# Display all assets
print("===== CYBERSECURITY ASSET INVENTORY =====")

for asset in assets:
    print("\nAsset ID       :", asset["assetID"])
    print("Asset Name     :", asset["assetName"])
    print("Asset Type     :", asset["assetType"])
    print("IP Address     :", asset["ipAddress"])
    print("Operating System:", asset["operatingSystem"])
    print("Department     :", asset["department"])
    print("Risk Level     :", asset["riskLevel"])
    print("Security Status:", asset["securityStatus"])


# Find critical and high-risk assets
print("\n===== HIGH-RISK ASSETS =====")

for asset in assets:
    if asset["riskLevel"] in ["Critical", "High"]:
        print(
            asset["assetName"],
            "-> Risk:",
            asset["riskLevel"],
            "| Status:",
            asset["securityStatus"]
        )


# Find vulnerable assets
print("\n===== VULNERABLE ASSETS =====")

for asset in assets:
    if asset["securityStatus"] == "Vulnerable":
        print(
            asset["assetName"],
            "-> IP:",
            asset["ipAddress"]
        )


# Display summary
critical = 0
high = 0
medium = 0
secure = 0
vulnerable = 0
warning = 0

for asset in assets:

    if asset["riskLevel"] == "Critical":
        critical += 1
    elif asset["riskLevel"] == "High":
        high += 1
    elif asset["riskLevel"] == "Medium":
        medium += 1

    if asset["securityStatus"] == "Secure":
        secure += 1
    elif asset["securityStatus"] == "Vulnerable":
        vulnerable += 1
    elif asset["securityStatus"] == "Warning":
        warning += 1


print("\n===== ASSET SUMMARY =====")
print("Total Assets       :", len(assets))
print("Critical Risk      :", critical)
print("High Risk          :", high)
print("Medium Risk        :", medium)
print("Secure Assets      :", secure)
print("Vulnerable Assets  :", vulnerable)
print("Warning Assets     :", warning)

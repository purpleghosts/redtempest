# Red Tempest

**Red Tempest** is a suite for cybersecurity counterintelligence red team ops, designed to generate false alerts and noise to obscure real attacker activities. Using techniques like IP, MAC spoofing, TOR or SOCKS services, Red Tempest is designed to create credible false signals across various protocols, including C2 UDP traffic, DNS, Kerberos, SNMP and more. The goal is to overflow SOCs and defensive teams with misleading data, enhancing the stealth of offensive operations. 

Red Tempest offers a powerful toolset for red teams looking to maintain anonymity and increase the complexity of their engagements.

## Features

- **C2 UDP Traffic Generator**: Generate internal false Command and Control traffic to known malicious C2 servers.
- **C2 DNS Resolution Spoofing**: Spoof internal DNS requests to domains associated with C2 activities.
- **Kerberoasting Spoofing**: Perform internal Kerberoasting attacks with spoofed IP addresses.
- **External Web Attacks via Tor**: Simulate external web attacks using the Tor network / Socks for anonymity.
- **UDP Exfiltration Simulation**: Generate internal massive UDP traffic to external IPs to simulate data exfiltration.
- **Rsyslog False Alerts**: Inject internal false alert events into Rsyslog services.
- **Network Scanning Simulation**: Simulate internal network scanning activities with Fake IP.
- **SNMP Brute Force Attacks**: Perform internal SNMP brute force attacks with spoofed IP and MAC addresses.
- **Office 365 Authentication Simulation**: Perform external brute force attacks on Office 365 accounts using Tor network / Socks for anonymity.
- **Malicious Email Injection in Office 365**: Send external fake malicious emails directly into Office 365 tenants using Tor network / Socks for anonymity.
- **OpenVPN Traffic Simulation**: Generate internal fake OpenVPN UDP traffic to simulate suspicious network activity.
- **SIP VoIP Traffic Simulation**: Simulate internal SIP requests to generate false VoIP traffic.
- **LDAP Brute Force Simulation**: Send internal spoofed LDAP AUTH requests over UDP with fake IP and MAC addresses.
- **Kerberos Brute Force Simulation**: Simulate internal Kerberos brute force attacks with spoofed IP and MAC addresses.
- **Fortigate VPN-SSL Brute Force Simulation**: Perform external brute force attacks on Fortigate VPN-SSL portals using Tor network / Socks for anonymity.

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/redtempest-lab/red-tempest.git
    ```
2. Navigate to the project directory:
    ```sh
    cd red-tempest
    ```
3. Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```

## Usage
1. Each module in the suite can be executed independently. Here are some examples:
    ```sh
    python red-tempest-c2.py --source-ip <spoofed-ip> --random-mac --delay 10 --destination-c2 <whell-know-c2-list>
    ```

## Contributing

We welcome contributions to enhance Red Tempest. Please fork the repository and create a pull request with your changes.

## License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE](LICENSE) file for details.

## Disclaimer

Red Tempest is intended for educational and ethical testing purposes only. Misuse of this tool for malicious activities is illegal and strictly prohibited.



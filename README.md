# Red Tempest

**Red Tempest** is a suite for cybersecurity counterintelligence red team ops, designed to generate false alerts and noise to obscure real attacker activities. Using techniques like IP and MAC spoofing, Red Tempest creates credible false signals across various protocols, including C2 UDP traffic, DNS, Kerberos, SNMP and more. The goal is to saturate SOCs and defensive teams with misleading data, enhancing the stealth of offensive operations. 

Red Tempest offers a powerful toolset for red teams looking to maintain anonymity and increase the complexity of their engagements.

## Features

- **C2 UDP Traffic Generator**: Generate false Command and Control traffic to known malicious C2 servers.
- **C2 DNS Resolution Spoofing**: Spoof DNS requests to domains associated with C2 activities.
- **Kerberoasting Spoofing**: Perform Kerberoasting attacks with spoofed IP addresses.
- **External Web Attacks via Tor**: Simulate various web attacks using the Tor network for anonymity.
- **UDP Exfiltration Simulation**: Generate massive UDP traffic to simulate data exfiltration.
- **Rsyslog False Alerts**: Inject false alert events into Rsyslog.
- **Network Scanning Simulation**: Simulate network scanning activities with Fake IP.
- **SNMP Brute Force Attacks**: Perform SNMP brute force attacks with spoofed IP and MAC addresses.

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

Each module in the suite can be executed independently. Here are some examples:

- **C2 UDP Traffic Generator**:
    ```sh
    python red-tempest-c2.py --source-ip <spoofed-ip> --random-mac --delay 10 --destination-c2 <whell-know-c2-list>
    ```
## Contributing

We welcome contributions to enhance Red Tempest. Please fork the repository and create a pull request with your changes.

## License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE](LICENSE) file for details.

## Disclaimer

Red Tempest is intended for educational and ethical testing purposes only. Misuse of this tool for malicious activities is illegal and strictly prohibited.



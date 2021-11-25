# Software Defined Networking (SDN) with OpenFlow

<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;"><strong>OpenFlow:</strong></span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">
        <span style="color: rgb(84, 172, 210);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;OpenFlow&nbsp;</span>is a protocol that enables <span style="color: rgb(84, 172, 210);">SDN&nbsp;</span>(Software defined networking), which
        makes it the backbone of SDN. It is a communication protocol which separates the routing and switching logic from the actual forwarding.
    </span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">&nbsp;</span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;"><strong>Software Defined Networking:</strong></span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">
        &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;It is a technology which enables dynamic network configuration and management. This helps to improve performance, provide scalability and flexibility.
    </span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;"><br /></p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;"><u>The device templates used for the stimulation of a basic network are:</u></span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;"><strong>SDN Controller:</strong></span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">
        &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; It is a centralized application that acts as the control point for the Software defined networking.<span style="color: rgb(84, 172, 210);">&nbsp;Faucet SDN controller</span> is
        used in this architecture. &nbsp; &nbsp;&nbsp;
    </span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">The configuration can be found in the following file of the controller:</span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif; text-align: center;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">
        <em><span style="background: lightgrey;">/etc/faucet/faucet.yaml</span></em>
    </span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">Command to check the setting is proper:</span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif; text-align: center;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">
        <em><span style="background: lightgrey;">check_faucet_config /etc/faucet/faucet.yaml</span></em>
    </span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">Command to reload with new configuration:</span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif; text-align: center;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">
        <em><span style="background: lightgrey;">pkill -HUP ryu-manager</span></em>
    </span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;"><strong>Open vSwitch:</strong></span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">
        &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; It is a data switch that communicates to the centralized or external controller, using <span style="color: rgb(84, 172, 210);">OpenFlow</span>. Open vSwitch contains flow
        tables which are used for forwarding the packets based on the information stored in them, called Flow entries. Flow tables can be manipulated using SDN controller, programmatically.
    </span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">Command to show controller information:</span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif; text-align: center;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">
        <em><span style="background: lightgrey;">ovs-vsctl list controller</span></em>
    </span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">Command to show current flow information:</span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif; text-align: center;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">
        <em><span style="background: lightgrey;">ovs-ofctl dump-flows br0</span></em>
    </span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;"><strong>DHCP Server:</strong></span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">
        &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; DHCP server dynamically assigns IP addresses to the nodes. To start DHCP service and assign all devices with IPs, the following command is used:
    </span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif; text-align: center;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">
        <em><span style="background: lightgrey;">/etc/init.d/isc-dhcp-server start</span></em>
    </span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">&nbsp;</span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;"><strong>Ethernet Switch:</strong></span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">
        &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; This is a built in GNS3 switch. It is only used to connect the Open vSwitches to the SDN controller.
    </span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;"><strong>Web Server:</strong></span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">
        &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; A Linux based web server is connected an Open vSwitch, which contains nginx server. The following commands is used for nginx:
    </span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">To start:</span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 17.95pt; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif; text-align: center;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">
        <em><span style="background: lightgrey;">sudo service nginx start</span></em>
    </span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">To stop:</span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif; text-align: center;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">
        <em><span style="background: lightgrey;">sudo service nginx stop</span></em>
    </span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">To restart:</span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif; text-align: center;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">
        <em><span style="background: lightgrey;">sudo service nginx restart</span></em>
    </span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;"><strong>Web terms:</strong></span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; Web terms are used acting as client nodes, which are connecting the Open vSwitches.</span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">&nbsp;</span>
</p>
<p style="margin-top: 0cm; margin-right: 0cm; margin-bottom: 8pt; margin-left: 0cm; line-height: 107%; font-size: 15px; font-family: 'Calibri', sans-serif;">
    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px;">&nbsp;</span>
</p>


# A03U - Activitat 3 - DHCP a Win 2020 Server (examen)

## Objectiu

Instal·lació i configuració del **```servei de DHCP```** en un servidor **Windows 2022 Server**.

## Eines

Per tal de dur a terme la pràctica la instal·lació s'implementarà sobre una màquina **Windows 2022 Server**. També caldrà que tingueu una maquina client amb dues interfícies de xarxa.

Com a *Sistema Operatiu client* podreu fer servir qualsevol màquina virtual que tingui la possibilitat de configurar-li dues interfícies de xarxa perquè rebin la configuració de xarxa de forma automàtica.

## Passos per realitzar l'activitat

**1.** Cal que modifiqueu el nom del vostre servidor. El nom d'aquest cal que sigui **```<CognomAlumne>examen```**, on **```<CognomAlumne>```** serà **només** el vostre **cognom** **sense el nom**. Per exemple, en el meu cas seria **```pardoexamen```**.

**2.** Cal verificar que el vostre servidor disposa de **dues interfícies de xarxa**:

   * la primera interfície de xarxa del servidor que donarà sortida a Internet, estarà configurada com a **```NAT```**.

   * la segona interfície de xarxa, estarà configurada com a **```Xarxa interna```**, i tindrà la següent IP fixa
        **```172.128.<mesDelVostreAniversari>.1/24```**

**3.** El **rang d'adreces IP** que assignarà el vostre servidor **DHCP**, anirà des de l'adreça IP:

 * **```172.128.<mesDelVostreAniversari>.50```**, fins a la
 
 * **```172.128.<mesDelVostreAniversari>.150```**.

**4.** Les **adreces dels servidors de DNS** que assignarà el vostre **servidor DHCP**, cal que siguin les dues **DNS de google**.

**5.** El vostre **```servidor DHCP```** assignarà de manera **fixa** (*caldrà fer una reserva*) l'adreça IP **```172.128.<mesDelVostreAniversari>.55/24```** a una de les interfícies de xarxa de la vostra màquina client. Per tant, caldrà que esbrineu quina *MacAddress* té la interfície de xarxa del client.

## Avaluació

Com a condició imprescindible per aprovar, cal que:

**1.** el servidor **DHCP** funcioni correctament, és a dir,

  * **1.1.** que assigni la ip **```172.128.<mesDelVostreAniversari>.55/24```** a una de les interfícies de xarxa de la vostra màquina client, i

   * **1.2.** que assigni una adreça ip, del rang d'adreces demanat, de manera dinàmica a l'altra interfície de xarxa de la vostra màquina client.

**2.** A part caldrà que respongueu correctament, demostrant que heu entès l'activitat, a un parell de preguntes que us faré, **SEMPRE** relacionades amb aquesta activitat, durant el dia de l'examen.
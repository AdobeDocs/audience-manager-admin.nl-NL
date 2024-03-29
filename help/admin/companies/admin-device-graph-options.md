---
description: De opties voor apparaatgrafiek zijn beschikbaar voor bedrijven die deelnemen aan de Adobe Experience Cloud Device Co-op. Als een klant ook een contractuele relatie heeft met een externe provider van apparaatgrafieken die is geïntegreerd met Audience Manager, worden in deze sectie opties voor die apparaatgrafiek weergegeven. U vindt deze opties in Bedrijven > bedrijfsnaam > Profiel > Opties apparaatgrafiek.
seo-description: The Device Graph Options are available to companies that participate in the Adobe Experience Cloud Device Co-op. If a customer also has a contractual relationship with a third-party device graph provider that is integrated with Audience Manager, this section will show options for that device graph. These options are located in Companies > company name > Profile > Device Graph Options.
seo-title: Device Graph Options for Companies
title: Device graph-opties voor bedrijven
uuid: a8ced843-710c-4a8f-a0d7-ea89d010a7a5
exl-id: 2502f3d2-b43c-410c-acb6-03c2a2ba2c1d
source-git-commit: 1f4dbf8f7b36e64c3015b98ef90b6726d0e7495a
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 3%

---

# Device graph-opties voor bedrijven {#device-graph-options-for-companies}

De [!UICONTROL Device Graph Options] beschikbaar zijn voor ondernemingen die deelnemen aan de [!DNL Adobe Experience Cloud Device Co-op]. Als een klant ook een contractuele relatie heeft met een externe provider van apparaatgrafieken die is geïntegreerd met Audience Manager, worden in deze sectie opties voor die apparaatgrafiek weergegeven. Deze opties bevinden zich in [!UICONTROL Companies] > Bedrijfsnaam > [!UICONTROL Profile] > [!UICONTROL Device Graph Options].

![](assets/adminUIdataSource.png)

Deze illustratie gebruikt generieke namen voor de grafiekopties van apparaten van derden. In productie, komen deze namen uit de leverancier van de apparatengrafiek en kunnen van wat variëren hier wordt getoond. De [!DNL LiveRamp] opties meestal (maar niet altijd):

* Beginnen met &quot;[!DNL LiveRamp]&quot;
* Bevat een variërende middelste naam
* Eindigen met &quot;[!UICONTROL - Household]&quot; of &quot;[!UICONTROL -Person]&quot;

## Apparaatgrafiekopties gedefinieerd {#device-graph-options-defined}

Met de opties voor apparaatgrafieken die u hier selecteert, kunt u de [!UICONTROL Device Options] keuzemogelijkheden voor een [!DNL Audience Manager] klanten wanneer zij een [!UICONTROL Profile Merge Rule].

### Afbeelding van apparaat voor coop {#co-op-graph}

Klanten die deelnemen aan de [Adobe Experience Cloud Device Co-op](https://experienceleague.adobe.com/docs/device-co-op/using/about/overview.html?lang=en) Gebruik deze opties om een [!UICONTROL Profile Merge Rule] with [deterministische en probabilistische gegevens](https://experienceleague.adobe.com/docs/device-co-op/using/device-graph/links.html?lang=en). De [!DNL Corporate Provisioning Team] activeert en deactiveert deze optie via een achterste eind [!DNL API] vraag. U kunt deze vakken niet in het dialoogvenster [!DNL Admin UI]. Ook de **[!UICONTROL Co-op Device Graph]** en **[!UICONTROL Company Device Graph]** opties sluiten elkaar uit . Klanten kunnen ons vragen het ene of het andere te activeren, maar niet beide. Als deze optie is ingeschakeld, wordt de **[!UICONTROL Co-op Device Graph]** controle in de [!UICONTROL Device Options] instellingen voor een [!UICONTROL Profile Merge Rule].

![](assets/adminUI1.png)

### Bedrijfsapparaatgrafiek {#company-graph}

Deze optie is bedoeld voor [!DNL Analytics] klanten die de [!UICONTROL People] metrieke [!DNL Analytics] rapportsuite. De [!DNL Corporate Provisioning Team] activeert en deactiveert deze optie via een achterste eind [!DNL API] vraag. U kunt deze vakken niet in het dialoogvenster [!DNL Admin UI]. Ook de **[!UICONTROL Company Device Graph]** en **[!UICONTROL Co-op Device Graph]** opties sluiten elkaar uit . Klanten kunnen ons vragen het ene of het andere te activeren, maar niet beide. Indien ingeschakeld:

* Deze apparatengrafiek gebruikt deterministische gegevens die tot het bedrijf behoren u (geen probabilistische gegevens) vormt.
* [!DNL Audience Manager] maakt automatisch een [!UICONTROL Data Source] gebeld `*`partnernaam`*-Company Device Graph-Person`. In de [!UICONTROL Data Source] detailpagina, [!DNL Audience Manager] klanten kunnen de partnernaam, beschrijving veranderen en toepassen [Besturingselementen voor gegevensexport](https://experienceleague.adobe.com/docs/device-co-op/using/device-graph/links.html?lang=en) naar deze gegevensbron.
* [!DNL Audience Manager] klanten *niet* zie een nieuwe instelling in het dialoogvenster [!UICONTROL Device Options] sectie voor een [!UICONTROL Profile Merge Rule].

### Grafiek LiveRamp-apparaat (persoonlijk of in het huishouden) {#liveramp-device-graph}

Deze selectievakjes zijn ingeschakeld in het dialoogvenster [!DNL Admin UI] wanneer een partner een [!UICONTROL Data Source] en selecteert **[!UICONTROL Use as an Authenticated Profile]** en/of **[!UICONTROL Use as a Device Graph]**. De namen voor deze instellingen worden bepaald door de externe provider van apparaatgrafieken (bijvoorbeeld [!DNL LiveRamp], [!DNL TapAd], enz.). Als deze optie is ingeschakeld, betekent dit dat het bedrijf dat u configureert, gegevens zal gebruiken die door deze apparaatgrafieken worden verschaft.

![](assets/adminUI2.png)

>[!MORELIKETHIS]
>
>* [Definities van opties voor regels voor profielsamenvoeging](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/profile-merge-rules/merge-rule-definitions.html?lang=en).
>* [Instellingen gegevensbron en menuopties](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/data-sources/datasources-list-and-settings.html?lang=en)


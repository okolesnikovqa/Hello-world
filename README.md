# Hello-world
Learning GitHub

@smoke-test @not-mobile @not-tablet
Feature: ST 12.1.1 : Smoke Test : Level 1

  These scenarios will run basic tests to open and verify KPIs and Dashboards loaded without errors 


  Scenario: 12.1.1.1 : An 'Admin' user should be able to verify KPIs renders for "Data Entry Rate - Country" (Site Productivity FOLDER)
   When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
   And I switch to the 'CCDM' account if I am on another account   
   And I open a folder named 'Site Productivity' from the analytics list
   Then I should see I am on the 'Site Productivity' page
   When I navigate to the page containing the analytics named 'Data Entry Rate - Country'
   And I open the analytics named 'Data Entry Rate - Country'
   And I should see I am on the 'Data Entry Rate - Country' page
   Then I should see 'Select filters to proceed.' in the report body
   When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
   And I select 'Beta 21' from the 'Study' session filter dropdown
   And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
   Then I can see the following study in the 'Study' session filter minimized view:
   | Beta 21 |
   When I open the 'Filters' panel
   And I select the following values from the 'Site Country' included dropdown filter: 
   | Argentina |
   Then the 'Site Country' included dropdown filter should contain the following filter tags:
   | Argentina |
   And I should see I am on the 'Data Entry Rate - Country' page
   And I can see the analytics has rendered

   Scenario: 12.1.1.2 : An 'Admin' user should be able to verify KPIs renders for "Data Entry Rate - Site" (Site Productivity FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Site Productivity' from the analytics list
    Then I should see I am on the 'Site Productivity' page
    When I navigate to the page containing the analytics named 'Data Entry Rate - Site'
    And I open the analytics named 'Data Entry Rate - Site'
    Then I should see I am on the 'Data Entry Rate - Site' page
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    When I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I should see 'Select filters to proceed.' in the report body
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
    When I select the following values from the 'Site Name' included dropdown filter: 
    | Center Pharmatech |
    Then the 'Site Name' included dropdown filter should contain the following filter tags:
    | Center Pharmatech |
    And I should see I am on the 'Data Entry Rate - Site' page
    And I can see the analytics has rendered
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I remove 'Beta 21' from the 'Study' session filter dropdown

   Scenario: 12.1.1.3 : An 'Admin' user should be able to verify KPIs renders for "Data Entry Rate - Study" (Site Productivity FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Site Productivity' from the analytics list
    Then I should see I am on the 'Site Productivity' page
    When I open the analytics named 'Data Entry Rate - Study'
    And I should see I am on the 'Data Entry Rate - Study' page
    Then I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I can see the analytics has rendered

   Scenario: 12.1.1.4 : An 'Admin' user should be able to verify KPIs renders for "Drug Accountability by Status - Country" (Site Productivity FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Site Productivity' from the analytics list
    And I open the analytics named 'Drug Accountability by Status - Country'
    Then I should see I am on the 'Drug Accountability by Status - Country' page
    And I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
   | Beta 21 |
   When I open the 'Filters' panel
   And I select the following values from the 'Site Country' included dropdown filter: 
   | Argentina |
   Then the 'Site Country' included dropdown filter should contain the following filter tags:
   | Argentina |
   And I should see I am on the 'Drug Accountability by Status - Country' page
   And I can see the analytics has rendered

    Scenario: 12.1.1.5 : An 'Admin' user should be able to verify KPIs renders for "Drug Accountability by Status - Site" (Site Productivity FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Site Productivity' from the analytics list
    Then I should see I am on the 'Site Productivity' page
    When I open the analytics named 'Drug Accountability by Status - Site'
    Then I should see I am on the 'Drug Accountability by Status - Site' page
    And I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I should see 'Select filters to proceed.' in the report body
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
    When I select the following values from the 'Site Name' included dropdown filter: 
    | Center Pharmatech |
    And the 'Site Name' included dropdown filter should contain the following filter tags:
    | Center Pharmatech |
    And I can see the analytics has rendered


Scenario: 12.1.1.6 : An 'Admin' user should be able to verify KPIs renders for "Drug Accountability by Status - Study" (Site Productivity FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
   And I switch to the 'CCDM' account if I am on another account   
   And I open a folder named 'Site Productivity' from the analytics list
   Then I should see I am on the 'Site Productivity' page
   When I navigate to the page containing the analytics named 'Drug Accountability by Status - Study'
   And I open the analytics named 'Drug Accountability by Status - Study'
   And I should see I am on the 'Drug Accountability by Status - Study' page
   Then I should see 'Select filters to proceed.' in the report body
   When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
   And I select 'Beta 21' from the 'Study' session filter dropdown
   And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
   Then I can see the following study in the 'Study' session filter minimized view:
   | Beta 21 |
   And I should see I am on the 'Drug Accountability by Status - Study' page
   And I can see the analytics has rendered

 Scenario: 12.1.1.7 : An 'Admin' user should be able to verify KPIs renders for "Issue Resolution - Country" (Site Productivity FOLDER)
   When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
   And I switch to the 'CCDM' account if I am on another account   
   And I open a folder named 'Site Productivity' from the analytics list
   Then I should see I am on the 'Site Productivity' page
   When I navigate to the page containing the analytics named 'Issue Resolution - Country'
   And I open the analytics named 'Issue Resolution - Country'
   And I should see I am on the 'Issue Resolution - Country' page
   Then I should see 'Select filters to proceed.' in the report body
   When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
   And I select 'Beta 21' from the 'Study' session filter dropdown
   And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
   Then I can see the following study in the 'Study' session filter minimized view:
   | Beta 21 |
   When I open the 'Filters' panel
   And I select the following values from the 'Site Country' included dropdown filter: 
   | Argentina |
   Then the 'Site Country' included dropdown filter should contain the following filter tags:
   | Argentina |
   And I should see I am on the 'Issue Resolution - Country' page
   And I can see the analytics has rendered

   Scenario: 12.1.1.8 : An 'Admin' user should be able to verify KPIs renders for "Issue Resolution - Site" (Site Productivity FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Site Productivity' from the analytics list
    Then I should see I am on the 'Site Productivity' page
    When I open the analytics named 'Issue Resolution - Site'
    Then I should see I am on the 'Issue Resolution - Site' page
    And I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I should see 'Select filters to proceed.' in the report body
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
    When I select the following values from the 'Site Name' included dropdown filter: 
    | Mountain Novex Research Center Radiant |
    And the 'Site Name' included dropdown filter should contain the following filter tags:
    | Mountain Novex Research Center Radiant |
    And I can see the analytics has rendered

Scenario: 12.1.1.9 : An 'Admin' user should be able to verify KPIs renders for "Issue Resolution - Study" (Site Productivity FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
   And I switch to the 'CCDM' account if I am on another account   
   And I open a folder named 'Site Productivity' from the analytics list
   Then I should see I am on the 'Site Productivity' page
   When I navigate to the page containing the analytics named 'Issue Resolution - Study'
   And I open the analytics named 'Issue Resolution - Study'
   And I should see I am on the 'Issue Resolution - Study' page
   Then I should see 'Select filters to proceed.' in the report body
   When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
   And I select 'Beta 21' from the 'Study' session filter dropdown
   And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
   Then I can see the following study in the 'Study' session filter minimized view:
   | Beta 21 |
   And I should see I am on the 'Issue Resolution - Study' page
   And I can see the analytics has rendered


 Scenario: 12.1.1.10 : An ‘Advanced’ user should be able to verify KPIs renders "Missing Data per Visit - Study" (Site Productivity FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
   And I switch to the 'CCDM' account if I am on another account   
   And I open a folder named 'Site Productivity' from the analytics list
   Then I should see I am on the 'Site Productivity' page
   When I navigate to the page containing the analytics named 'Missing Data per Visit - Study'
   And I open the analytics named 'Missing Data per Visit - Study'
   And I should see I am on the 'Missing Data per Visit - Study' page
   Then I should see 'Select filters to proceed.' in the report body
   When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
   And I select 'Beta 21' from the 'Study' session filter dropdown
   And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
   Then I can see the following study in the 'Study' session filter minimized view:
   | Beta 21 |
   And I should see I am on the 'Missing Data per Visit - Study' page
   And I can see the analytics has rendered

  Scenario: 12.1.1.11 : An 'Admin' user should be able to verify KPIs renders for "Monitoring Visits Past Due - Country" (Site Productivity FOLDER)
   When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
   And I switch to the 'CCDM' account if I am on another account   
   And I open a folder named 'Site Productivity' from the analytics list
   Then I should see I am on the 'Site Productivity' page
   When I navigate to the page containing the analytics named 'Monitoring Visits Past Due - Country'
   And I open the analytics named 'Monitoring Visits Past Due - Country'
   And I should see I am on the 'Monitoring Visits Past Due - Country' page
   Then I should see 'Select filters to proceed.' in the report body
   When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
   And I select 'Beta 21' from the 'Study' session filter dropdown
   And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
   Then I can see the following study in the 'Study' session filter minimized view:
   | Beta 21 |
   When I open the 'Filters' panel
   And I select the following values from the 'Site Country' included dropdown filter: 
   | Argentina |
   Then the 'Site Country' included dropdown filter should contain the following filter tags:
   | Argentina |
   And I should see I am on the 'Monitoring Visits Past Due - Country' page
   And I can see the analytics has rendered

   Scenario: 12.1.1.12 : An 'Admin' user should be able to verify KPIs renders for "Monitoring Visits Past Due - Study" (Site Productivity FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Site Productivity' from the analytics list
    Then I should see I am on the 'Site Productivity' page
    When I open the analytics named 'Monitoring Visits Past Due - Study'
    And I should see I am on the 'Monitoring Visits Past Due - Study' page
    Then I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I can see the analytics has rendered

  Scenario: 12.1.1.13 : An 'Admin' user should be able to verify KPIs renders for "Open Queries by Age - Country" (Site Productivity FOLDER)
   When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
   And I switch to the 'CCDM' account if I am on another account   
   And I open a folder named 'Site Productivity' from the analytics list
   Then I should see I am on the 'Site Productivity' page
   When I navigate to the page containing the analytics named 'Open Queries by Age - Country'
   And I open the analytics named 'Open Queries by Age - Country'
   And I should see I am on the 'Open Queries by Age - Country' page
   Then I should see 'Select filters to proceed.' in the report body
   When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
   And I select 'Beta 21' from the 'Study' session filter dropdown
   And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
   Then I can see the following study in the 'Study' session filter minimized view:
   | Beta 21 |
   When I open the 'Filters' panel
   And I select the following values from the 'Site Country' included dropdown filter: 
   | Argentina |
   Then the 'Site Country' included dropdown filter should contain the following filter tags:
   | Argentina |
   And I should see I am on the 'Open Queries by Age - Country' page
   And I can see the analytics has rendered

   Scenario: 12.1.1.14 : An 'Admin' user should be able to verify KPIs renders for "Open Queries by Age - Site" (Site Productivity FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Site Productivity' from the analytics list
    Then I should see I am on the 'Site Productivity' page
    When I navigate to the page containing the analytics named 'Open Queries by Age - Site'
    And I open the analytics named 'Open Queries by Age - Site'
    Then I should see I am on the 'Open Queries by Age - Site' page
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    When I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I should see 'Select filters to proceed.' in the report body
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
    When I select the following values from the 'Site Name' included dropdown filter: 
    | Center Pharmatech |
    Then the 'Site Name' included dropdown filter should contain the following filter tags:
    | Center Pharmatech |
    And I should see I am on the 'Open Queries by Age - Site' page
    And I can see the analytics has rendered
    
   Scenario: 12.1.1.15 : An 'Admin' user should be able to verify KPIs renders for "Open Queries by Age - Study" (Site Productivity FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Site Productivity' from the analytics list
    Then I should see I am on the 'Site Productivity' page
    And I navigate to the page containing the analytics named 'Open Queries by Age - Study'
    When I open the analytics named 'Open Queries by Age - Study'
    And I should see I am on the 'Open Queries by Age - Study' page
    Then I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I can see the analytics has rendered

  Scenario: 12.1.1.16 : An 'Admin' user should be able to verify KPIs renders for "Query Rate - Country" (Site Productivity FOLDER)
   When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
   And I switch to the 'CCDM' account if I am on another account   
   And I open a folder named 'Site Productivity' from the analytics list
   Then I should see I am on the 'Site Productivity' page
   And I navigate to the page containing the analytics named 'Query Rate - Country'
   When I navigate to the page containing the analytics named 'Query Rate - Country'
   And I open the analytics named 'Query Rate - Country'
   And I should see I am on the 'Query Rate - Country' page
   Then I should see 'Select filters to proceed.' in the report body
   When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
   And I select 'Beta 21' from the 'Study' session filter dropdown
   And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
   Then I can see the following study in the 'Study' session filter minimized view:
   | Beta 21 |
   When I open the 'Filters' panel
   And I select the following values from the 'Site Country' included dropdown filter: 
   | Argentina |
   Then the 'Site Country' included dropdown filter should contain the following filter tags:
   | Argentina |
   And I should see I am on the 'Query Rate - Country' page
   And I can see the analytics has rendered

   Scenario: 12.1.1.17 : An 'Admin' user should be able to verify KPIs renders for "Query Rate - Site" (Site Productivity FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Site Productivity' from the analytics list
    Then I should see I am on the 'Site Productivity' page
    When I navigate to the page containing the analytics named 'Query Rate - Site'
    And I open the analytics named 'Query Rate - Site'
    Then I should see I am on the 'Query Rate - Site' page
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    When I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I should see 'Select filters to proceed.' in the report body
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
    When I select the following values from the 'Site Name' included dropdown filter: 
    | Center Pharmatech |
    Then the 'Site Name' included dropdown filter should contain the following filter tags:
    | Center Pharmatech |
    And I should see I am on the 'Query Rate - Site' page
    And I can see the analytics has rendered
    
   Scenario: 12.1.1.18 : An 'Admin' user should be able to verify KPIs renders for "Query Rate - Study" (Site Productivity FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Site Productivity' from the analytics list
    Then I should see I am on the 'Site Productivity' page
    And I navigate to the page containing the analytics named 'Query Rate - Study'
    When I open the analytics named 'Query Rate - Study'
    And I should see I am on the 'Query Rate - Study' page
    Then I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I can see the analytics has rendered

  Scenario: 12.1.1.19 : An 'Admin' user should be able to verify KPIs renders for "Query Rate by eCRF - Country" (Site Productivity FOLDER)
   When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
   And I switch to the 'CCDM' account if I am on another account   
   And I open a folder named 'Site Productivity' from the analytics list
   Then I should see I am on the 'Site Productivity' page
   And I navigate to the page containing the analytics named 'Query Rate by eCRF - Country'
   When I navigate to the page containing the analytics named 'Query Rate by eCRF - Country'
   And I open the analytics named 'Query Rate by eCRF - Country'
   And I should see I am on the 'Query Rate by eCRF - Country' page
   Then I should see 'Select filters to proceed.' in the report body
   When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
   And I select 'Beta 21' from the 'Study' session filter dropdown
   And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
   Then I can see the following study in the 'Study' session filter minimized view:
   | Beta 21 |
   When I open the 'Filters' panel
   And I select the following values from the 'Site Country' included dropdown filter: 
   | Argentina |
   Then the 'Site Country' included dropdown filter should contain the following filter tags:
   | Argentina |
   And I should see I am on the 'Query Rate by eCRF - Country' page
   And I can see the analytics has rendered

   Scenario: 12.1.1.20 : An 'Admin' user should be able to verify KPIs renders for "Query Rate by eCRF - Site" (Site Productivity FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Site Productivity' from the analytics list
    Then I should see I am on the 'Site Productivity' page
    When I navigate to the page containing the analytics named 'Query Rate by eCRF - Site'
    And I open the analytics named 'Query Rate by eCRF - Site'
    Then I should see I am on the 'Query Rate by eCRF - Site' page
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    When I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I should see 'Select filters to proceed.' in the report body
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
    When I select the following values from the 'Site Name' included dropdown filter: 
    | Center Pharmatech |
    Then the 'Site Name' included dropdown filter should contain the following filter tags:
    | Center Pharmatech |
    And I should see I am on the 'Query Rate by eCRF - Site' page
    And I can see the analytics has rendered

   Scenario: 12.1.1.21 : An 'Admin' user should be able to verify KPIs renders for "Query Rate by eCRF - Study" (Site Productivity FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Site Productivity' from the analytics list
    Then I should see I am on the 'Site Productivity' page
    And I navigate to the page containing the analytics named 'Query Rate by eCRF - Study'
    When I open the analytics named 'Query Rate by eCRF - Study'
    And I should see I am on the 'Query Rate by eCRF - Study' page
    Then I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I can see the analytics has rendered

  Scenario: 12.1.1.22 : An 'Admin' user should be able to verify KPIs renders for "Query Resolution - Country" (Site Productivity FOLDER)
   When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
   And I switch to the 'CCDM' account if I am on another account   
   And I open a folder named 'Site Productivity' from the analytics list
   Then I should see I am on the 'Site Productivity' page
   And I navigate to the page containing the analytics named 'Query Resolution - Country'
   When I navigate to the page containing the analytics named 'Query Resolution - Country'
   And I open the analytics named 'Query Resolution - Country'
   And I should see I am on the 'Query Resolution - Country' page
   Then I should see 'Select filters to proceed.' in the report body
   When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
   And I select 'Beta 21' from the 'Study' session filter dropdown
   And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
   Then I can see the following study in the 'Study' session filter minimized view:
   | Beta 21 |
   When I open the 'Filters' panel
   And I select the following values from the 'Site Country' included dropdown filter: 
   | Argentina |
   Then the 'Site Country' included dropdown filter should contain the following filter tags:
   | Argentina |
   And I should see I am on the 'Query Resolution - Country' page
   And I can see the analytics has rendered


   Scenario: 12.1.1.23 : An 'Admin' user should be able to verify KPIs renders for "Query Resolution - Site" (Site Productivity FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Site Productivity' from the analytics list
    Then I should see I am on the 'Site Productivity' page
    When I navigate to the page containing the analytics named 'Query Resolution - Site'
    And I open the analytics named 'Query Resolution - Site'
    Then I should see I am on the 'Query Resolution - Site' page
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    When I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I should see 'Select filters to proceed.' in the report body
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
    When I select the following values from the 'Site Name' included dropdown filter: 
    | Center Pharmatech |
    Then the 'Site Name' included dropdown filter should contain the following filter tags:
    | Center Pharmatech |
    And I should see I am on the 'Query Resolution - Site' page
    And I can see the analytics has rendered
    

   Scenario: 12.1.1.24 : An 'Admin' user should be able to verify KPIs renders for "Query Resolution - Study" (Site Productivity FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Site Productivity' from the analytics list
    Then I should see I am on the 'Site Productivity' page
    And I navigate to the page containing the analytics named 'Query Resolution - Study'
    When I open the analytics named 'Query Resolution - Study'
    And I should see I am on the 'Query Resolution - Study' page
    Then I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I can see the analytics has rendered

#SUBJECT COMPLIENCE
  Scenario: 12.1.1.25 : An 'Admin' user should be able to verify KPIs renders for "AE Rate per Subject Days - Country" (Subject Compliance FOLDER)
   When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
   And I switch to the 'CCDM' account if I am on another account   
   And I open a folder named 'Subject Compliance' from the analytics list
   Then I should see I am on the 'Subject Compliance' page
   And I navigate to the page containing the analytics named 'AE Rate per Subject Days - Country'
   When I navigate to the page containing the analytics named 'AE Rate per Subject Days - Country'
   And I open the analytics named 'AE Rate per Subject Days - Country'
   And I should see I am on the 'AE Rate per Subject Days - Country' page
   Then I should see 'Select filters to proceed.' in the report body
   When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
   And I select 'Beta 21' from the 'Study' session filter dropdown
   And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
   Then I can see the following study in the 'Study' session filter minimized view:
   | Beta 21 |
   When I open the 'Filters' panel
   And I select the following values from the 'Site Country' included dropdown filter: 
   | Argentina |
   Then the 'Site Country' included dropdown filter should contain the following filter tags:
   | Argentina |
   And I should see I am on the 'AE Rate per Subject Days - Country' page
   And I can see the analytics has rendered

   Scenario: 12.1.1.26 : An 'Admin' user should be able to verify KPIs renders for "AE Rate per Subject Days - Site" (Subject Compliance FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Compliance' from the analytics list
    Then I should see I am on the 'Subject Compliance' page
    When I navigate to the page containing the analytics named 'AE Rate per Subject Days - Site'
    And I open the analytics named 'AE Rate per Subject Days - Site'
    Then I should see I am on the 'AE Rate per Subject Days - Site' page
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    When I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I should see 'Select filters to proceed.' in the report body
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
    When I select the following values from the 'Site Name' included dropdown filter: 
    | Mountain Novex Research Center Radiant |
    Then the 'Site Name' included dropdown filter should contain the following filter tags:
    | Mountain Novex Research Center Radiant |
    And I should see I am on the 'AE Rate per Subject Days - Site' page
    And I can see the analytics has rendered

   Scenario: 12.1.1.27 : An 'Admin' user should be able to verify KPIs renders for "AE Rate per Subject Days - Study" (Subject Compliance FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Compliance' from the analytics list
    Then I should see I am on the 'Subject Compliance' page
    And I navigate to the page containing the analytics named 'AE Rate per Subject Days - Study'
    When I open the analytics named 'AE Rate per Subject Days - Study'
    And I should see I am on the 'AE Rate per Subject Days - Study' page
    Then I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I can see the analytics has rendered

  Scenario: 12.1.1.28 : An 'Admin' user should be able to verify KPIs renders for "AE Terms by Relative Study Week - Country" (Subject Compliance FOLDER)
   When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
   And I switch to the 'CCDM' account if I am on another account   
   And I open a folder named 'Subject Compliance' from the analytics list
   Then I should see I am on the 'Subject Compliance' page
   And I navigate to the page containing the analytics named 'AE Terms by Relative Study Week - Country'
   When I navigate to the page containing the analytics named 'AE Terms by Relative Study Week - Country'
   And I open the analytics named 'AE Terms by Relative Study Week - Country'
   And I should see I am on the 'AE Terms by Relative Study Week - Country' page
   Then I should see 'Select filters to proceed.' in the report body
   When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
   And I select 'Beta 21' from the 'Study' session filter dropdown
   And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
   Then I can see the following study in the 'Study' session filter minimized view:
   | Beta 21 |
   When I open the 'Filters' panel
   And I select the following values from the 'Site Country' included dropdown filter: 
   | Argentina |
   Then the 'Site Country' included dropdown filter should contain the following filter tags:
   | Argentina |
   And I should see I am on the 'AE Terms by Relative Study Week - Country' page
   And I can see the analytics has rendered

   Scenario: 12.1.1.29 : An 'Admin' user should be able to verify KPIs renders for "AE Terms by Relative Study Week - Site" (Subject Compliance FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Compliance' from the analytics list
    Then I should see I am on the 'Subject Compliance' page
    When I navigate to the page containing the analytics named 'AE Terms by Relative Study Week - Site'
    And I open the analytics named 'AE Terms by Relative Study Week - Site'
    Then I should see I am on the 'AE Terms by Relative Study Week - Site' page
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    When I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I should see 'Select filters to proceed.' in the report body
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
    When I select the following values from the 'Site Name' included dropdown filter: 
    | Mountain Novex Research Center Radiant |
    Then the 'Site Name' included dropdown filter should contain the following filter tags:
    | Mountain Novex Research Center Radiant |
    And I should see I am on the 'AE Terms by Relative Study Week - Site' page
    And I can see the analytics has rendered

   Scenario: 12.1.1.30 : An 'Admin' user should be able to verify KPIs renders for "AE Terms by Relative Study Week - Study" (Site Productivity FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Compliance' from the analytics list
    Then I should see I am on the 'Subject Compliance' page
    And I navigate to the page containing the analytics named 'AE Terms by Relative Study Week - Study'
    When I open the analytics named 'AE Terms by Relative Study Week - Study'
    And I should see I am on the 'AE Terms by Relative Study Week - Study' page
    #Then I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I can see the analytics has rendered

  Scenario: 12.1.1.31 : An 'Admin' user should be able to verify KPIs renders for "AEs Against Study Baseline - Country" (Subject Compliance FOLDER)
   When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
   And I switch to the 'CCDM' account if I am on another account   
   And I open a folder named 'Subject Compliance' from the analytics list
   Then I should see I am on the 'Subject Compliance' page
   And I navigate to the page containing the analytics named 'AEs Against Study Baseline - Country'
   When I navigate to the page containing the analytics named 'AEs Against Study Baseline - Country'
   And I open the analytics named 'AEs Against Study Baseline - Country'
   And I should see I am on the 'AEs Against Study Baseline - Country' page
   And I can see the analytics has rendered
   When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
   And I select 'Beta 21' from the 'Study' session filter dropdown
   And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
   Then I can see the following study in the 'Study' session filter minimized view:
   | Beta 21 |
   When I open the 'Filters' panel
   And I select the following values from the 'Site Country' included dropdown filter: 
   | Argentina |
   Then the 'Site Country' included dropdown filter should contain the following filter tags:
   | Argentina |
   And I should see I am on the 'AEs Against Study Baseline - Country' page
   And I can see the analytics has rendered

   Scenario: 12.1.1.32 : An 'Admin' user should be able to verify KPIs renders for "AEs Against Study Baseline - Site" (Site Productivity FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Compliance' from the analytics list
    Then I should see I am on the 'Subject Compliance' page
    When I navigate to the page containing the analytics named 'AEs Against Study Baseline - Site'
    And I open the analytics named 'AEs Against Study Baseline - Site'
    Then I should see I am on the 'AEs Against Study Baseline - Site' page
    Then I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    When I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
    When I select the following values from the 'Site Name' included dropdown filter: 
    | Mountain Novex Research Center Radiant |
    Then the 'Site Name' included dropdown filter should contain the following filter tags:
    | Mountain Novex Research Center Radiant |
    And I should see I am on the 'AEs Against Study Baseline - Site' page
    And I can see the analytics has rendered

   Scenario: 12.1.1.33 : An 'Admin' user should be able to verify KPIs renders for "AEs Against Study Baseline - Study" (Subject Compliance FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Compliance' from the analytics list
    Then I should see I am on the 'Subject Compliance' page
    And I navigate to the page containing the analytics named 'AEs Against Study Baseline - Study'
    When I open the analytics named 'AEs Against Study Baseline - Study'
    And I should see I am on the 'AEs Against Study Baseline - Study' page
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I can see the analytics has rendered

  Scenario: 12.1.1.34 : An 'Admin' user should be able to verify KPIs renders for  "Primary Endpoint Data Entry Rate - Country" (Subject Compliance FOLDER)
   When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
   And I switch to the 'CCDM' account if I am on another account   
   And I open a folder named 'Subject Compliance' from the analytics list
   Then I should see I am on the 'Subject Compliance' page
   And I navigate to the page containing the analytics named 'Primary Endpoint Data Entry Rate - Country'
   When I navigate to the page containing the analytics named 'Primary Endpoint Data Entry Rate - Country'
   And I open the analytics named 'Primary Endpoint Data Entry Rate - Country'
   And I should see I am on the 'Primary Endpoint Data Entry Rate - Country' page
   Then I should see 'Select filters to proceed.' in the report body
   When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
   And I select 'Beta 21' from the 'Study' session filter dropdown
   And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
   Then I can see the following study in the 'Study' session filter minimized view:
   | Beta 21 |
   When I open the 'Filters' panel
   And I select the following values from the 'Site Country' included dropdown filter: 
   | Argentina |
   Then the 'Site Country' included dropdown filter should contain the following filter tags:
   | Argentina |
   And I should see I am on the 'Primary Endpoint Data Entry Rate - Country' page
   And I can see the analytics has rendered
   

   Scenario: 12.1.1.35 : An 'Admin' user should be able to verify KPIs renders for "Primary Endpoint Data Entry Rate - Site" (Subject Compliance FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Compliance' from the analytics list
    Then I should see I am on the 'Subject Compliance' page
    When I navigate to the page containing the analytics named 'Primary Endpoint Data Entry Rate - Site'
    And I open the analytics named 'Primary Endpoint Data Entry Rate - Site'
    Then I should see I am on the 'Primary Endpoint Data Entry Rate - Site' page
    Then I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    When I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
    When I select the following values from the 'Site Name' included dropdown filter: 
    | Mountain Novex Research Center Radiant |
    Then the 'Site Name' included dropdown filter should contain the following filter tags:
    | Mountain Novex Research Center Radiant |
    And I should see I am on the 'Primary Endpoint Data Entry Rate - Site' page
    And I can see the analytics has rendered

   Scenario: 12.1.1.36 : An 'Admin' user should be able to verify KPIs renders for "Primary Endpoint Data Entry Rate - Study" (Subject Compliance FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Compliance' from the analytics list
    Then I should see I am on the 'Subject Compliance' page
    And I navigate to the page containing the analytics named 'Primary Endpoint Data Entry Rate - Study'
    When I open the analytics named 'Primary Endpoint Data Entry Rate - Study'
    And I should see I am on the 'Primary Endpoint Data Entry Rate - Study' page
    Then I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I can see the analytics has rendered

  Scenario: 12.1.1.37 : An 'Admin' user should be able to verify KPIs renders for "Subject Count by Latest Scheduled Visit - Country" (Subject Compliance FOLDER)
   When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
   And I switch to the 'CCDM' account if I am on another account   
   And I open a folder named 'Subject Compliance' from the analytics list
   Then I should see I am on the 'Subject Compliance' page
   And I navigate to the page containing the analytics named 'Subject Count by Latest Scheduled Visit - Country'
   When I navigate to the page containing the analytics named 'Subject Count by Latest Scheduled Visit - Country'
   And I open the analytics named 'Subject Count by Latest Scheduled Visit - Country'
   And I should see I am on the 'Subject Count by Latest Scheduled Visit - Country' page
   Then I should see 'Select filters to proceed.' in the report body
   When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
   And I select 'Beta 21' from the 'Study' session filter dropdown
   And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
   Then I can see the following study in the 'Study' session filter minimized view:
   | Beta 21 |
   When I open the 'Filters' panel
   And I select the following values from the 'Site Country' included dropdown filter: 
   | Argentina |
   Then the 'Site Country' included dropdown filter should contain the following filter tags:
   | Argentina |
   And I should see I am on the 'Subject Count by Latest Scheduled Visit - Country' page
   And I can see the analytics has rendered

   Scenario: 12.1.1.38 : An 'Admin' user should be able to verify KPIs renders for "Subject Count by Latest Scheduled Visit - Site" (Subject Compliance FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Compliance' from the analytics list
    Then I should see I am on the 'Subject Compliance' page
    When I navigate to the page containing the analytics named 'Subject Count by Latest Scheduled Visit - Site'
    And I open the analytics named 'Subject Count by Latest Scheduled Visit - Site'
    Then I should see I am on the 'Subject Count by Latest Scheduled Visit - Site' page
    Then I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    When I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
    When I select the following values from the 'Site Name' included dropdown filter: 
    | Mountain Novex Research Center Radiant |
    Then the 'Site Name' included dropdown filter should contain the following filter tags:
    | Mountain Novex Research Center Radiant |
    And I should see I am on the 'Subject Count by Latest Scheduled Visit - Site' page
    And I can see the analytics has rendered

   Scenario: 12.1.1.39 : An 'Admin' user should be able to verify KPIs renders for "Subject Count by Latest Scheduled Visit - Study" (Subject Compliance FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Compliance' from the analytics list
    Then I should see I am on the 'Subject Compliance' page
    And I navigate to the page containing the analytics named 'Subject Count by Latest Scheduled Visit - Study'
    When I open the analytics named 'Subject Count by Latest Scheduled Visit - Study'
    And I should see I am on the 'Subject Count by Latest Scheduled Visit - Study' page
    Then I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I can see the analytics has rendered

  Scenario: 12.1.1.40 : An 'Admin' user should be able to verify KPIs renders for Protocol_Deviations_Rate - Country (Subject Compliance FOLDER)
   When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
   And I switch to the 'CCDM' account if I am on another account   
   And I open a folder named 'Subject Compliance' from the analytics list
   Then I should see I am on the 'Subject Compliance' page
   And I navigate to the page containing the analytics named 'Protocol Deviations Rate - Country'
   When I navigate to the page containing the analytics named 'Protocol Deviations Rate - Country'
   And I open the analytics named 'Protocol Deviations Rate - Country'
   And I should see I am on the 'Protocol Deviations Rate - Countr' page
   Then I should see 'Select filters to proceed.' in the report body
   When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
   And I select 'Beta 21' from the 'Study' session filter dropdown
   And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
   Then I can see the following study in the 'Study' session filter minimized view:
   | Beta 21 |
   When I open the 'Filters' panel
   And I select the following values from the 'Site Country' included dropdown filter: 
   | China |
   Then the 'Site Country' included dropdown filter should contain the following filter tags:
   | China |
   And I should see I am on the 'Protocol Deviations Rate - Country' page
   And I can see the analytics has rendered

   Scenario: 12.1.1.41 : An 'Admin' user should be able to verify KPIs renders for Protocol_Deviations_Rate - Site (Subject Compliance FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Compliance' from the analytics list
    Then I should see I am on the 'Subject Compliance' page
    When I navigate to the page containing the analytics named 'Protocol Deviations Rate - Site'
    And I open the analytics named 'Protocol Deviations Rate - Site'
    Then I should see I am on the 'Protocol Deviations Rate - Site' page
    Then I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    When I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | China |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | China |
    When I select the following values from the 'Site Name' included dropdown filter: 
    | Clinical Swedish |
    Then the 'Site Name' included dropdown filter should contain the following filter tags:
    | Clinical Swedish |
    And I should see I am on the 'Protocol Deviations Rate - Site' page
    And I can see the analytics has rendered

   Scenario: 12.1.1.42 : An 'Admin' user should be able to verify KPIs renders for Protocol_Deviations_Rate - Study (Subject Compliance FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Compliance' from the analytics list
    Then I should see I am on the 'Subject Compliance' page
    And I navigate to the page containing the analytics named 'Protocol Deviations Rate - Study'
    When I open the analytics named 'Protocol Deviations Rate - Study'
    And I should see I am on the 'Protocol Deviations Rate - Study' page
    Then I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I can see the analytics has rendered

  Scenario: 12.1.1.43 : An 'Admin' user should be able to verify KPIs renders for Subject_Count_by_Latest_Scheduled_Visit - Country (Subject Compliance FOLDER)
   When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
   And I switch to the 'CCDM' account if I am on another account   
   And I open a folder named 'Subject Compliance' from the analytics list
   Then I should see I am on the 'Subject Compliance' page
   And I navigate to the page containing the analytics named 'Subject Count by Latest Scheduled Visit - Country'
   When I navigate to the page containing the analytics named 'Subject Count by Latest Scheduled Visit - Country'
   And I open the analytics named 'Subject Count by Latest Scheduled Visit - Country'
   And I should see I am on the 'Subject Count by Latest Scheduled Visit - Country' page
   Then I should see 'Select filters to proceed.' in the report body
   When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
   And I select 'Beta 21' from the 'Study' session filter dropdown
   And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
   Then I can see the following study in the 'Study' session filter minimized view:
   | Beta 21 |
   When I open the 'Filters' panel
   And I select the following values from the 'Site Country' included dropdown filter: 
   | China |
   Then the 'Site Country' included dropdown filter should contain the following filter tags:
   | China |
   And I should see I am on the 'Subject Count by Latest Scheduled Visit - Country' page
   And I can see the analytics has rendered

   Scenario: 12.1.1.44 : An 'Admin' user should be able to verify KPIs renders for Subject_Count_by_Latest_Scheduled_Visit - Site (Subject Compliance FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Compliance' from the analytics list
    Then I should see I am on the 'Subject Compliance' page
    When I navigate to the page containing the analytics named 'Subject Count by Latest Scheduled Visit - Site'
    And I open the analytics named 'Subject Count by Latest Scheduled Visit - Site'
    Then I should see I am on the 'Subject Count by Latest Scheduled Visit - Site' page
    Then I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    When I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
    When I select the following values from the 'Site Name' included dropdown filter: 
    | Mountain Novex Research Center Radiant |
    Then the 'Site Name' included dropdown filter should contain the following filter tags:
    | Mountain Novex Research Center Radiant |
    And I should see I am on the 'Subject Count by Latest Scheduled Visit - Site' page
    And I can see the analytics has rendered

   Scenario: 12.1.1.45 : An 'Admin' user should be able to verify KPIs renders for Subject_Count_by_Latest_Scheduled_Visit - Study (Subject Compliance FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Compliance' from the analytics list
    Then I should see I am on the 'Subject Compliance' page
    And I navigate to the page containing the analytics named 'Subject Count by Latest Scheduled Visit - Study'
    When I open the analytics named 'Subject Count by Latest Scheduled Visit - Study'
    And I should see I am on the 'Subject Count by Latest Scheduled Visit - Study' page
    Then I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I can see the analytics has rendered

  Scenario: 12.1.1.46 : An 'Admin' user should be able to verify KPIs renders for Subject_Visit_Compliance_with_Schedule - Country (Subject Compliance FOLDER)
   When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
   And I switch to the 'CCDM' account if I am on another account   
   And I open a folder named 'Subject Compliance' from the analytics list
   Then I should see I am on the 'Subject Compliance' page
   And I navigate to the page containing the analytics named 'Subject Visit Compliance with Schedule - Country'
   When I navigate to the page containing the analytics named 'Subject Visit Compliance with Schedule - Country'
   And I open the analytics named 'Subject Visit Compliance with Schedule - Country'
   And I should see I am on the 'Subject Visit Compliance with Schedule - Country' page
   Then I should see 'Select filters to proceed.' in the report body
   When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
   And I select 'Beta 21' from the 'Study' session filter dropdown
   And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
   Then I can see the following study in the 'Study' session filter minimized view:
   | Beta 21 |
   When I open the 'Filters' panel
   And I select the following values from the 'Site Country' included dropdown filter: 
   | China |
   Then the 'Site Country' included dropdown filter should contain the following filter tags:
   | China |
   And I should see I am on the 'Subject Visit Compliance with Schedule - Country' page
   And I can see the analytics has rendered

   Scenario: 12.1.1.47 : An 'Admin' user should be able to verify KPIs renders for Subject_Visit_Compliance_with_Schedule - Site (Subject Compliance FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Compliance' from the analytics list
    Then I should see I am on the 'Subject Compliance' page
    When I navigate to the page containing the analytics named 'Subject Visit Compliance with Schedule - Site'
    And I open the analytics named 'Subject Visit Compliance with Schedule - Site'
    Then I should see I am on the 'Subject Visit Compliance with Schedule - Site' page
    Then I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    When I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
    When I select the following values from the 'Site Name' included dropdown filter: 
    | Mountain Novex Research Center Radiant |
    Then the 'Site Name' included dropdown filter should contain the following filter tags:
    | Mountain Novex Research Center Radiant |
    And I should see I am on the 'Subject Visit Compliance with Schedule - Site' page
    And I can see the analytics has rendered

   Scenario: 12.1.1.48 : An 'Admin' user should be able to verify KPIs renders for Subject_Visit_Compliance_with_Schedule - Study (Subject Compliance FOLDER)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Compliance' from the analytics list
    Then I should see I am on the 'Subject Compliance' page
    And I navigate to the page containing the analytics named 'Subject Visit Compliance with Schedule - Study'
    When I open the analytics named 'Subject Visit Compliance with Schedule - Study'
    And I should see I am on the 'Subject Visit Compliance with Schedule - Study' page
    Then I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I can see the analytics has rendered

  Scenario: 12.1.1.49 : An 'Admin' user should be able to verify KPI renders for "Consent Rate – Country" (Subject Enrollment FOLDER)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account   
    When I open a folder named 'Subject Enrollment' from the analytics list
    Then I should see I am on the 'Subject Enrollment' page
    And I open the analytics named 'Consent Rate - Country'
    Then I should see I am on the 'Consent Rate - Country' page
    And I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
     When I toggle the 'Consented' legend from the current graphical analytics
    Then I should see the 'Consented' legend as visible from the current graphical analytics
    Then I should see I am on the 'Consent Rate - Country' page
    And I can see the analytics has rendered

  Scenario: 12.1.1.50 : An 'Admin' user should be able to verify KPIs renders for "Consent Rate - Site" (Subject Enrollment FOLDER)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Enrollment' from the analytics list
    Then I should see I am on the 'Subject Enrollment' page
    When I navigate to the page containing the analytics named 'Consent Rate - Site'
    And I open the analytics named 'Consent Rate - Site'
    Then I should see I am on the 'Consent Rate - Site' page
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I should see 'Select filters to proceed.' in the report body
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
    When I select the following values from the 'Site Name' included dropdown filter: 
    | Center Pharmatech |
    Then the 'Site Name' included dropdown filter should contain the following filter tags:
    | Center Pharmatech |
    And I should see I am on the 'Consent Rate - Site' page
    And I can see the analytics has rendered
    And I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I remove 'Beta 21' from the 'Study' session filter dropdown

  Scenario: 12.1.1.51 : An 'Admin' user should be able to verify KPIs renders for "Consent Rate – Study" (Subject Enrollment FOLDER)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Enrollment' from the analytics list
    And I open the analytics named 'Consent Rate - Site'
    Then I should see I am on the 'Consent Rate - Site' page
    And I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
    When I select the following values from the 'Site Name' included dropdown filter: 
    | Center Pharmatech |
    Then the 'Site Name' included dropdown filter should contain the following filter tags:
    | Center Pharmatech |
    And I should see I am on the 'Consent Rate - Site' page
    When I toggle the 'Consented' legend from the current graphical analytics
    Then I should see the 'Consented' legend as visible from the current graphical analytics
    And I can see the analytics has rendered

  Scenario: 12.1.1.52 : An 'Admin' user should be able to verify KPIs renders for "Current Subject Disposition - Country" (Subject Enrollment FOLDER)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account   
    When I open a folder named 'Subject Enrollment' from the analytics list
    Then I should see I am on the 'Subject Enrollment' page
    And I open the analytics named 'Current Subject Disposition - Country'
    Then I should see I am on the 'Current Subject Disposition - Country' page
    And I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |

    #Breakes here:
    When I toggle the 'Consented' legend from the current graphical analytics
    Then I should see the 'Consented' legend as visible from the current graphical analytics
    Then I should see I am on the 'Current Subject Disposition - Country' page
    And I can see the analytics has rendered

  Scenario: 12.1.1.53 : An 'Admin' user should be able to verify KPIs renders for "Current Subject Disposition – Site" (Subject Enrollment FOLDER)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Enrollment' from the analytics list
    Then I should see I am on the 'Subject Enrollment' page
    When I navigate to the page containing the analytics named 'Current Subject Disposition - Site'
    And I open the analytics named 'Current Subject Disposition - Site'
    Then I should see I am on the 'Current Subject Disposition - Site' page
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I should see 'Select filters to proceed.' in the report body
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
    When I select the following values from the 'Site Name' included dropdown filter: 
    | Center Pharmatech |
    Then the 'Site Name' included dropdown filter should contain the following filter tags:
    | Center Pharmatech |
    And I should see I am on the 'Current Subject Disposition - Site' page
    And I can see the analytics has rendered
    And I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I remove 'Beta 21' from the 'Study' session filter dropdown

  Scenario: 12.1.1.54 : An 'Admin' user should be able to verify KPIs renders for "Current Subject Disposition - Study" (Subject Enrollment FOLDER)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Enrollment' from the analytics list
    And I open the analytics named 'Current Subject Disposition - Study'
    Then I should see I am on the 'Current Subject Disposition - Study' page
    And I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I should see I am on the 'Current Subject Disposition - Study' page
    And I can see the analytics has rendered

  Scenario: 12.1.1.55 : An 'Admin' user should be able to verify KPIs renders for "Randomization Failures by Reason – Country" (Subject Enrollment FOLDER)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account   
    When I open a folder named 'Subject Enrollment' from the analytics list
    Then I should see I am on the 'Subject Enrollment' page
    And I open the analytics named 'Randomization Failures by Reason - Country'
    Then I should see I am on the 'Randomization Failures by Reason - Country' page
    And I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
    When I toggle the 'Randomized' legend from the current graphical analytics
    Then I should see the 'Randomized' legend as visible from the current graphical analytics
    Then I should see I am on the 'Randomization Failures by Reason - Country' page
    And I can see the analytics has rendered

  Scenario: 12.1.1.56 : An 'Admin' user should be able to verify KPIs renders for "Randomization Failures by Reason - Site" (Subject Enrollment FOLDER)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Enrollment' from the analytics list
    Then I should see I am on the 'Subject Enrollment' page
    When I navigate to the page containing the analytics named 'Randomization Failures by Reason - Site'
    And I open the analytics named 'Randomization Failures by Reason - Site'
    Then I should see I am on the 'Randomization Failures by Reason - Site' page
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I should see 'Select filters to proceed.' in the report body
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
    When I select the following values from the 'Site Name' included dropdown filter: 
    | Center Pharmatech |
    Then the 'Site Name' included dropdown filter should contain the following filter tags:
    | Center Pharmatech |
    When I toggle the 'Randomized' legend from the current graphical analytics
    Then I should see the 'Randomized' legend as visible from the current graphical analytics
    And I should see I am on the 'Randomization Failures by Reason - Site' page
    And I can see the analytics has rendered
    And I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I remove 'Beta 21' from the 'Study' session filter dropdown

  Scenario: 12.1.1.57 : An 'Admin' user should be able to verify KPIs renders for "Randomization Failures by Reason - Study" (Subject Enrollment FOLDER)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Enrollment' from the analytics list
    And I open the analytics named 'Randomization Failures by Reason - Study'
    Then I should see I am on the 'Randomization Failures by Reason - Study' page
    And I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I should see I am on the 'Randomization Failures by Reason - Study' page
    And I can see the analytics has rendered

  Scenario: 12.1.1.58 : An 'Admin' user should be able to verify KPIs renders for "Screen Failures by Reason – Country" (Subject Enrollment FOLDER)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45' 
    When I switch to the 'CCDM' account if I am on another account   
    When I open a folder named 'Subject Enrollment' from the analytics list
    Then I should see I am on the 'Subject Enrollment' page
    And I open the analytics named 'Screen Failures by Reason - Country'
    Then I should see I am on the 'Screen Failures by Reason - Country' page
    And I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
    When I toggle the 'Enrolled' legend from the current graphical analytics
    Then I should see the 'Enrolled' legend as visible from the current graphical analytics
    Then I should see I am on the 'Screen Failures by Reason - Country' page
    And I can see the analytics has rendered

  Scenario: 12.1.1.59 : An 'Admin' user should be able to verify KPIs renders for "Screen Failures by Reason - Site" (Subject Enrollment FOLDER)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Enrollment' from the analytics list
    Then I should see I am on the 'Subject Enrollment' page
    When I navigate to the page containing the analytics named 'Randomization Failures by Reason - Site'
    And I open the analytics named 'Screen Failures by Reason - Site'
    Then I should see I am on the 'Screen Failures by Reason - Site' page
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I should see 'Select filters to proceed.' in the report body
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
    When I select the following values from the 'Site Name' included dropdown filter: 
    | Center Pharmatech |
    Then the 'Site Name' included dropdown filter should contain the following filter tags:
    | Center Pharmatech |
    When I toggle the 'Enrolled' legend from the current graphical analytics
    Then I should see the 'Enrolled' legend as visible from the current graphical analytics
    And I should see I am on the 'Screen Failures by Reason - Site' page
    And I can see the analytics has rendered
    And I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I remove 'Beta 21' from the 'Study' session filter dropdown

  Scenario: 12.1.1.60 : An 'Admin' user should be able to verify KPIs renders for "Screen Failures by Reason - Study" (Subject Enrollment FOLDER)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Enrollment' from the analytics list
    And I open the analytics named 'Screen Failures by Reason - Study'
    Then I should see I am on the 'Screen Failures by Reason - Study' page
    And I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I should see I am on the 'Screen Failures by Reason - Study' page
    And I can see the analytics has rendered

  Scenario: 12.1.1.61 : An 'Admin' user should be able to verify KPIs renders for "Site Activation – Country" (Subject Enrollment FOLDER)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45' 
    When I switch to the 'CCDM' account if I am on another account   
    When I open a folder named 'Subject Enrollment' from the analytics list
    Then I should see I am on the 'Subject Enrollment' page
    And I open the analytics named 'Site Activation - Country'
    Then I should see I am on the 'Site Activation - Country' page
    And I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
    Then I should see I am on the 'Site Activation - Country' page
    And I can see the analytics has rendered

  Scenario: 12.1.1.62 : An 'Admin' user should be able to verify KPIs renders for "Site Activation – Study" (Subject Enrollment FOLDER)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Enrollment' from the analytics list
    And I open the analytics named 'Site Activation - Study'
    Then I should see I am on the 'Site Activation - Study' page
    And I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I should see I am on the 'Site Activation - Study' page
    And I can see the analytics has rendered

  Scenario: 12.1.1.63 : An 'Admin' user should be able to verify KPIs renders for "Subject Enrollment Funnel - Study" (Subject Enrollment FOLDER)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Enrollment' from the analytics list
    And I open the analytics named 'Subject Enrollment Funnel - Study'
    Then I should see I am on the 'Subject Enrollment Funnel - Study' page
    And I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I should see I am on the 'Subject Enrollment Funnel - Study' page
    And I can see the analytics has rendered

  Scenario: 12.1.1.64 : An 'Admin' user should be able to verify KPIs renders for "Subject Enrollment Rate – Country" (Subject Enrollment FOLDER)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45' 
    When I switch to the 'CCDM' account if I am on another account   
    When I open a folder named 'Subject Enrollment' from the analytics list
    Then I should see I am on the 'Subject Enrollment' page
    And I navigate to the page containing the analytics named 'Subject Enrollment Rate - Country'
    And I open the analytics named 'Subject Enrollment Rate - Country'
    Then I should see I am on the 'Subject Enrollment Rate - Country' page
    And I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
    Then I should see I am on the 'Subject Enrollment Rate - Country' page
    And I can see the analytics has rendered

  Scenario: 12.1.1.65 : An 'Admin' user should be able to verify KPIs renders for "Subject Enrollment Rate – Site" (Subject Enrollment FOLDER)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Enrollment' from the analytics list
    Then I should see I am on the 'Subject Enrollment' page
    When I navigate to the page containing the analytics named 'Subject Enrollment Rate - Site'
    And I open the analytics named 'Subject Enrollment Rate - Site'
    Then I should see I am on the 'Subject Enrollment Rate - Site' page
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I should see 'Select filters to proceed.' in the report body
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
    When I select the following values from the 'Site Name' included dropdown filter: 
    | Center Pharmatech |
    Then the 'Site Name' included dropdown filter should contain the following filter tags:
    | Center Pharmatech |
    And I should see I am on the 'Subject Enrollment Rate - Site' page
    And I can see the analytics has rendered
    And I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I remove 'Beta 21' from the 'Study' session filter dropdown

  Scenario: 12.1.1.66 : An 'Admin' user should be able to verify KPIs renders for "Subject Enrollment Rate – Study" (Subject Enrollment FOLDER)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Enrollment' from the analytics list
    And I navigate to the page containing the analytics named 'Subject Enrollment Rate - Site'
    And I open the analytics named 'Subject Enrollment Rate - Study'
    Then I should see I am on the 'Subject Enrollment Rate - Study' page
    And I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I should see I am on the 'Subject Enrollment Rate - Study' page
    And I can see the analytics has rendered

  Scenario: 12.1.1.67 : An 'Admin' user should be able to verifyKPIs renders for "Subject Evaluable – Country" (Subject Enrollment FOLDER)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45' 
    When I switch to the 'CCDM' account if I am on another account   
    When I open a folder named 'Subject Enrollment' from the analytics list
    Then I should see I am on the 'Subject Enrollment' page
    And I navigate to the page containing the analytics named 'Subject Evaluable - Country'
    And I open the analytics named 'Subject Evaluable - Country'
    Then I should see I am on the 'Subject Evaluable - Country' page
    And I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
    Then I should see I am on the 'Subject Evaluable - Country' page
    And I can see the analytics has rendered

  Scenario: 12.1.1.68 : An 'Admin' user should be able to verify KPIs renders for "Subject Evaluable – Site" (Subject Enrollment FOLDER)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Enrollment' from the analytics list
    Then I should see I am on the 'Subject Enrollment' page
    When I navigate to the page containing the analytics named 'Subject Evaluable - Site'
    And I open the analytics named 'Subject Evaluable - Site'
    Then I should see I am on the 'Subject Evaluable - Site' page
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I should see 'Select filters to proceed.' in the report body
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
    When I select the following values from the 'Site Name' included dropdown filter: 
    | Found Innovation Baptist Rex Research |
    Then the 'Site Name' included dropdown filter should contain the following filter tags:
    | Found Innovation Baptist Rex Research |
    And I should see I am on the 'Subject Evaluable - Site' page
    And I can see the analytics has rendered
    And I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I remove 'Beta 21' from the 'Study' session filter dropdown

  Scenario: 12.1.1.69 : An 'Admin' user should be able to verify KPIs renders for "Subject Evaluable – Study" (Subject Enrollment FOLDER)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Enrollment' from the analytics list
    And I navigate to the page containing the analytics named 'Subject Evaluable - Site'
    And I open the analytics named 'Subject Evaluable - Study'
    Then I should see I am on the 'Subject Evaluable - Study' page
    And I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I should see I am on the 'Subject Evaluable - Study' page
    And I can see the analytics has rendered

  Scenario: 12.1.1.70 : An 'Admin' user should be able to verify KPIs renders for "Subject Withdrawal – Country" (Subject Enrollment FOLDER)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45' 
    When I switch to the 'CCDM' account if I am on another account   
    When I open a folder named 'Subject Enrollment' from the analytics list
    Then I should see I am on the 'Subject Enrollment' page
    And I navigate to the page containing the analytics named 'Subject Withdrawal - Country'
    And I open the analytics named 'Subject Withdrawal - Country'
    Then I should see I am on the 'Subject Withdrawal - Country' page
    And I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
    When I toggle the 'Completed' legend from the current graphical analytics
    Then I should see the 'Completed' legend as visible from the current graphical analytics
    Then I should see I am on the 'Subject Withdrawal - Country' page
    And I can see the analytics has rendered

  Scenario: 12.1.1.71 : An 'Admin' user should be able to verify KPIs renders for "Subject Withdrawal – Site" (Subject Enrollment FOLDER)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Enrollment' from the analytics list
    Then I should see I am on the 'Subject Enrollment' page
    When I navigate to the page containing the analytics named 'Subject Withdrawal - Site'
    And I open the analytics named 'Subject Withdrawal - Site'
    Then I should see I am on the 'Subject Withdrawal - Site' page
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' session filter minimized view:
    | Beta 21 |
    And I should see 'Select filters to proceed.' in the report body
    When I open the 'Filters' panel
    And I select the following values from the 'Site Country' included dropdown filter: 
    | Argentina |
    Then the 'Site Country' included dropdown filter should contain the following filter tags:
    | Argentina |
    When I select the following values from the 'Site Name' included dropdown filter: 
    | Found Innovation Baptist Rex Research |
    Then the 'Site Name' included dropdown filter should contain the following filter tags:
    | Found Innovation Baptist Rex Research |
    When I toggle the 'Completed' legend from the current graphical analytics
    Then I should see the 'Completed' legend as visible from the current graphical analytics
    And I should see I am on the 'Subject Withdrawal - Site' page
    And I can see the analytics has rendered
    And I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I remove 'Beta 21' from the 'Study' session filter dropdown

  Scenario: 12.1.1.72 : An 'Admin' user should be able to verify KPIs renders for "Subject Withdrawal – Study" (Subject Enrollment FOLDER)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Enrollment' from the analytics list
    And I navigate to the page containing the analytics named 'Subject Withdrawal - Site'
    And I open the analytics named 'Subject Withdrawal - Study'
    Then I should see I am on the 'Subject Withdrawal - Study' page
    And I should see 'Select filters to proceed.' in the report body
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    Then I can see the following study in the 'Study' sessfilter minimized view:
    | Beta 21 |
    And I should see I am on the 'Subject Withdrawal - Study' page
    And I can see the analytics has rendered



    # DEMO FLOW:

     Scenario: 12.1.1.169 : Automated test from Demo Flow Part 2 (Breakes)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account
    When I navigate to the 'Analytics' page
    And I open a folder named 'Subject Enrollment' from the analytics list
    Then I should see I am on the 'Subject Enrollment' page
    And I navigate to the page containing the analytics named 'Subject Enrollment Funnel - Study'
    And I open the analytics named 'Subject Enrollment Funnel - Study'
    Then I should see I am on the 'Subject Enrollment Funnel - Study' page
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    And I can see the analytics has rendered
    #When I select the '1st' data point (China) from the current 'bubble chart' graphical analytics
    And I select the '1st' data point (Pre-Screened: 595 Subjects) from the current 'bar chart' graphical analytics
    And I click 'Randomization Failures by Reason - Study' in the Drilldown tooltip
    Then I should see I am on the 'Randomization Failures by Reason - Study' page
    And I can see the analytics has rendered

    #Brakes on following step:
    Then I can select the '1st' data point (Randomized) from the current 'pie chart' graphical analytics
    And I click 'Subject Disposition - Listing' in the Drilldown tooltip
    When I should see I am on the 'Subject Disposition - Listing' page
  

    When I sort the 'Study Name' column of the analytics list
    Then I can see the analytics list is sorted by column 'Study Name' in ascending order
    When I sort the 'Title' column of the favorites list again
    Then I can see the favorites list is sorted by column 'Title' in descending order
    When I sort the 'Created' column of the favorites list
    Then I can see the favorites list is sorted by column 'Created' in ascending order
    When I sort the 'Created' column of the favorites list again
    Then I can see the favorites list is sorted by column 'Created' in descending order
    When I sort the 'Type' column of the favorites list
    Then I can see the favorites list is sorted by column 'Type' in ascending order
    When I sort the 'Type' column of the favorites list again
    Then I can see the favorites list is sorted by column 'Type' in descending order
    And I log out

    #Brakes on following step:
    Then I can see the Subject Enrollment list is not sorted by column 'Site Name'
    When I sort the 'Site Name' column of the tasks list
    Then I can see the tasks list is sorted by column 'Site Name' in ascending order
    When I sort the 'Site name' column of the tasks list again
    Then I can see the tasks list is sorted by column 'Site Name' in descending order
    And I log out



  Scenario: 12.1.1.170 : Automated test from Demo Flow (Brakes)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account
    And I open a folder named 'Portfolio Dashboard' from the analytics list
    Then I should see I am on the 'Portfolio Dashboard' page
    And I can see the analytics has rendered
    And I navigate to the 'Favorites' page
    Then I should see a list of favorites
    And I should be able to find a file named 'Subject Enrollment Funnel - Study' in the favorites page

    #This is work around (Ideally we should open 'Subject Enrollment Funnel - Study' from favorites tab)
    When I navigate to the 'Analytics' page
    And I open a folder named 'Subject Enrollment' from the analytics list
    Then I should see I am on the 'Subject Enrollment' page
    And I navigate to the page containing the analytics named 'Subject Enrollment Funnel - Study'
    And I open the analytics named 'Subject Enrollment Funnel - Study'
    Then I should see I am on the 'Subject Enrollment Funnel - Study' page
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    And I can see the analytics has rendered
    And I select the '3st' data point (Failed Screen: 135 Subjects) from the current 'bar chart' graphical analytics
    And I click 'Screen Failures by Reason - Study' in the Drilldown tooltip
    Then I should see I am on the 'Screen Failures by Reason - Study' page
    And I can see the analytics has rendered
    Then I can select the '2nd' data point (Other) from the current 'pie chart' graphical analytics
    And I click 'Screen Failures - Listing' in the Drilldown tooltip
    Then I should see I am on the 'Screen Failures - Listing' page
    When I navigate to the 'Analytics' page
    And I navigate to the page containing the analytics named 'Portfolio Dashboard'
    And I open the analytics named 'Portfolio Dashboard'
    Then I should see I am on the 'Portfolio Dashboard' page
    #When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    #And I select 'Beta 21' from the 'Study' session filter dropdown
    #And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    And I can see the analytics has rendered

    #Brakes on following step:
    And I can select the '1st' data point (Beta 21) from the current 'scatter chart' graphical analytics
    When I select the '1st' data point (Beta 21) from the current 'scatter chart' graphical analytics
    And I click 'Study Milestones' in the Drilldown tooltip
    Then I should see I am on the 'Subject Enrollment Rate - Study' page
    And I log out


    Scenario: 12.1.1.171 : Automated test from Demo Flow Part 2 (Breakes)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account
    And I open a folder named 'Portfolio Dashboard' from the analytics list
    Then I should see I am on the 'Portfolio Dashboard' page
    And I can see the analytics has rendered
    And I navigate to the 'Favorites' page
    Then I should see a list of favorites
    And I should be able to find a file named 'Subject Enrollment Funnel - Study' in the favorites page
    When I navigate to the 'Analytics' page
    And I open a folder named 'Subject Enrollment' from the analytics list
    Then I should see I am on the 'Subject Enrollment' page
    And I navigate to the page containing the analytics named 'Subject Enrollment Funnel - Study'
    And I open the analytics named 'Subject Enrollment Funnel - Study'
    Then I should see I am on the 'Subject Enrollment Funnel - Study' page
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    And I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    And I can see the analytics has rendered
    And I select the '3st' data point (Failed Screen: 135 Subjects) from the current 'bar chart' graphical analytics
    And I click 'Screen Failures by Reason - Study' in the Drilldown tooltip
    Then I should see I am on the 'Screen Failures by Reason - Study' page
    And I can see the analytics has rendered
    Then I can select the '2nd' data point (Other) from the current 'pie chart' graphical analytics
    And I click 'Screen Failures - Listing' in the Drilldown tooltip
    When I should see I am on the 'Screen Failures - Listing' page
    And I close the 'Filters' panel


    #Brakes on following step:
    Then I can see the Subject Enrollment list is not sorted by column 'Site Name'
    When I sort the 'Site Name' column of the tasks list
    Then I can see the tasks list is sorted by column 'Site Name' in ascending order
    When I sort the 'Site name' column of the tasks list again
    Then I can see the tasks list is sorted by column 'Site Name' in descending order
    And I log out


    Scenario: 12.1.172 : Automated test from Demo Flow (Pass)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account
    When I open a folder named 'Portfolio Dashboard' from the analytics list
    Then I should see I am on the 'Portfolio Dashboard' page
    And I can see the analytics has rendered
    When I navigate to the 'Favorites' page
    Then I should see a list of favorites
    And I should be able to find a file named 'Subject Enrollment Funnel - Study' in the favorites page
    When I navigate to the 'Analytics' page
    And I open a folder named 'Subject Enrollment' from the analytics list
    Then I should see I am on the 'Subject Enrollment' page
    When I navigate to the page containing the analytics named 'Subject Enrollment Funnel - Study'
    And I open the analytics named 'Subject Enrollment Funnel - Study'
    Then I should see I am on the 'Subject Enrollment Funnel - Study' page
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    Then I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    And I can see the analytics has rendered
    And I select the '3st' data point (Failed Screen: 135 Subjects) from the current 'bar chart' graphical analytics
    And I click 'Screen Failures by Reason - Study' in the Drilldown tooltip
    Then I should see I am on the 'Screen Failures by Reason - Study' page
    And I can see the analytics has rendered
    Then I can select the '2nd' data point (Other) from the current 'pie chart' graphical analytics
    And I click 'Screen Failures - Listing' in the Drilldown tooltip
    Then I should see I am on the 'Screen Failures - Listing' page
    And I log out
  

    Scenario: 12.1.173 : Automated test from Demo Flow Part 2 (Pass)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account
    And I open a folder named 'Portfolio Dashboard' from the analytics list
    When I navigate to the 'Analytics' page
    And I navigate to the page containing the analytics named 'Portfolio Dashboard'
    And I open the analytics named 'Portfolio Dashboard'
    Then I should see I am on the 'Portfolio Dashboard' page
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Omega 91' from the 'Study' session filter dropdown
    Then I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    And I can see the analytics has rendered
    #Start
    And I can select the '1st' data point (Omega 91) from the current 'scatter chart' graphical analytics
    #When I select the '1st' data point (Omega 91) from the current 'scatter chart' graphical analytics
    And I click 'Study Milestones - Listing' in the Drilldown tooltip
    Then I should see I am on the 'Study Milestones - Listing' page
    And I log out


    Scenario: 12.1.174 : Automated test from Demo Flow Part 3 (Breakes)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account
    And I open a folder named 'Portfolio Dashboard' from the analytics list
    When I navigate to the 'Analytics' page
    And I navigate to the page containing the analytics named 'Portfolio Dashboard'
    And I open the analytics named 'Portfolio Dashboard'
    Then I should see I am on the 'Portfolio Dashboard' page
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    Then I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    And I can see the analytics has rendered
    
    #Breakes Here
    And I can select the '1st' data point (Beta 21) from the current 'scatter chart' graphical analytics
    #When I select the '1st' data point (Omega 91) from the current 'scatter chart' graphical analytics
    And I click 'Study Milestones - Listing' in the Drilldown tooltip
    Then I should see I am on the 'Study Milestones - Listing' page
    And I log out


    Scenario: 12.1.175 : Automated test from Demo Flow Part 4 (Pass)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account
    When I open a folder named 'Site Productivity' from the analytics list
    Then I should see I am on the 'Site Productivity' page
    When I navigate to the page containing the analytics named 'Drug Accountability by Status - Country'
    And I open the analytics named 'Drug Accountability by Status - Country'
    Then I should see I am on the 'Drug Accountability by Status - Country' page
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Omega 91' from the 'Study' session filter dropdown
    Then I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    And I can see the analytics has rendered
    And I select the '3rd' data point (units: 20150) from the current 'pie chart' graphical analytics
    And I click 'Drug Accountability - Listing' in the Drilldown tooltip
    Then I should see I am on the 'Drug Accountability - Listing' page
    And I log out


    Scenario: 12.1.176 : Automated test from Demo Flow Part 5 (Brakes)
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account
    When I open a folder named 'Portfolio Dashboard' from the analytics list
    Then I should see I am on the 'Portfolio Dashboard' page
    And I can see the analytics has rendered
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    Then I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    And I can see the analytics has rendered


    # Brakes Here: 
    #And I can select the '1st' data point (Beta 21) from the current 'scatter chart' graphical analytics
    When I select the '1st' data point (Beta 21) from the current 'scatter chart' graphical analytics
    And I click 'Study Milestones - Listing' in the Drilldown tooltip
    Then I should see I am on the 'Study Milestones - Listing' page
    And I can select the '1st' data point (Beta 21) from the current 'scatter chart' graphical analytics
    And I click 'Study Milestones - Listing' in the Drilldown tooltip
    Then I should see I am on the 'Study Milestones - Listing' page
    And I open a folder named 'Subject Enrollment' from the analytics list
    Then I should see I am on the 'Subject Enrollment' page
    When I navigate to the page containing the analytics named 'Subject Enrollment Funnel - Study'
    And I open the analytics named 'Subject Enrollment Funnel - Study'
    Then I should see I am on the 'Subject Enrollment Funnel - Study' page
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    Then I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    And I can see the analytics has rendered
    And I select the '3st' data point (Failed Screen: 135 Subjects) from the current 'bar chart' graphical analytics
    And I click 'Screen Failures by Reason - Study' in the Drilldown tooltip
    Then I should see I am on the 'Screen Failures by Reason - Study' page
    And I can see the analytics has rendered
    Then I can select the '2nd' data point (Other) from the current 'pie chart' graphical analytics
    And I click 'Screen Failures - Listing' in the Drilldown tooltip
    Then I should see I am on the 'Screen Failures - Listing' page
    And I log out


    Scenario: 12.1.177 : Automated test from Demo Flow Part 4
    Given I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account
    When I open a folder named 'Subject Enrollment' from the analytics list
    Then I should see I am on the 'Subject Enrollment' page
    When I navigate to the page containing the analytics named 'Subject Evaluable - Study'
    And I open the analytics named 'Subject Evaluable - Study'
    Then I should see I am on the 'Subject Evaluable - Study' page
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    Then I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    And I can see the analytics has rendered

    #Brakes on following step:
    
    And I can select the '2nd' data point (Count of Subjects: 6) from the current 'pie chart' graphical analytics
    When I select the '1st' data point (Count of Subjects: 6) from the current 'bar chart' graphical analytic
    #And I can select the '2nd' data point (Evaluable) from the current 'pie chart' graphical analytics
    #When I select the '2nd' data point (Evaluable) from the current 'pie chart' graphical analytics
    And I click 'Study Milestones' in the Drilldown tooltip
    Then I can select the '1st' data point (Not eveluable) from the current 'pie chart' graphical analytics
    And I select the '1st' data point (Subjects: 18) from the current 'bar chart' graphical analytics
    And I click 'Subject Disposition - Listing' in the Drilldown tooltip
    And I select the '1st' data point (Iceland) from the current 'scatter chart' graphical analytics
    And I can select the '1st' data point (Beta 21) from the current 'scatter chart' graphical analytics
    And I click 'Site - Listing' in the Drilldown tooltip



    When I navigate to the page containing the analytics named 'Subject Enrollment Funnel - Study'
    And I open the analytics named 'Subject Enrollment Funnel - Study'
    Then I should see I am on the 'Subject Enrollment Funnel - Study' page
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    Then I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    And I can see the analytics has rendered
    And I select the '3st' data point (Failed Screen: 135 Subjects) from the current 'bar chart' graphical analytics
    And I click 'Screen Failures by Reason - Study' in the Drilldown tooltip
    Then I should see I am on the 'Screen Failures by Reason - Study' page
    And I can see the analytics has rendered
    Then I can select the '2nd' data point (Other) from the current 'pie chart' graphical analytics
    And I click 'Screen Failures - Listing' in the Drilldown tooltip
    Then I should see I am on the 'Screen Failures - Listing' page
    And I log out


  Scenario: 12.1.178 : Life in A day (Pass)
    When I am an authenticated admin user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account
    And I navigate to the 'Favorites' page
    When I sort the 'Title' column of the favorites list
    Then I can see the favorites list is sorted by column 'Title' in ascending order
    When I sort the 'Title' column of the favorites list again
    Then I can see the favorites list is sorted by column 'Title' in descending order
    When I sort the 'Created' column of the favorites list
    Then I can see the favorites list is sorted by column 'Created' in ascending order
    When I sort the 'Created' column of the favorites list again
    Then I can see the favorites list is sorted by column 'Created' in descending order
    When I sort the 'Type' column of the favorites list
    Then I can see the favorites list is sorted by column 'Type' in ascending order
    When I sort the 'Type' column of the favorites list again
    Then I can see the favorites list is sorted by column 'Type' in descending order
    And I log out

    Scenario: 12.1.179 : Life in A day (Pass)
    When I am an authenticated admin user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account
    And I navigate to the 'Analytics' page
    When I sort the 'Title' column of the analytics list
    Then I can see the analytics list is sorted by column 'Title' in ascending order
    When I sort the 'Title' column of the analytics list again
    Then I can see the analytics list is sorted by column 'Title' in descending order
    When I sort the 'Created' column of the analytics list
    Then I can see the analytics list is sorted by column 'Created' in ascending order
    When I sort the 'Created' column of the analytics list again
    Then I can see the analytics list is sorted by column 'Created' in descending order
    When I sort the 'Type' column of the analytics list
    Then I can see the analytics list is sorted by column 'Type' in ascending order
    When I sort the 'Type' column of the analytics list again
    Then I can see the analytics list is sorted by column 'Type' in descending order
    And I log out


    Scenario: 12.1.180: Life in A day (Pass)
    When I am an authenticated admin user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    When I switch to the 'CCDM' account if I am on another account
    And I navigate to the 'Analytics' page
    When I open a folder named 'Site Productivity' from the analytics list
    Then I should see I am on the 'Site Productivity' page
    When I sort the 'Title' column of the analytics list
    Then I can see the analytics list is sorted by column 'Title' in ascending order
    When I sort the 'Title' column of the analytics list again
    Then I can see the analytics list is sorted by column 'Title' in descending order
    When I sort the 'Created' column of the analytics list
    Then I can see the analytics list is sorted by column 'Created' in ascending order
    When I sort the 'Created' column of the analytics list again
    Then I can see the analytics list is sorted by column 'Created' in descending order
    When I sort the 'Type' column of the analytics list
    Then I can see the analytics list is sorted by column 'Type' in ascending order
    When I sort the 'Type' column of the analytics list again
    Then I can see the analytics list is sorted by column 'Type' in descending order
    And I navigate to the 'Analytics' page
    When I open a folder named 'Subject Enrollment' from the analytics list
    Then I should see I am on the 'Subject Enrollment' page
    When I sort the 'Title' column of the analytics list
    Then I can see the analytics list is sorted by column 'Title' in ascending order
    When I sort the 'Title' column of the analytics list again
    Then I can see the analytics list is sorted by column 'Title' in descending order
    When I sort the 'Created' column of the analytics list
    Then I can see the analytics list is sorted by column 'Created' in ascending order
    When I sort the 'Created' column of the analytics list again
    Then I can see the analytics list is sorted by column 'Created' in descending order
    When I sort the 'Type' column of the analytics list
    Then I can see the analytics list is sorted by column 'Type' in ascending order
    When I sort the 'Type' column of the analytics list again
    Then I can see the analytics list is sorted by column 'Type' in descending order
    And I navigate to the 'Analytics' page
    When I open a folder named 'Subject Enrollment' from the analytics list
    Then I should see I am on the 'Subject Enrollment' page
    When I navigate to the page containing the analytics named 'Screen Failure Rates - Listing'
    And I open the analytics named 'Screen Failure Rates - Listing'
    Then I should see I am on the 'Screen Failure Rates - Listing' page
    And I navigate to the 'Analytics' page
    Then I can see the analytics list is not sorted by column 'Type'
    Then I can see the analytics list is not sorted by column 'Title'
    Then I can see the analytics list is not sorted by column 'Created'
    Then I can see the analytics list is not sorted by column 'Updated'
    And I navigate to the 'Analytics' page
    And I log out



    Scenario: 12.1.1.181 : Life in A day (Brakes)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Enrollment' from the analytics list
    Then I should see I am on the 'Subject Enrollment' page
    When I navigate to the page containing the analytics named 'Subject Enrollment Rate - Study'
    When I open the analytics named 'Subject Enrollment Rate - Study'
    And I should see I am on the 'Subject Enrollment Rate - Study' page
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    Then I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    And I can see the analytics has rendered

    #Brakes:
    And I should see the following analytics in Related Analytics:
      | Subject Enrollment Rate - Country                            |
      | Subject Disposition - Listing                                |
      | Site - listing                                               |
    When I click 'Site - listing' in Related Analytics
    Then I should see I am on the 'Site - listing' page
    And I navigate to the 'Favorites' page
    Then I should see a list of favorites
    When I navigate to the 'Analytics' page
    Then I should see a list of analytics
    And I open a folder named 'Subject Compliance' from the analytics list
    Then I should see I am on the 'Subject Compliance' page
    When I navigate to the page containing the analytics named 'Protocol Deviation Rate - Study'
    #STAR 
    When I toggle the star icon for the file named 'Protocol Deviation Rate - Study' on the 'Analytics' page
    And I navigate to the 'Favorites' page
    And I should be able to find a file named 'Protocol Deviation Rate - Study' in the favorites page
    And I open a folder named 'Portfolio Dashboard' from the analytics list
    And I navigate to the page containing the analytics named 'AE Rate per Subject Days - Country'
    When I navigate to the page containing the analytics named 'AE Rate per Subject Days - Country'
    And I open the analytics named 'AE Rate per Subject Days - Country' from the favorites page 
    And I should see I am on the 'AE Rate per Subject Days - Country' page
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    Then I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    And I can see the analytics has rendered
    When I select the '1st' data point (Spain) from the current 'bubble chart' graphical analytics
    And I click 'Protocol Deviations Rate - Country' in the Drilldown tooltip
    Then I should see I am on the 'Protocol Deviations Rate - Country' page
    And I log out



    Scenario: 12.1.1.182 : Life in A day (Last Part)
    When I am an authenticated 'Admin' user with username 'testuser+cqs@xoroto.com' and password 'Test!23#45'
    And I switch to the 'CCDM' account if I am on another account  
    And I open a folder named 'Subject Enrollment' from the analytics list
    Then I should see I am on the 'Subject Enrollment' page
    When I navigate to the page containing the analytics named 'Subject Enrollment Rate - Study'
    When I open the analytics named 'Subject Enrollment Rate - Study'
    And I should see I am on the 'Subject Enrollment Rate - Study' page
    When I click on 'CHANGE' from the 'Study' session filter to switch to update mode
    And I select 'Beta 21' from the 'Study' session filter dropdown
    Then I click on 'MINIMIZE' from the 'Study' session filter to switch to minimized mode
    And I can see the analytics has rendered

    #The last test I should have, requres tasks which is not set up with current cqs account. 
    

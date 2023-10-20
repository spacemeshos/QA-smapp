# Test Scenario

#### Unique ID: 

**Description:** short info about the topic 

**Priority:** 1 (highest) - 3 (lowest)

**Prerequisites:** anything that needs to be in place before running the tests - so that the result may be considered as valid

**Test Cases:** 

[01]() - Verify Successful Wallet Recovery Using 12 Words Backup.

[02]() - Verify Error Handling - Invalid 12 Words.

[03]() - Verify Error Handling - Empty 12 Words.

[04]() - Verify Error Handling - Case Insensitivity.

[05]() - Verify Error Handling - Leading/Trailing Whitespace.

[06]() - Verify Backup Validation - Incorrect Words.

[07]() - Verify Backup Recovery with Different Word Order.

[08]() - Verify Error Handling - Missing Words.




#### Test Case ID: 01

**Description:** Verify Successful Wallet Recovery Using 12 Words Backup.

**Steps:**

1. User opens the Spacemesh application.
2. User selects the "Recover Wallet using 12 words backup" option.
3. User enters the 12-word backup.
4. User confirms the recovery process.

**Test Data:** Valid 12-word backup: 
1. stock
2. orbit
3. acquire
4. such
5. sure
6. yard
7. property
8. spoon
9. upgrade
10. mango
11. horse
12. effort

**Expected Result:** The wallet should be successfully recovered using the 12-word backup.



---

#### Test Case ID: 02

**Description:** Verify Error Handling - Invalid 12 Words.

**Steps:**

1. User opens the Spacemesh application.
2. User selects the "Recover Wallet" option.
3. User enters an invalid set of 12 words.
4. User confirms the recovery process.

**Test Data:** Invalid 12-word backup: 
1. stocks
2. galaxy
3. acquires
4. any
5. secure
6. yards
7. properties
8. fork
9. upgrades
10. mangos
11. horses
12. efforts

**Expected Result:** An error message should indicate that the 12-word backup is invalid, and the recovery process should fail.



---

#### Test Case ID: 03

**Description:** Verify Error Handling - Empty 12 Words.

**Steps:**

1. User opens the Spacemesh application.
2. User selects the "Recover Wallet" option.
3. User attempts to proceed with an empty 12-word input.

**Test Data:** Empty 12-word backup.

**Expected Result:** An error message should indicate that the 12-word backup cannot be empty, and the recovery process should fail.



---

#### Test Case ID: 04

**Description:** Verify Error Handling - Case Insensitivity.

**Steps:**

1. User opens the Spacemesh application.
2. User selects the "Recover Wallet" option.
3. User enters words with varying cases in the 12-word backup.
4. User confirms the recovery process.

**Test Data:** 12-word backup with mixed cases: 
1. Stock
2. orbit
3. acquire
4. such
5. sure
6. YARD
7. property
8. spoon
9. upgrade
10. mango
11. horse
12. eFfOrT

**Expected Result:** The recovery process should be case-sensitive and fail.



---

#### Test Case ID: 05

**Description:** Verify Error Handling - Leading/Trailing Whitespace.

**Steps:**

1. User opens the Spacemesh application.
2. User selects the "Recover Wallet" option.
3. User enters words with leading/trailing whitespace in the 12-word backup.
4. User confirms the recovery process.

**Test Data:** 12-word backup with leading/trailing whitespace: 
1.  stock
2. orbit 
3.  acquire
4. such
5.  sure
6. yard
7. property
8. spoon
9. upgrade
10. mango
11. horse
12. effort

**Expected Result:** The recovery process should fail, smapp should not accept spaces at all.



---

#### Test Case ID: 06

**Description:** Verify Backup Validation - Incorrect Words.

**Steps:**

1. User opens the Spacemesh application.
2. User selects the "Recover Wallet" option.
3. User enters a set of 12 words, including some incorrect ones.
4. User confirms the recovery process.

**Test Data:** 12-word backup with some incorrect words: 
1. stocks
2. orbit
3. acquire
4. such
5. sure
6. yard
7. property
8. fork
9. upgrade
10. mango
11. horse
12. efforts

**Expected Result:** The recovery process should fail with an error message if any of the words are incorrect.



---

#### Test Case ID: 07

**Description:** Verify Backup Recovery with Different Word Order.

**Steps:**

1. User creates a valid 12-word backup.
2. User enters the words in a different order during recovery.
3. User confirms the recovery process.

**Test Data:** Valid 12-word backup with a different word order:
1. mango
2. such
3. property
4. orbit
5. spoon
6. effort
7. upgrade
8. stock
9. acquire
10. yard
11. sure
12. horse

**Expected Result:** The recovery process should fail to recover the wallet.



---

#### Test Case ID: 08

**Description:** Verify Error Handling - Missing Words.

**Steps:**

1. User opens the Spacemesh application.
2. User selects the "Recover Wallet" option.
3. User enters a subset of the 12 words, leaving some out.
4. User confirms the recovery process.

**Test Data:** Incomplete 12-word backup: 
1. stock
2. orbit
3. 
4. such
5. sure
6. yard
7. 
8. spoon
9. 
10. mango
11. horse
12. effort

**Expected Result:** An error message should indicate that all 12 words are required, and the recovery process should fail.



---
# Portfolio

Cleaning
--------
- Deleted gameId, quarter, down, playNullifiedByPenalty, preSnapHomeScore, preSnapVisitorScore, possessionTeam, defensiveteam, yardlineSide, gameClock, targetX, targetY, preSnapHomeWinProbabaility, preSnapVisitorWinProbability, expectedPoints, playClockAtSnap, dropbackDistance, timeToThrow, timeInTackleBox, timeToSack, passTippedAtLine, penaltyYards, prePenaltyYardsGained, homeTeamWinProbabilityAdded, visitorTeamWinProbabilityAdded, expectedPointsAdded, qbSpike, qbKneel, plays where ball is spiked, and plays where ball is kneeled
- Removed "pff_" from pff_runConceptPrimary, pff_runConceptSecondary, pff_runPassOption, pff_passCoverage, and pff_manZone
- Changed the following columns to Text: playId, playDescription, offenseFormation, receiverAlignment, passResult, playAction, dropbackType, passLocationType, unblockedPressure, qbSneak, rushLocationType, isDropback, runConceptPrimary, runConceptSecondary, runPassOption, passCoverage, and manZone
- Changed the following columns to Number: yardsToGo, yardlineNumber, absoluteYardlineNumber, passLength, and yardsGained

Analysis
--------
- I organized the data by adding context to whether the offense is looking to score a touchdown within a few plays as well as whether there was a score
- The pivot tables answer questions such as:
    - What is the offensive formation and defensive formation and rush location type for rushing touchdowns in the redzone?
    - What is the pass coverage on passing touchdowns in the redzone?
    - What is the offensive and defensive formation on interceptions?
    - What is the receiver alignment on plays that gained more than 20 yards?
 
- Surprises
  - Zone defenses are more difficult to rush for a touchdown while man to man is the easiest
  - Redzone or cover-0 pass coverage is ideal for passing touchdowns while cover-1 doubles should be avoided
  - Cover-3 cloud and goal line are not likely to result in interceptions
  - A pistol offensive formation is least likely to result in an interception

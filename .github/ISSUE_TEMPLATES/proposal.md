name: Proposal
description: Proposal a major change to Project Shards
title: "[Proposal]: "
labels: ["proposal"]
assignees:
  - axtloss
  - hericiumvevo

body:
  - type: input
    id: date-proposed
    attributes:
      label: Date proposed
      placeholder: yyyy/mm/dd
    validations:
      required: true
  - type: textarea
    id: summary
    attributes:
      label: Summary
      description: A summary or what you'd like to see changed/improved
    validations:
      required: true
  - type: textarea
    id: motivation
    attributes:
      label: Motivation
      description: Does this issue/direction affect you directly? Or is it a wider known pain-point. 
   validations:
      required: true
  - type: textarea
    id: changes
    attributes:
      label: Changes
      description: To consider this Proposal as complete, what would have to be done?
    validations:
      required: true
  - type: textarea
    id: drawbacks
    attributes:
      label: Drawbacks
      description: Is this a trade-off of some kind? List any possible relecant notes here
    validations:
      required: true

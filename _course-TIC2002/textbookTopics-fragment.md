{% set textbook_topics = {
  softwareEngineering : {
    name: "softwareEngineering",
    heading: "Software Engineering",
    level_one_topics: [
      {
        name: "introduction",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "prosAndCons", heading: "Pros and Cons", priority: "3"}
            ]
          }
        ]
      }
    ]
  },
  oop : {
    name: "oop",
    heading: "Object-Oriented Programming",
    level_one_topics: [
      {
        name: "introduction",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "1"}
            ]
          }
        ]
      },
      {
        name: "objects",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "2"},
              {name: "abstraction", heading: "Objects as Abstractions", priority: "2"},
              {name: "encapsulation", heading: "Encapsulation Of Objects", priority: "3"}
            ]
          }
        ]
      },
      {
        name: "classes",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "1"},
              {name: "classLevelMembers", heading: "Class Level Members", priority: "2"},
              {name: "enumerations", heading: "Enumerations", priority: "2"}
            ]
          }
        ]
      },
      {
        name: "associations",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "1"},
              {name: "navigability", heading: "Navigability", priority: "2"},
              {name: "multiplicity", heading: "Multiplicity", priority: "2"},
              {name: "dependencies", heading: "Dependencies", priority: "3"},
              {name: "composition", heading: "Composition", priority: "3"},
              {name: "aggregation", heading: "Aggregation", priority: "3"},
              {name: "associationClasses", heading: "Association Classes", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "inheritance",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "1"},
              {name: "overriding", heading: "Overriding", priority: "2"},
              {name: "overloading", heading: "Overloading", priority: "2"},
              {name: "interfaces", heading: "Interfaces", priority: "3"},
              {name: "abstractClasses", heading: "Abstract Classes", priority: "3"},
              {name: "substitutability", heading: "Substitutability", priority: "3"},
              {name: "dynamicAndStaticBinding", heading: "Dynamic and Static Binding", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "polymorphism",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "3"},
              {name: "how", heading: "How", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "more",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "miscellaneous", heading: "Miscellaneous", priority: "3"},
              {name: "review", heading: "Review", priority: "4"}
            ]
          }
        ]
      }
    ]
  },
  requirements : {
    name: "requirements",
    heading: "Requirements",
    level_one_topics: [
      {
        name: "",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "introduction", heading: "Introduction", priority: "2"},
              {name: "nonFunctionalRequirements", heading: "Non-Functional Requirements", priority: "3"},
              {name: "prioritizing", heading: "Prioritizing Requirements", priority: "4"},
              {name: "quality", heading: "Quality of Requirements", priority: "4"}
            ]
          }
        ]
      }
    ]
  },
  gatheringRequirements : {
    name: "gatheringRequirements",
    heading: "Gathering Requirements",
    level_one_topics: [
      {
        name: "",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "brainstorming", heading: "Brainstorming", priority: "3"},
              {name: "userSurveys", heading: "User Surveys", priority: "3"},
              {name: "observation", heading: "Observation", priority: "3"},
              {name: "interviews", heading: "Interviews", priority: "3"},
              {name: "focusGroups", heading: "Focus Groups", priority: "3"},
              {name: "prototyping", heading: "Prototyping", priority: "3"},
              {name: "productSurveys", heading: "Product Surveys", priority: "3"}
            ]
          }
        ]
      }
    ]
  },
  specifyingRequirements : {
    name: "specifyingRequirements",
    heading: "Specifying Requirements",
    level_one_topics: [
      {
        name: "prose",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "3"}
            ]
          }
        ]
      },
      {
        name: "featureList",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "2"}
            ]
          }
        ]
      },
      {
        name: "userStories",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "introduction", heading: "Introduction", priority: "1"},
              {name: "details", heading: "Details", priority: "2"},
              {name: "usage", heading: "Usage", priority: "2"}
            ]
          }
        ]
      },
      {
        name: "useCases",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "introduction", heading: "Introduction", priority: "1"},
              {name: "identifying", heading: "Identifying", priority: "4"},
              {name: "details", heading: "Details", priority: "4"},
              {name: "usage", heading: "Usage", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "glossary",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "3"}
            ]
          }
        ]
      },
      {
        name: "supplementaryRequirements",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "3"}
            ]
          }
        ]
      }
    ]
  },
  design : {
    name: "design",
    heading: "Software Design",
    level_one_topics: [
      {
        name: "introduction",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "3"}
            ]
          }
        ]
      }
    ]
  },
  designFundamentals : {
    name: "designFundamentals",
    heading: "Design Fundamentals",
    level_one_topics: [
      {
        name: "abstraction",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "2"}
            ]
          }
        ]
      },
      {
        name: "coupling",
        priority: "3",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "2"},
              {name: "how", heading: "How", priority: "3"},
              {name: "types", heading: "Types of Coupling", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "cohesion",
        priority: "3",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "2"},
              {name: "how", heading: "How", priority: "3"}
            ]
          }
        ]
      }
    ]
  },
  modeling : {
    name: "modeling",
    heading: "Modeling (Using UML)",
    level_one_topics: [
      {
        name: "introduction",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "2"},
              {name: "how", heading: "How", priority: "3"},
              {name: "umlModels", heading: "UML Models", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "modelingStructures",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "ooStructures", heading: "OO Structures", priority: "2"},
              {name: "classDiagramsBasic", heading: "Class Diagrams (Basics)", priority: "2"},
              {name: "addingMoreInfo", heading: "Adding More Info to UML Models", priority: "3"},
              {name: "classDiagramsIntermediate", heading: "Class Diagrams - Intermediate", priority: "3"},
              {name: "classDiagramsAdvanced", heading: "Class Diagrams - Advanced", priority: "4"},
              {name: "objectDiagrams", heading: "Object Diagrams", priority: "2"},
              {name: "objectOrientedDomainModels", heading: "Conceptual Class Diagrams (aka OODMs)", priority: "4"},
              {name: "deploymentDiagrams", heading: "Deployment Diagrams", priority: "4"},
              {name: "componentDiagrams", heading: "Component Diagrams", priority: "4"},
              {name: "packageDiagrams", heading: "Package Diagrams", priority: "4"},
              {name: "compositeStructureDiagrams", heading: "Composite Structure Diagrams", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "modelingBehaviors",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "activityDiagrams", heading: "Activity Diagrams", priority: "4"},
              {name: "activityDiagramsIntermediate", heading: "Activity Diagrams", priority: "4"},
              {name: "sequenceDiagramsBasic", heading: "Sequence Diagrams - Basic", priority: "2"},
              {name: "sequenceDiagramsIntermediate", heading: "Sequence Diagrams - Intermediate", priority: "3"},
              {name: "sequenceDiagramsAdvanced", heading: "Sequence Diagrams - Advanced", priority: "4"},
              {name: "useCaseDiagrams", heading: "Use Case Diagrams", priority: "4"},
              {name: "timingDiagrams", heading: "Timing Diagrams", priority: "4"},
              {name: "interactionOverviewDiagrams", heading: "Interaction Overview Diagrams", priority: "4"},
              {name: "communicationDiagrams", heading: "Communication Diagrams", priority: "4"},
              {name: "stateMachineDiagrams", heading: "State Machine Diagrams", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "modelingASolution",
        priority: "-1",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "introduction", heading: "Introduction", priority: "2"},
              {name: "basic", heading: "Basic", priority: "3"},
              {name: "intermediate", heading: "Intermediate", priority: "4"}
            ]
          }
        ]
      }
    ]
  },
  architecture : {
    name: "architecture",
    heading: "Software Architecture",
    level_one_topics: [
      {
        name: "introduction",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "architectureDiagrams",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "reading", heading: "Reading", priority: "4"},
              {name: "drawing", heading: "Drawing", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "architecturalStyles",
        level_two_topics: [
          {
            name: "introduction",
            level_three_topics: [
              {name: "what", heading: "What", priority: "4"}
            ]
          },
          {
            name: "nTier",
            level_three_topics: [
              {name: "what", heading: "What", priority: "4"}
            ]
          },
          {
            name: "clientServer",
            level_three_topics: [
              {name: "what", heading: "What", priority: "4"}
            ]
          },
          {
            name: "transactionProcessing",
            level_three_topics: [
              {name: "what", heading: "What", priority: "4"}
            ]
          },
          {
            name: "serviceOriented",
            level_three_topics: [
              {name: "what", heading: "What", priority: "4"}
            ]
          },
          {
            name: "eventDriven",
            level_three_topics: [
              {name: "what", heading: "What", priority: "4"}
            ]
          },
          {
            name: "more",
            level_three_topics: [
              {name: "moreStyles", heading: "More Styles", priority: "4"},
              {name: "usingStyles", heading: "Using Styles", priority: "4"}
            ]
          }
        ]
      }
    ]
  },
  designPatterns : {
    name: "designPatterns",
    heading: "Software Design Patterns",
    level_one_topics: [
      {
        name: "introduction",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "4"},
              {name: "format", heading: "Format", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "singleton",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "4"},
              {name: "implementation", heading: "Implementation", priority: "4"},
              {name: "evaluation", heading: "Evaluation", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "abstractionOccurrence",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "facade",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "command",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "modelViewController",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "observer",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "more",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "combiningDesignPatterns", heading: "Combining Design Patterns", priority: "4"},
              {name: "otherDesignPatterns", heading: "Other Design Patterns", priority: "4"},
              {name: "usingDesignPatterns", heading: "Using Design Patterns", priority: "4"},
              {name: "otherTypesOfPatterns", heading: "Other Types of Patterns", priority: "4"},
              {name: "vsPrinciples", heading: "Design Patterns vs Design Principles", priority: "4"}
            ]
          }
        ]
      }
    ]
  },
  designApproaches : {
    name: "designApproaches",
    heading: "Design Approaches",
    level_one_topics: [
      {
        name: "multilevelDesign",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "Multi-Level Design", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "topDownBottomUp",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "Top-Down and Bottom-Up Design", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "agileDesign",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "Agile Design", priority: "4"}
            ]
          }
        ]
      }
    ]
  },
  ides : {
    name: "ides",
    heading: "IDEs",
    level_one_topics: [
      {
        name: "introduction",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "2"}
            ]
          }
        ]
      },
      {
        name: "debugging",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "3"}
            ]
          }
        ]
      }
    ]
  },
  codeQuality : {
    name: "codeQuality",
    heading: "Code Quality",
    level_one_topics: [
      {
        name: "introduction",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "basic", heading: "Basic", priority: "3"}
            ]
          }
        ]
      },
      {
        name: "maximizeReadability",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "introduction", heading: "Introduction", priority: "1"}
            ]
          },
          {
            name: "basic",
            level_three_topics: [
              {name: "avoidLongMethods", heading: "Avoid Long Methods", priority: "2"},
              {name: "avoidDeepNesting", heading: "Avoid Deep Nesting", priority: "2"},
              {name: "avoidComplicatedExpressions", heading: "Avoid Complicated Expressions", priority: "2"},
              {name: "avoidMagicNumbers", heading: "Avoid Magic Numbers", priority: "2"},
              {name: "makeCodeObvious", heading: "Make the Code Obvious", priority: "3"}
            ]
          },
          {
            name: "intermediate",
            level_three_topics: [
              {name: "structureCodeLogically", heading: "Structure Code Logically", priority: "3"},
              {name: "dontTripReader", heading: "Do Not 'Trip Up' Reader", priority: "4"},
              {name: "practiceKISSing", heading: "Practice KISSing", priority: "4"},
              {name: "avoidPrematureOptimizations", heading: "Avoid Premature Optimizations", priority: "4"},
              {name: "slapHard", heading: "SLAP Hard", priority: "4"}
            ]
          },
          {
            name: "advanced",
            priority: "4",
            level_three_topics: [
              {name: "makeHappyPathProminent", heading: "Make the Happy Path Prominent", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "followStandard",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "introduction", heading: "Introduction", priority: "2"},
              {name: "basic", heading: "Basic", priority: "3"},
              {name: "intermediate", heading: "Intermediate", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "nameWell",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "introduction", heading: "Introduction", priority: "2"}
            ]
          },
          {
            name: "basic",
            level_three_topics: [
              {name: "nounsAndVerbsAsNames", heading: "Use Nouns for Things and Verbs for Actions", priority: "2"},
              {name: "useStandardWords", heading: "Use Standard Words", priority: "3"}
            ]
          },
          {
            name: "intermediate",
            priority: "4",
            level_three_topics: [
              {name: "useNameExplain", heading: "Use Name to Explain", priority: "4"},
              {name: "notTooLongNorShort", heading: "Not Too Long, Not Too Short", priority: "4"},
              {name: "avoidMisleadingNames", heading: "Avoid Misleading Names", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "avoidShortcuts",
        priority: "4",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "introduction", heading: "Introduction", priority: "4"}
            ]
          },
          {
            name: "basic",
            level_three_topics: [
              {name: "useDefaultBranch", heading: "Use the Default Branch", priority: "4"},
              {name: "dontRecycleVarsOrParams", heading: "Don't Recycle Variables or Parameters", priority: "4"},
              {name: "avoidEmptyCatchBlocks", heading: "Avoid Empty Catch Blocks", priority: "4"},
              {name: "deleteDeadCode", heading: "Delete Dead Code", priority: "4"}
            ]
          },
          {
            name: "intermediate",
            level_three_topics: [
              {name: "minimiseVariableScope", heading: "Minimize Scope of Variables", priority: "4"},
              {name: "minimiseCodeDuplication", heading: "Minimize Code Duplication", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "commentMinimally",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "introduction", heading: "Introduction", priority: "2"}
            ]
          },
          {
            name: "basic",
            level_three_topics: [
              {name: "dontRepeatObvious", heading: "Do Not Repeat the Obvious", priority: "2"},
              {name: "writeToReader", heading: "Write to the Reader", priority: "2"}
            ]
          },
          {
            name: "intermediate",
            priority: "4",
            level_three_topics: [
              {name: "explainWhatWhyNotHow", heading: "Explain WHAT and WHY, not HOW", priority: "4"}
            ]
          }
        ]
      }
    ]
  },
  refactoring : {
    name: "refactoring",
    heading: "Refactoring",
    level_one_topics: [
      {
        name: "",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "2"},
              {name: "how", heading: "How", priority: "3"},
              {name: "when", heading: "When", priority: "4"}
            ]
          }
        ]
      }
    ]
  },
  documentation : {
    name: "documentation",
    heading: "Documentation",
    level_one_topics: [
      {
        name: "introduction",
        priority: "-1",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "guidelines",
        priority: "4",
        level_two_topics: [
          {
            name: "goTopDown",
            level_three_topics: [
              {name: "what", heading: "What", priority: "4"},
              {name: "why", heading: "Why", priority: "4"},
              {name: "how", heading: "How", priority: "4"}
            ]
          },
          {
            name: "aimForComprehensibility",
            level_three_topics: [
              {name: "what", heading: "What", priority: "4"},
              {name: "how", heading: "How", priority: "4"}
            ]
          },
          {
            name: "documentMinimally",
            level_three_topics: [
              {name: "what", heading: "What", priority: "4"},
              {name: "how", heading: "How", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "tools",
        level_two_topics: [
          {
            name: "javaDoc",
            level_three_topics: [
              {name: "what", heading: "What", priority: "2"},
              {name: "how", heading: "How", priority: "3"}
            ]
          }
        ]
      }
    ]
  },
  errorHandling : {
    name: "errorHandling",
    heading: "Error Handling",
    level_one_topics: [
      {
        name: "introduction",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "2"}
            ]
          }
        ]
      },
      {
        name: "exceptions",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "1"},
              {name: "how", heading: "How", priority: "2"},
              {name: "when", heading: "When", priority: "3"}
            ]
          }
        ]
      },
      {
        name: "assertions",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "2"},
              {name: "how", heading: "How", priority: "3"},
              {name: "when", heading: "When", priority: "3"}
            ]
          }
        ]
      },
      {
        name: "logging",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "2"},
              {name: "how", heading: "How", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "defensiveProgramming",
        priority: "4",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "4"},
              {name: "compulsoryAssociations", heading: "Enforcing Compulsory Associations", priority: "4"},
              {name: "1to1Associations", heading: "Enforcing 1-to-1 Associations", priority: "4"},
              {name: "referentialIntegrity", heading: "Enforcing Referential Integrity", priority: "4"},
              {name: "when", heading: "When", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "designByContract",
        priority: "-1",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "Design by Contract", priority: "4"}
            ]
          }
        ]
      }
    ]
  },
  integration : {
    name: "integration",
    heading: "Integration",
    level_one_topics: [
      {
        name: "introduction",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "3"}
            ]
          }
        ]
      },
      {
        name: "approaches",
        priority: "4",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "lateVsEarly", heading: "'Late and One Time' vs 'Early and Frequent'", priority: "4"},
              {name: "bigBangVsIncremental", heading: "Big-Bang vs Incremental Integration", priority: "4"},
              {name: "topDownVsBottomUp", heading: "Top-Down vs Bottom-Up Integration", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "buildAutomation",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "3"},
              {name: "continuousIntegrationDeployment", heading: "Continuous Integration and Continuous Deployment", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "more",
        priority: "-1",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "review", heading: "Review", priority: "-1"}
            ]
          }
        ]
      }
    ]
  },
  reuse : {
    name: "reuse",
    heading: "Reuse",
    level_one_topics: [
      {
        name: "introduction",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "2"},
              {name: "when", heading: "When", priority: "3"}
            ]
          }
        ]
      },
      {
        name: "apis",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "2"},
              {name: "designingAPIs", heading: "Designing APIs", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "libraries",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "1"},
              {name: "how", heading: "How", priority: "2"}
            ]
          }
        ]
      },
      {
        name: "frameworks",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "2"},
              {name: "frameworksVsLibraries", heading: "Frameworks vs Libraries", priority: "3"}
            ]
          }
        ]
      },
      {
        name: "platforms",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "3"}
            ]
          }
        ]
      },
      {
        name: "cloudComputing",
        priority: "4",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "4"},
              {name: "services", heading: "Iaas, PaaS, and SaaS", priority: "4"}
            ]
          }
        ]
      }
    ]
  },
  qualityAssurance : {
    name: "qualityAssurance",
    heading: "Quality Assurance",
    level_one_topics: [
      {
        name: "introduction",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "2"},
              {name: "validationVsVerification", heading: "Validation vs Verification", priority: "3"}
            ]
          }
        ]
      },
      {
        name: "codeReviews",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "3"}
            ]
          }
        ]
      },
      {
        name: "staticAnalysis",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "3"}
            ]
          }
        ]
      },
      {
        name: "formalVerification",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "3"}
            ]
          }
        ]
      }
    ]
  },
  testing : {
    name: "testing",
    heading: "Testing",
    level_one_topics: [
      {
        name: "introduction",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "1"},
              {name: "testability", heading: "Testability", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "testingTypes",
        level_two_topics: [
          {
            name: "unitTesting",
            level_three_topics: [
              {name: "what", heading: "What", priority: "1"},
              {name: "stubs", heading: "Stubs", priority: "4"}
            ]
          },
          {
            name: "integrationTesting",
            level_three_topics: [
              {name: "what", heading: "What", priority: "2"},
              {name: "how", heading: "How", priority: "4"}
            ]
          },
          {
            name: "systemTesting",
            level_three_topics: [
              {name: "what", heading: "What", priority: "2"}
            ]
          },
          {
            name: "alphaBetaTesting",
            level_three_topics: [
              {name: "what", heading: "What", priority: "3"}
            ]
          },
          {
            name: "dogfooding",
            priority: "4",
            level_three_topics: [
              {name: "what", heading: "What", priority: "4"}
            ]
          },
          {
            name: "developerTesting",
            level_three_topics: [
              {name: "what", heading: "What", priority: "2"},
              {name: "why", heading: "Why", priority: "3"}
            ]
          },
          {
            name: "exploratoryVsScriptedTesting",
            level_three_topics: [
              {name: "what", heading: "What", priority: "3"},
              {name: "when", heading: "When", priority: "3"}
            ]
          },
          {
            name: "acceptanceTesting",
            level_three_topics: [
              {name: "what", heading: "What", priority: "2"},
              {name: "acceptanceVsSystemTesting", heading: "Acceptance vs System Testing", priority: "3"}
            ]
          },
          {
            name: "regressionTesting",
            level_three_topics: [
              {name: "what", heading: "What", priority: "2"}
            ]
          }
        ]
      },
      {
        name: "testAutomation",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "3"},
              {name: "testingTextUis", heading: "Automated Testing of CLI Apps", priority: "3"},
              {name: "usingTestDrivers", heading: "Test Automation Using Test Drivers", priority: "3"},
              {name: "tools", heading: "Test Automation Tools", priority: "3"},
              {name: "testingGuis", heading: "Automated Testing of GUIs", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "testCoverage",
        priority: "4",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "4"},
              {name: "how", heading: "How", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "dependencyInjection",
        priority: "4",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "4"},
              {name: "how", heading: "How", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "tdd",
        priority: "4",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "4"},
              {name: "how", heading: "How", priority: "4"}
            ]
          }
        ]
      }
    ]
  },
  testCaseDesign : {
    name: "testCaseDesign",
    heading: "Test Case Design",
    level_one_topics: [
      {
        name: "introduction",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "3"},
              {name: "positiveVsNegative", heading: "Positive vs Negative Test Cases", priority: "4"},
              {name: "blackVsGlass", heading: "Black Box vs Glass Box", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "equivalencePartitions",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "4"},
              {name: "basic", heading: "Basic", priority: "4"},
              {name: "intermediate", heading: "Intermediate", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "boundaryValueAnalysis",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "4"},
              {name: "how", heading: "How", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "combiningTestInputs",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "why", heading: "Why", priority: "2"},
              {name: "combinationStrategies", heading: "Test Input Combination Strategies", priority: "2"},
              {name: "heuristicValid", heading: "Heuristic: Each Valid Input at Least Once in a Positive Test Case", priority: "3"},
              {name: "heuristicInvalid", heading: "Heuristic: Test Invalid Inputs Individually Before Combining Them", priority: "3"},
              {name: "mix", heading: "Mix", priority: "3"}
            ]
          }
        ]
      },
      {
        name: "more",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "testingUseCases", heading: "Testing Based on Use Cases", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "summary",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "recap", heading: "Recap", priority: "-1"},
              {name: "exercises", heading: "Exercises", priority: "3"}
            ]
          }
        ]
      }
    ]
  },
  projectPlanning : {
    name: "projectPlanning",
    heading: "Project Planning",
    level_one_topics: [
      {
        name: "",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "workBreakdownStructure", heading: "Work Breakdown Structure", priority: "3"},
              {name: "milestones", heading: "Milestones", priority: "2"},
              {name: "buffers", heading: "Buffers", priority: "3"},
              {name: "issueTrackers", heading: "Issue Trackers", priority: "3"},
              {name: "ganttCharts", heading: "GANTT Charts", priority: "4"},
              {name: "pertCharts", heading: "PERT Charts", priority: "4"}
            ]
          }
        ]
      }
    ]
  },
  teamwork : {
    name: "teamwork",
    heading: "Teamwork",
    level_one_topics: [
      {
        name: "",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "teamStructures", heading: "Team Structures", priority: "3"}
            ]
          }
        ]
      }
    ]
  },
  processModels : {
    name: "processModels",
    heading: "SDLC Process Models",
    level_one_topics: [
      {
        name: "introduction",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What", priority: "1"},
              {name: "sequentialModels", heading: "Sequential Models", priority: "2"},
              {name: "iterativeModels", heading: "Iterative Models", priority: "2"},
              {name: "agileModels", heading: "Agile Models", priority: "3"}
            ]
          }
        ]
      },
      {
        name: "exampleProcessModels",
        priority: "-1",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "xp", heading: "XP", priority: "4"},
              {name: "scrum", heading: "Scrum", priority: "4"},
              {name: "unifiedProcess", heading: "Unified Process", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "more",
        priority: "-1",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "cmmi", heading: "CMMI", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "summary",
        priority: "-1",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "recap", heading: "Recap", priority: "4"}
            ]
          }
        ]
      }
    ]
  },
  uml : {
    name: "uml",
    heading: "UML",
    level_one_topics: [
      {
        name: "classDiagrams",
        level_two_topics: [
          {
            name: "introduction",
            level_three_topics: [
              {name: "what", heading: "What", priority: "1"}
            ]
          },
          {
            name: "classes",
            level_three_topics: [
              {name: "what", heading: "What", priority: "1"}
            ]
          },
          {
            name: "associations",
            level_three_topics: [
              {name: "what", heading: "What", priority: "1"},
              {name: "navigability", heading: "Navigability", priority: "2"},
              {name: "roles", heading: "Roles", priority: "3"},
              {name: "labels", heading: "Labels", priority: "2"},
              {name: "multiplicity", heading: "Multiplicity", priority: "3"}
            ]
          },
          {
            name: "dependencies",
            level_three_topics: [
              {name: "what", heading: "What", priority: "3"}
            ]
          },
          {
            name: "associationsAsAttributes",
            priority: "3",
            level_three_topics: [
              {name: "what", heading: "What", priority: "3"}
            ]
          },
          {
            name: "enumerations",
            level_three_topics: [
              {name: "what", heading: "What", priority: "3"}
            ]
          },
          {
            name: "classLevelMembers",
            level_three_topics: [
              {name: "what", heading: "What", priority: "3"}
            ]
          },
          {
            name: "associationClasses",
            priority: "4",
            level_three_topics: [
              {name: "what", heading: "What", priority: "3"}
            ]
          },
          {
            name: "composition",
            level_three_topics: [
              {name: "what", heading: "What", priority: "2"}
            ]
          },
          {
            name: "aggregation",
            level_three_topics: [
              {name: "what", heading: "What", priority: "3"}
            ]
          },
          {
            name: "classInheritance",
            level_three_topics: [
              {name: "what", heading: "What", priority: "2"}
            ]
          },
          {
            name: "interfaces",
            level_three_topics: [
              {name: "what", heading: "What", priority: "2"}
            ]
          },
          {
            name: "abstractClasses",
            level_three_topics: [
              {name: "what", heading: "What", priority: "3"}
            ]
          },
          {
            name: "combine",
            priority: "4",
            level_three_topics: [
              {name: "basic", heading: "Basic", priority: "2"}
            ]
          }
        ]
      },
      {
        name: "sequenceDiagrams",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "introduction", heading: "Introduction", priority: "1"},
              {name: "basic", heading: "Basic", priority: "1"},
              {name: "objectCreation", heading: "Object Creation", priority: "2"},
              {name: "objectDeletion", heading: "Object Deletion", priority: "3"},
              {name: "loops", heading: "Loops", priority: "2"},
              {name: "selfInvocation", heading: "Self Invocation", priority: "3"},
              {name: "alternativePaths", heading: "Alternative Paths", priority: "3"},
              {name: "optionalPaths", heading: "Optional Paths", priority: "3"},
              {name: "parallelPaths", heading: "Parallel Paths", priority: "3"},
              {name: "referenceFrames", heading: "Reference Frames", priority: "3"},
              {name: "staticMethods", heading: "Calls to Static Methods", priority: "3"},
              {name: "minimalNotation", heading: "Minimal Notation", priority: "3"}
            ]
          }
        ]
      },
      {
        name: "objectDiagrams",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "introduction", heading: "Introduction", priority: "1"},
              {name: "objects", heading: "Objects", priority: "2"},
              {name: "associations", heading: "What", priority: "3"}
            ]
          }
        ]
      },
      {
        name: "activityDiagrams",
        priority: "4",
        level_two_topics: [
          {
            name: "introduction",
            level_three_topics: [
              {name: "what", heading: "Introduction", priority: "4"}
            ]
          },
          {
            name: "basicNotations",
            level_three_topics: [
              {name: "linearPaths", heading: "Linear Paths", priority: "4"},
              {name: "alternatePaths", heading: "Alternate Paths", priority: "4"},
              {name: "parallelPaths", heading: "Parallel Paths", priority: "4"},
              {name: "rakes", heading: "Rakes", priority: "4"},
              {name: "swimlanes", heading: "Swimlanes", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "notes",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "notes", heading: "Notes", priority: "3"},
              {name: "constraints", heading: "Constraints", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "miscellaneous",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "objectVsClassDiagrams", heading: "Object vs Class Diagrams", priority: "2"}
            ]
          }
        ]
      }
    ]
  },
  intellij : {
    name: "intellij",
    heading: "IntelliJ IDEA",
    priority: "4",
    level_one_topics: [
      {
        name: "",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "projectSetup", heading: "Project Setup", priority: "2"},
              {name: "codeNavigation", heading: "Code Navigation", priority: "3"},
              {name: "productivityShortcuts", heading: "Productivity Shortcuts", priority: "4"},
              {name: "debuggingBasic", heading: "Debugging: Basic", priority: "3"},
              {name: "refactoring", heading: "Refactoring", priority: "3"}
            ]
          }
        ]
      }
    ]
  },
    gitAndGithub : {
    name: "gitAndGithub",
    heading: "Revision Control (Using Git & GitHub)",
    level_one_topics: [
      {
        name: "trail",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "recordingFolderHistory", heading: "Tour 1: Recording the History of a Folder", priority: "1"},
              {name: "backingUpOnCloud", heading: "Tour 2: Backing up a Repo on the Cloud", priority: "1"},
              {name: "workingWithRemotes", heading: "Tour 3: Working Off a Remote Repo", priority: "1"},
              {name: "usingRevisionHistory", heading: "Tour 4: Using the Revision History of a Repo", priority: "1"},
              {name: "fineTuningHistory", heading: "Tour 5: Fine-Tuning the Revision History", priority: "4"},
              {name: "branchingLocally", heading: "Tour 6: Branching Locally", priority: "2"},
              {name: "syncingBranches", heading: "Tour 7: Keeping Branches in Sync", priority: "3"},
              {name: "remoteBranches", heading: "Tour 8: Working with Remote Branches", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "intro", heading: "Introduction to Revision Control", priority: "1"},
              {name: "init", heading: "Putting a Folder Under Git's Control", priority: "1"},
              {name: "stage", heading: "Specifying What to include in a Snapshot", priority: "1"},
              {name: "commit", heading: "Saving a Snapshot", priority: "1"},
              {name: "remoteRepos", heading: "Remote Repositories", priority: "1"},
              {name: "createRemoteRepo", heading: "Creating a Repo on GitHub", priority: "1"},
              {name: "setRemote", heading: "Linking a Local Repo With a Remote Repo", priority: "1"},
              {name: "push", heading: "Updating the Remote Repo", priority: "1"},
              {name: "ignore", heading: "Omitting Files from Revision Control", priority: "1"},
              {name: "fork", heading: "Duplicating a Remote Repo on the Cloud", priority: "1"},
              {name: "clone", heading: "Creating a Local Copy of a Repo", priority: "1"},
              {name: "pull", heading: "Downloading Data Into a Local Repo", priority: "1"},
              {name: "log", heading: "Examining the Revision History", priority: "1"},
              {name: "show", heading: "Examining a Commit", priority: "1"},
              {name: "tag", heading: "Tagging Commits", priority: "1"},
              {name: "diff", heading: "Comparing Points of History", priority: "1"},
              {name: "checkout", heading: "Traversing to a Specific Commit", priority: "1"},
              {name: "reset", heading: "Rewriting History to Start Over", priority: "1"},
              {name: "selectiveStage", heading: "Controlling What Goes Into a Commit", priority: "2"},
              {name: "commitMessage", heading: "Writing Good Commit Messages", priority: "3"},
              {name: "interactiveRebase", heading: "Reorganising Commits", priority: "3"},
              {name: "branch", heading: "Creating Branches", priority: "1"},
              {name: "merge", heading: "Merging Branches", priority: "1"},
              {name: "mergeConflicts", heading: "Resolving Merge Conflicts", priority: "1"},
              {name: "branchRename", heading: "Renaming Branches", priority: "3"},
              {name: "branchDelete", heading: "Deleting Branches", priority: "1"},
              {name: "syncByMerge", heading: "Merging to Sync Branches", priority: "1"},
              {name: "syncByRebase", heading: "Rebasing to Sync Branches", priority: "3"},
              {name: "cherryPick", heading: "Copying Specific Commits", priority: "3"},
              {name: "remoteBranchPush", heading: "Pushing Branches to a Remote", priority: "1"},
              {name: "remoteBranchPull", heading: "Pulling Branches from a Remote", priority: "1"},
              {name: "remoteBranchDelete", heading: "Deleting Branches from a Remote", priority: "2"},
              {name: "remoteBranchRename", heading: "Renaming Branches in a Remote", priority: "3"},
              {name: "createPRs", heading: "Creating PRs", priority: "1"},
              {name: "reviewPRs", heading: "Reviewing PRs", priority: "2"},
              {name: "managePRs", heading: "Merging PRs", priority: "2"},
              {name: "drcsVsCrcs", heading: "DRCS vs CRCS", priority: "4"},
              {name: "forkingWorkflow", heading: "Forking Workflow", priority: "4"},
              {name: "featureBranchFlow", heading: "Feature Branch flow", priority: "4"},
              {name: "centralizedFlow", heading: "Centralised flow", priority: "4"}
            ]
          }
        ]
      }
    ]
  },
  principles : {
    name: "principles",
    heading: "Principles",
    level_one_topics: [
      {
        name: "",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "singleResponsibilityPrinciple", heading: "Single Responsibility Principle", priority: "3"},
              {name: "openClosedPrinciple", heading: "Open-Closed Principle", priority: "4"},
              {name: "liskovSubstitutionPrinciple", heading: "Liskov Substitution Principle", priority: "4"},
              {name: "interfaceSegregationPrinciple", heading: "Interface Segregation Principle", priority: "4"},
              {name: "dependencyInversionPrinciple", heading: "Dependency Inversion Principle", priority: "4"},
              {name: "solidPrinciples", heading: "SOLID Principles", priority: "4"},
              {name: "separationOfConcernsPrinciple", heading: "Separation of Concerns Principle", priority: "2"},
              {name: "lawOfDemeter", heading: "Law of Demeter", priority: "4"},
              {name: "yagniPrinciple", heading: "YAGNI Principle", priority: "4"},
              {name: "dryPrinciple", heading: "DRY Principle", priority: "4"},
              {name: "brooksLaw", heading: "Brooks' Law", priority: "4"},
              {name: "review", heading: "Review", priority: "4"}
            ]
          }
        ]
      }
    ]
  },
  cppToJava : {
    name: "cppToJava",
    heading: "C++ to Java",
    level_one_topics: [
      {
        name: "",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "about", heading: "About this Book Chapter", priority: "3"}
            ]
          }
        ]
      },
      {
        name: "javaWorld",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What is Java?", priority: "3"},
              {name: "how", heading: "How Java Works", priority: "3"},
              {name: "editions", heading: "Java Editions", priority: "4"}
            ]
          }
        ]
      },
      {
        name: "gettingStarted",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "installation", heading: "Installation", priority: "1"},
              {name: "helloWorld", heading: "HelloWorld", priority: "1"},
              {name: "compiling", heading: "Compiling Programs", priority: "1"},
              {name: "running", heading: "Running Programs", priority: "1"}
            ]
          }
        ]
      },
      {
        name: "dataTypes",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "primitiveTypes", heading: "Primitive Data Types", priority: "1"},
              {name: "variables", heading: "Variables", priority: "1"},
              {name: "operators", heading: "Operators", priority: "1"},
              {name: "arrays", heading: "Arrays", priority: "1"}
            ]
          }
        ]
      },
      {
        name: "controlFlow",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "branching", heading: "Branching", priority: "1"},
              {name: "methods", heading: "Methods", priority: "1"},
              {name: "loops", heading: "Loops", priority: "1"}
            ]
          }
        ]
      },
      {
        name: "objects",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "usingObjects", heading: "Using Java Objects", priority: "1"},
              {name: "instanceMembers", heading: "Instance Members", priority: "1"},
              {name: "passingObjects", heading: "Passing Objects", priority: "1"},
              {name: "garbageCollection", heading: "Garbage Collection", priority: "3"}
            ]
          }
        ]
      },
      {
        name: "classes",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "definingClasses", heading: "Defining Classes", priority: "1"},
              {name: "gettersAndSetters", heading: "Getters and Setters", priority: "1"},
              {name: "classLevelMembers", heading: "Class-Level Members", priority: "2"}
            ]
          }
        ]
      },
      {
        name: "usefulClasses",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "api", heading: "Java API", priority: "2"},
              {name: "stringClass", heading: "The String Class", priority: "1"},
              {name: "wrapperClasses", heading: "Wrapper Classes for Primitive Types", priority: "3"},
              {name: "arraysClass", heading: "The Arrays Class", priority: "3"},
              {name: "scannerClass", heading: "The Scanner Class", priority: "3"}
            ]
          }
        ]
      },
      {
        name: "inheritance",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "basic", heading: "Inheritance (Basic)", priority: "2"},
              {name: "objectClass", heading: "The Object Class", priority: "3"},
              {name: "polymorphism", heading: "Polymorhism", priority: "3"},
              {name: "abstractClassesAndMethods", heading: "Abstract Classes and Methods", priority: "3"},
              {name: "interfaces", heading: "Interfaces", priority: "3"}
            ]
          }
        ]
      },
      {
        name: "exceptions",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What are Exceptions?", priority: "2"},
              {name: "how", heading: "How to use Exceptions", priority: "3"}
            ]
          }
        ]
      },
      {
        name: "generics",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "What are Generics?", priority: "2"},
              {name: "how", heading: "How to use Generics", priority: "3"}
            ]
          }
        ]
      },
      {
        name: "collections",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "what", heading: "The Collections Framework", priority: "3"},
              {name: "arrayListClass", heading: "The ArrayList Class", priority: "2"},
              {name: "hashMapClass", heading: "The HashMap Class", priority: "3"}
            ]
          }
        ]
      },
      {
        name: "junit",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "basic", heading: "JUnit: Basic", priority: "2"},
              {name: "intermediate", heading: "JUnit: Intermediate", priority: "3"}
            ]
          }
        ]
      },
      {
        name: "misc",
        level_two_topics: [
          {
            name: "",
            level_three_topics: [
              {name: "enums", heading: "Enums", priority: "3"},
              {name: "packages", heading: "Packages", priority: "3"},
              {name: "accessModifiers", heading: "Access Modifiers", priority: "3"},
              {name: "constants", heading: "Constants", priority: "3"},
              {name: "casting", heading: "Casting", priority: "3"},
              {name: "fileAccess", heading: "File Access", priority: "3"},
              {name: "jar", heading: "Using JAR Files", priority: "3"},
              {name: "varargs", heading: "Varargs ", priority: "4"},
              {name: "streams", heading: "Streams", priority: "4"},
              {name: "javaFX", heading: "JavaFX", priority: "4"}
            ]
          }
        ]
      }
    ]
  }
} %}

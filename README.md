# MYM Games Studios Challenge
Test case for MYM Games Studios 

## Design Choices
- BPI_Actor is kind of useless here. The purpose if it is just overriding or exposing CPP functionality. Since the project outline stated that this should be a blueprint only project, it wasn't possible to properly overriding or using CPP functios. Hence, this interface exists.
- BP_ColorMachine and BP_ShapeMachine has similar functionality. However they have implemented as separate actors, without any common base. I don't think having a base would be the best solution considering they would still override the same functions and implement same as they are doing right now. It both feels like code duplication and separate logic (due to possibility of different future extensions) at the same time. I'm not sure what would be the best solution
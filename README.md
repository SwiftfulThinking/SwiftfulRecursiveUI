LazyZStack is similar to adding several items into a ZStack and then adding logic to determine which item to render based on selection. This component manages the View's rendering lifecycle and ZIndex patterns so that SwiftUI Transitions always work as expected.

LazyZStack supports Bool, Int, or Identifiable selection.
Set allowSimultaneous to false to restrict the view to render only one item as a time.
LazyZStack is actually named AnyRecursiveView under the hood. AnyRecursiveView is a SwiftUI View that recursively renders views in a pattern similar to using a linked-list. Each layer of the view renders itself and/or an array of its children, which are also recursive views.


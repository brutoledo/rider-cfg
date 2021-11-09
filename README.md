# rider-cfg

Setup:
- `Open Rider`
- `Open settings with ctrl + alt + s`
- `Go to Editor > Live Templates > C#`

Create:

xfact - Template for XUnit fact tests
[Fact]
public void Test_$MethodName$_Should$DoWhat$()
{
    // Arrange
    $END$
    // Act

    // Assert
    Assert.True(false);
}
 
xtheory - Template for XUnit theory tests
[Theory]
[InlineData(1, 2, 3)]
[InlineData(int.MinValue, -1, int.MaxValue)]
public void Test_$MethodName$_Should$DoWhat$(int value1, int value2, int expected)
{
    // Arrange
    $END$
    // Act

    // Assert
    Assert.Equal(expected, value1);
    Assert.Equal(expected, value2);
}
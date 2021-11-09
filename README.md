# rider-cfg

Setup:
- `Open Rider`
- `Open settings with ctrl + alt + s`
- `Go to Editor > Live Templates > C#`

***
<h3>xfact - Template for XUnit fact tests</h3>

    [Fact]
    public void Test_$MethodName$_Should$DoWhat$()
    {
        // Arrange
        $END$
        // Act
    
        // Assert
        Assert.True(false);
    }

***

<h3>xtheory - Template for XUnit theory tests</h3>

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
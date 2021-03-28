```java 
public boolean onCommand(CommandSender sender, Command command, String s, String[] strings) {
    if (sender instanceof Player) {
        Player player = (Player) sender;

        // Create a new ItemStack (type: diamond)
        ItemStack diamond = new ItemStack(Material.DIAMOND);

        // Create a new ItemStack (type: brick)
        ItemStack bricks = new ItemStack(Material.BRICK);

        // Set the amount of the ItemStack
        bricks.setAmount(20);

        // Give the player our items (comma-seperated list of all ItemStack)
        player.getInventory().addItem(bricks, diamond);

        getLogger().info("Item given");
    }

    return true;
}
```

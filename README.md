# guiapi

# EX)
```java
        Plugin plugin = Bukkit.getPluginManager().getPlugin("Test");
        ItemStack itemStack = new ItemStack(Material.APPLE);
        Gui.frame(plugin, 3, "Test Title! Click Apple!")
                .slot(1, 4, itemStack, event -> {
                    Player player = (Player) event.getWhoClicked();
                    player.sendMessage("You Clicked Apple!");
                    player.closeInventory();
                });
```
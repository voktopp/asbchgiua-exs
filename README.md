# asbchgiua-exsdefmodule Hangman.GameTest do
  use ExUnit.Case
  alias Hangman.Game

  test "new_game returns structure" do
    game = Game.new_game()
    assert(game.turns_left == 7)
    assert(game.game_state == :initializing)

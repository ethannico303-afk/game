# game
game &lt;3
gam coding stuff






if box_y > HEIGHT:
        text = font.render("GAME OVER", True, BLACK)
        screen.blit(text, (WIDTH//2 - 100, HEIGHT//2))
        pygame.display.update()
        pygame.time.delay(2000)
        running = False

    # Draw objects
    pygame.draw.rect(screen, BLUE, (player_x, player_y, player_WIDTH, player_HEIGHT))
    pygame.draw.rect(screen, RED, (box_x, box_y, box_size, box_size))

    # Show score
    score_text = font.render("Score: " + str(score), True, BLACK)
    screen.blit(score_text, (10, 10))

    pygame.display.update()

pygame.quit()
sys.exit()

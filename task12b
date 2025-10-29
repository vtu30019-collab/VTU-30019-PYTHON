import pygame

# Initialize pygame
pygame.init()

# Set screen size and title
screen_size = (640, 640)
screen = pygame.display.set_mode(screen_size)
pygame.display.set_caption('Chess Board')

# Define colors
black = (0, 0, 0)
white = (255, 255, 255)
brown = (153, 76, 0)

# Define function to draw the board
def draw_board():
    for row in range(8):
        for col in range(8):
            square_color = white if (row + col) % 2 == 0 else brown
            square_rect = pygame.Rect(col * 80, row * 80, 80, 80)
            pygame.draw.rect(screen, square_color, square_rect)

# Define function to draw the pieces
def draw_pieces(board):
    piece_images = {
        'r': pygame.image.load('images/rook.png'),
        'n': pygame.image.load('images/knight.png'),
        'b': pygame.image.load('images/bishop.png'),
        'q': pygame.image.load('images/queen.png'),
        'k': pygame.image.load('images/king.png'),
        'p': pygame.image.load('images/pawn.png')
    }
    for row in range(8):
        for col in range(8):
            piece = board[row][col]
            if piece != '.':
                piece_image = piece_images[piece]
                piece_rect = pygame.Rect(col * 80, row * 80, 80, 80)
                screen.blit(piece_image, piece_rect)



# Define initial state of the board
board = [
    ['r', 'n', 'b', 'q', 'k', 'b', 'n', 'r'],
    ['p', 'p', 'p', 'p', 'p', 'p', 'p', 'p'],
    ['.', '.', '.', '.', '.', '.', '.', '.'],
    ['.', '.', '.', '.', '.', '.', '.', '.'],
    ['.', '.', '.', '.', '.', '.', '.', '.'],
    ['.', '.', '.', '.', '.', '.', '.', '.'],
    ['P', 'P', 'P', 'P', 'P', 'P', 'P', 'P'],
    ['R', 'N', 'B', 'Q', 'K', 'B', 'N', 'R']
]

# Draw board and pieces
draw_board()
draw_pieces(board)

# Start game loop
while True:
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            pygame.quit()
            quit()
    pygame.display.update()

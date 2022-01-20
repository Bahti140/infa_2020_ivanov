# infa_2020_ivanov
def main():
    x, y = 300, 400
    width, height = 200, 300

    draw_house(x, y, width, height)


def draw_house(x, y, width, height):

    """
    Нарисовать домик в полной ширины widtg и высоты height
    от опороной точки x y котороя находится в середине  нижней точки фундмента

    :param x: координата x середины домика
    :param y: координата y низа фундамента
    :param width: полная ширина
    :param height: полная высота домика
    :return: None
    """
    print("Типа ресую домик......", x, y, width, height)
    foundation_height = 0.05 * height
    walls_height = 0.5 * height
    walls_width = 0.9 * width
    roof_height = height - foundation_height - walls_height

    draw_foundation(x, y, width, foundation_height)
    draw_house_walls(x, y - foundation_height, walls_width, walls_height)
    draw_house_roof(x, y - foundation_height - walls_height, width, roof_height)


def draw_foundation(x, y, width, height):
    print("Типа ресую основание......", x, y, width, height)
    pass


def draw_house_walls(x, y, width, height):
    print("Типа ресую стены......", x, y, width, height)
    pass


def draw_house_roof(x, y, width, height):
    print("Типа ресую крышу......", x, y, width, height)
    pass


main()

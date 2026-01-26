class Kitap:
    def __init__(self, at):
        self.at = at


class Okyrman:
    def __init__(self, at):
        self.at = at
        self.kesiktirilgen = 0

    def kitap_kesiktiru(self, sany):
        self.kesiktirilgen += sany


class Kitaphana:
    def __init__(self, atauy, jalpy_kitap):
        self.atauy = atauy
        self.jalpy_kitap = jalpy_kitap
        self.berilgen_kitap = 0

    def kitap_beru(self, sany):
        if sany <= self.jalpy_kitap:
            self.berilgen_kitap += sany
            self.jalpy_kitap -= sany
        else:
            print("Кітап жеткіліксіз!")

    def kitap_kaytaru(self, sany):
        self.berilgen_kitap -= sany
        self.jalpy_kitap += sany
        print("Кітап қайтарылды, жалпы саны жаңартылды")

    def zhana_kitap_kosu(self, sany):
        self.jalpy_kitap += sany
        print("Жаңа кітаптар қосылды")

    def kesiktiru_tekseru(self, okyrman):
        if okyrman.kesiktirilgen > 3:
            print("Кешіктірілген кітаптар тым көп!")
k1 = Kitaphana("Орталық кітапхана", 100)
o1 = Okyrman("Айбек")

k1.kitap_beru(10)
k1.kitap_kaytaru(5)
k1.zhana_kitap_kosu(20)

o1.kitap_kesiktiru(4)
k1.kesiktiru_tekseru(o1)


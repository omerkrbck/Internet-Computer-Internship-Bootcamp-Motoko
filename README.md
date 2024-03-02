// hesap makinası

actor hesap_makinasi {
  var hucre : Int = 0;

  // toplama fonksiyonu
  public func toplama(s : Int) : async Int {
    hucre += s;
    hucre;
  };

  // cıkarma fonksiyonu
  public func cikarma(s : Int) : async Int {
    hucre -= s;
    hucre;
  };

  // carpma fonksiyonu
  public func carpma(s : Int) : async Int {
    hucre *= s;
    hucre;
  };

  // bolme fonksiyonu
  public func bolme(s : Int) : async ?Int {

    if (s == 0) {
      null;
    } else {
      hucre /= s;
      ?hucre;
    };
  };

  public func temizle() : async () {
    hucre := 0;
  };
};

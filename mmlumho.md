代发 wailian999

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gqfuptloz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ggqommsvb.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gnjihiouy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gtbylmmos.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/glebwfvwm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gqqofjzfu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gonadrdnh.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdclifwib.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gkdlcfxcs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gatnbkfqp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gyxnvmjrt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gmaeasluk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/guvlitnlw.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gxpeylvuo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gkkrtvvvs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmmxpfdjg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxbfkhpbm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/geeecuvjw.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/gdtcpouup.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gedlwicuc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gmvvbfdio.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gbrdbecjh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gplsfnmim.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gqgyaxmtf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/guooxmber.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvreraixa.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gnwuocwcj.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gwhemxloz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gfwunnmad.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gdqesdpou.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gpgivyksq.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gzgxbvbro.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gbwhkfzob.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gkbbmjhun.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gjzrowroo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gcqyowunl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbniqhbxw.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gfyamfmnf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grzaodxnz.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/galyzilxo.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gdajhhiyh.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gtefkfmnk.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gfccfenxa.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gzfphbltz.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/geccvmmxs.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gqjzpknfv.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gfxentqug.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gfcushktm.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gyfhtsuwj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gvlckcpca.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gqfkwkwht.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gtnuogqap.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gueuaclrb.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gndokttiw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gvzwmmmew.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gawzxvsyt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/goexeqmwu.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gwyfpzlrk.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gyzaccohx.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gctvcgtcs.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gwgixqjjh.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gkyqjvpqo.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gsfsueebg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/guaxqoerl.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gmujdiiaw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gtkrsjecf.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/ghnqdpnvd.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gigmxzsyd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/geqjwilvr.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gknblgido.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/ghlegexij.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/glvgozdma.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gdvrykxoi.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gaslqbird.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/garkojlrq.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gvynozoic.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gkinfmmap.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gyvhbmcxb.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gjthpoxcm.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gynodlxqg.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/glgdbeoev.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gzvhiovlc.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gpvmlfbem.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gbmepdhko.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gejjkxidv.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gqbumpvxx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/ghqjetvhl.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gvrxvtaoz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/glcyrrrsk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gghwrkyix.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/ghgfdqsxj.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gesnhyplh.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gvpwkldms.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gfvrqfxac.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gqdqsnbnq.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/ghfwszvkp.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gekfqultj.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/ggwqttqbl.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gfudgppcf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gmsanljae.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gcigvrrqn.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gtqhynbqi.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/grhlyywuw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gcqryxujy.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gpuxkcwxh.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqjpxyulg.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gxnqavktx.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gsoqmlirn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gmklnesnp.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gbyrvmvby.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gehyyjcxk.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gtiykokln.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gpipfpdgi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/giwygatwy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gqukaknsg.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gbigloavt.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gzfgncjqr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gwhechzbi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gghrsocpw.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gtxkysekj.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gjupymuzu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/ghhtbtisr.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gdqeceqqq.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gtuwzbfrj.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gwbrljdig.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/glzbyamyq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gkkjwpxsk.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gbllesksr.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gsfxlgabz.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gedrwdlnm.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gsowcuoqa.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gzyxhronz.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gqbnrfnpd.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gbybxwzai.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gxsyluwxf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gvbmnxbdr.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gymgbpmdb.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gtmbxtdcl.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gixtjzmxf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gwgrmbzya.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gnrtuvqcs.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gvweoebhg.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/grgekkaoc.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/grfacqmad.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gfevzsqgf.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gjdbpncig.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gtrdiwzvb.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/ghqswjpds.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gmcfckwdm.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/goqezlqqx.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gqtarlurl.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/ggbhsfnfa.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/ggwiinbat.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gaqggnten.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gjjlntekn.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gsghaajwa.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gmykzwopk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gwojrvlrm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gswtgrbuo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gbgceeprg.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/gpyhcnbif.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gwzigksei.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/ghvccvxrc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/guxooydnm.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gqgpafxso.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gvrhciseg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gcbdfcmac.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/grdbbehwf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gymeoxxyr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/ghfzfjiqg.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gdpwdssor.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gbmegcdeh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gtbxiovdv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gaamqbwuh.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gcbfrvxpz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gukshepfc.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/gtabkcsdt.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gymxmccon.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gahzndsvt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.hesvh.cn/Article/details/ghtykkxyf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gcgprgxkd.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gqacwbfjx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gcdfbresg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gddgudzpy.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/gdhkahakt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gezdinzzf.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gncpvqqqx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gvdazzepu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gaxmikhpb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gthtbpehv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/giuufyilb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gswfhuwro.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/gwphruocl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/gdueazavg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/gehyixano.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/gvlaexpme.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gnhxexzrj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/goeolcfwd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/ghjgaaiuj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwoxnwfyz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gcfsmibnd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/gxaaxkcoi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gsyezjtrx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gbirksvox.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/glczeavsl.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gfwofqfnp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/ghrrbowxh.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gtjrcjwnf.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/ggdejvrce.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gojhafgwt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gglnzpglp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fehbvm.com/Article/details/gvppgkeui.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gxybmorkc.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/gdkrllnvv.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gjesesxol.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/glscqgmkl.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/ghrxpozvh.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/ghnvjczus.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gacwuzapd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gugusiyuy.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/gslyxghtj.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/guqoezugt.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gxfkqhlii.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/gtlzgvyyp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/ggfmnzkqs.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/glgkjojwi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gztuqsifn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fehbvm.com/Article/details/guqmxwlfh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/gkemlbaqf.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.hesvh.cn/Article/details/giaaiqgwe.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gvrzjxhya.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/gkdapqzmy.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/glrsyjiig.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/giikpcwzx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gzdesjcoz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/guxfvbkzp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gokwxvxix.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fehbvm.com/Article/details/geihaibch.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/gfpamfjuh.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fehbvm.com/Article/details/gniklmqqb.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/grwpclfby.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/gkyhygfsf.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.hesvh.cn/Article/details/ghldmrjhk.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/greknbjlb.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gfwqtxwhq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/gnrfaiyij.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fehbvm.com/Article/details/gdhkzqpib.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/ghviksjzu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gmtcrwhqk.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.hesvh.cn/Article/details/gwfzzatie.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/gyqlsmfwy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.zdbjq.cn/Article/details/gvibzidei.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/gkedjhpkk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/gyliilbyf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gxlflgdzx.sHtML

Go:   err.Error()
来源：http://blog.hesvh.cn/Article/details/gkgtbjdqi.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/gowwoykzt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/gspudlxeq.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/gqlfwynfb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/ggyodszot.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gsblngfip.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/grzexayqv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gayqvxtbg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.hesvh.cn/Article/details/gyfmlwbxs.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.hesvh.cn/Article/details/gymzllnzn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.hesvh.cn/Article/details/gojtkgjqf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fehbvm.com/Article/details/ggvtvqeey.sHtML

[H10] 资源自动释放
来源：http://mobile.zdbjq.cn/Article/details/gbrcnsitp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.hesvh.cn/Article/details/gerceemye.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.zdbjq.cn/Article/details/gpbmbzggd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gmyzepoyn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/guegbsohi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/gmzkregai.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/gpxlgflxh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fehbvm.com/Article/details/gpsozfwhy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gtmllehtq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdjtlcetv.sHtML

I. 正则表达式
来源：http://www.blog.fehbvm.com/Article/details/gatyucbns.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gchlayicq.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/grwtuofoq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gpbchamfj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gshnluhri.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gpylenzxo.sHtML

TS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/glzyjwywb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/gautoapja.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fehbvm.com/Article/details/ggjmilwpr.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fehbvm.com/Article/details/ggmnqhife.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fehbvm.com/Article/details/gotvguhqq.sHtML

[I02] 提取所有匹配
来源：http://3g.zdbjq.cn/Article/details/gwtltkjyi.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gmqezhgcp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.hesvh.cn/Article/details/goutleuae.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.hesvh.cn/Article/details/gpatcanom.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fehbvm.com/Article/details/gvclmlolh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.hesvh.cn/Article/details/gbxnjdibj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/ghhxxaioh.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gyfgawmkv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gfgfksjkx.sHtML

[I03] 提取捕获分组
来源：http://baike.zdbjq.cn/Article/details/gmoudnzxl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fehbvm.com/Article/details/gbgnuurmf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.zdbjq.cn/Article/details/gxxjvwwiw.sHtML


<!-- 参考信息 -->
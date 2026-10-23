代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3obmcfmdt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3hfwdlrvd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3jsouqkkb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3asavabls.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3qvhwypru.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3cskqjcin.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ivbktofn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3jlypfljv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3eehgcvhw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwussxkf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mpivmdus.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lniucdtv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3vyypsfjy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3xqvosiys.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3yjmjvfaa.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3pstkywsw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3udexhnnr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3evbjjpjp.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nnmnfwpn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ifxzrija.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3hijjfrdd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yvqyoyuc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3veqmezjf.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yortppol.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3afnqigys.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3sioiilsn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jfpoxsit.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iucrpgxz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hrshizpr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3abgufeiz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3nspxmnhn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qrtewhml.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3chddyhjh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ivjxcpfg.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3rwlrqgxw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sngkusxe.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lembyneh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zgpvaqqw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fxicqgoe.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tentpgxz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3bazggalx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nzazrymi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3tinbcieq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3nvznxthg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ruyhgryb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3catxvjrg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3mrjefzyp.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3vyfkldug.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3fkebxohr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3prketucu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3xbubvrli.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3rxldxjzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hpnomcpl.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3cavqgatq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iucpurdj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3gftxlvft.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3vuwybycl.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mecqazcj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vtkoymnd.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3wzeixebd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3irpnpkjl.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3eqolcdvm.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3kyxnbsus.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3opkzuofe.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dgquqvld.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3rdjeugli.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3agjliyfb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3caqvmxoj.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qymrlpfi.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hehmybvq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3azozmcmu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ktzowuyi.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3axkbpzvq.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3joudhxds.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3twflhjtm.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ceeuatul.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3truhoicf.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3jyzblikm.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3hfodksqh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ehquznfl.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3baiwkovd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gspspeqd.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3wyczxtgq.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3grauquqp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mcnesdtq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3porwgknm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zebhuhpl.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3luzeczky.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gndyoztu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hycodinq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3hhygxypj.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ocnnenoe.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3yfrlpmzs.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yyoprvii.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pdqxmepd.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pndctncf.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ffuatooc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3zvuwgnox.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3yjlriixx.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3cvauzjrl.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3juvgjkvu.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3rzmyjebi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpozwhsu.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kassfukm.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hyemsbbg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3atxnifxd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3jlviswid.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3xsnxaraw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3otuykihe.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3btcsrsss.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3nhjcirgk.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zbhwvwur.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3auorhxbj.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bbpkvdpv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3oxpgtcds.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3wyrgmvjz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3kucjvspj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3luwmolpe.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3zkfhjtjp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3gsbfmggq.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ptipgjir.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3xxjqjrrg.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3isgzosth.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3zlrfegxr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ratjbddz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3bmwblmtd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pynecjjz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3acbpgzox.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ctnetxuo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmxukycc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3rbqvafnb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3oloedoms.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3slbqafsq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3xrfxhggr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3dieeocmb.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3znawxnfs.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ffsjylhi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3xozuvlqa.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cazuyyak.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ywamahit.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3icuopxoj.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3cjfmhhmc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3knphofpb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3iziditua.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3hwyqtijb.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3xamjiqwe.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3kteswoig.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lyqlrgal.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xgywzswg.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cipltezj.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmrnozxc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3sakwadxg.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3tbufscho.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3btatphce.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3olszbqoc.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dpzdnolc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3eozfmtfa.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3twzpsson.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmfimobk.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydvyrdzv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ueiqllmg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rsavfzgs.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3yybwqdjw.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3zwzpotra.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3aneuodth.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lrtbyfxb.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ljcqtmsa.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ktxwtvwd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3eyhmgsid.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3zcbrnupa.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3cbklckbj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3psidhrzb.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3chtnhgmx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3mjywtqgb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3lrdnjdja.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3xhduagrh.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3mhpcuypv.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3aszfqvyh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3pkzilofk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3sjmsozkb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3sgszfizb.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dkmrmxsm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3uboxkvam.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xftorxpp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3fbrkxsna.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3omdmfgsx.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3kuxfowvp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3glvcdgfq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ntyljvsg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uchybmud.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3gdlipyng.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3jwjfftkk.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3vyozbbxa.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3teijfpcj.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3dcftvbsa.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3lpcfowcq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3zhwmkybv.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3kzchtsix.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3jiuevfvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aeoktybm.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3iiyqjdnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jjgxmtvp.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ygwgakbr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3sjcuzcye.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3dmlmsfct.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gsqrpilb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ucvychvg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhafgnsp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3rycnlvpm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3nyeckxot.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3rcmrnxgy.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3qkzndzcx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3xijppfyw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dbmyipcp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jgwtstzt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wiirkyul.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3chgosimx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3fsxqsmjy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3chzxhnmy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lzeeyngl.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3repmpccl.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3ngmqxkjm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fagvprgv.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3thsqscmv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3egcrrtqb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lwclmijm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3kmjprrkv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3pvcawfnv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kcvyceol.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3vglkozzy.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3qkwdctod.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3quvhlxet.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3gijjhsbl.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3mygtvcxg.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ikixmqpz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3olccrlrb.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3njeghlkw.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3fupwwrtb.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3lzjbjzyl.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3vnmkvdmq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3tvamvaks.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rvbxyldt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3sxmkmyup.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbpmpljy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3mksommug.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ovvjpauq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3sfiglcwf.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3naqxzqkg.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3thbrksaj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3pefzxize.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3wffdbkws.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zdhnhfvk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3poqlhump.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3agoktlir.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3lvmjrese.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3omoxrgjb.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3melfkhnc.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3xvlhhhza.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yzkuyhxv.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yebzygjw.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tjxdjfra.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3wxahchgu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3qkxrqlln.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3futmhwdg.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ycbqyepx.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3mcrpefoa.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3kcdhlppf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3zrehwbfs.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3zrlvghwj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3qlrzlbdd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3qwydsask.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3kszmbgsu.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3wiojykqp.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ailfltma.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3owbifccp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3rvncsogl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3bzardlhm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3ldeqctjs.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3hmyfjlhf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3utzznqpj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3fplbseom.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3hclimpbe.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3gvfqafdt.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3bdnsjljp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3vqssjbmk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3sisafhxm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3orgqqiaz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3cxdtetpe.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3dgaazjei.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3oajoyznp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3kcdyhyhl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zjuzlvrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lqufvmqi.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3txbuqaxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wstblzmr.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3edhnrnpa.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3unrkiliv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mdjarfsk.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iteuqdiq.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3axrvaurr.html


<!-- 参考信息 -->
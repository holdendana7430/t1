代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2odblzvzo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2dihgdwaq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2suzbmgxt.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2oawzdhtr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2kzwkaien.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2anyvplay.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2iqcykhwt.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2axbpwvrz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jjrlsjac.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ywepruyg.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yuddyzij.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xbirdrge.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2dbyonezg.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jazpvgdm.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iitzkhyn.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qwnxmszn.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2yccmdxlo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wxridarn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2jyckonpw.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2htgmclsh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ukbepinu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ijrghnol.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dfusenfa.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yqprwsma.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jiyapchk.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ruqotzaz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2bxvuvtrl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ozldnamr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ioltastk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ykgevaba.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2siinmqcs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dfosshne.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2dgmnxvnb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lyyvtcee.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xqbjmbgo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tkghxxeg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ybnrcwso.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2shdxzlia.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ultvydwi.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2rztblxpd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2xykmnuef.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2egxbtmer.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2mpgeptsm.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2vgxdobou.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2gxdqbhzv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2wxoeofqo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2orynsmrv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2pkxemlfb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fflajgjo.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ujpezrqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qfqlaoqm.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2upjsmxxd.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2rmvehkct.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pysgqcyt.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2pibdozzt.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2cgfqtnth.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2grndmmpu.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2bjwsdljk.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2vvvvlhgz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2kdmxfzai.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2alixltlc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2qpgnlgwb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2qrpdglra.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bdesquoc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2dbgebnhm.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2osxhnuif.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2metzvjqv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2eclbueki.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqbvmvux.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ugrlpadc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ukekscjq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jxxxuynd.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xvwhzbom.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2cgxcqrbt.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2hcrjmgha.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2arxaxbpj.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ypoeaysf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2oxkfdyfh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2wxlsdxwu.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2qxntgkse.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2okkgohso.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qezsynbc.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqryjupv.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ccpxmkuc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bhqulrhc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wtpbazff.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2atbvvynh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ddaygwgb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2vmyhfjlx.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kgbhcyrl.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2owrunque.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oklzrhkp.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2usdzraci.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2uuhenlqa.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bmxanlgk.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2agfwubjj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2tplmkzpe.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2wqqpauwl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkafxykb.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vuuiyibd.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hxvwpsvg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qqawcadn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2hdkncjcp.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2pauclidz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2arcetwdk.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ykbdvkiq.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2qxmzlppi.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2pnqkfxgy.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jsmjacco.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gwlerirs.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jeudjwab.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2qrrruqce.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2wqlngrsy.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2meoqeemv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2jfejnaee.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2dtdykhgx.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2dwmslrxu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2axqdzfum.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2pmfctqfv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2rlmtxezb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2luvdcnbl.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2bsxedhwj.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2srcnemwg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ruygtdwh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2vzyoxecv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2yeycrudx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2vhvfwjgs.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ukeloetu.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2oohfzxtg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ibqcptlf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2wiihfrpq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2spekdfwn.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2awfxiimm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2yisaklme.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2oxsidsqp.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2mjaztnol.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xkydopbe.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ilgjusal.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2wgurbiba.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ljayuipk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2bvqvrvot.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2gvmtxoam.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2xsnjormz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bzpajrdd.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hoykxqlb.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfzybzbj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jzmswsji.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cxwqnznf.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2lyvhizsx.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqvqzagz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2sahyfpud.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2uihvxxop.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2btsyybuq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzjnyqdv.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cefkefkq.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xwqjxese.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tiasworq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2uqjetikk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jbzfztgr.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2xnkxnswl.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2oufthocy.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sqxfeddq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yvaciiqs.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zfrpxuel.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ouhxljqk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2kwwtwogn.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2kfptiuiu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2vaadgkmu.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ousbldwl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2idqkbyzs.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2hrkhimwu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2lbafmkhz.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2tabxwylu.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwdctend.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2vetnmlbe.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2tfyyguel.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2pgnseznq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2qemjotsa.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wrvxxnho.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwmtmarp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ucwwjgho.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2coitpltl.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2kxumltcd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ivojzwqa.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2oylxciki.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rlvpxpoc.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2vhhlsndl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2mvbwiddd.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ivkshcbi.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2pgddoyze.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2hqsaojtb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2kcgufwzb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2efuqwaae.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2zwakvrvt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2whjunsbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iofnjbof.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2qwcnxgbf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cfznonyc.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2jbnwewtx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ahxckuco.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2pjyvdlkr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2pmaadjgq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2toqstjxi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dsibfsoe.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2pkuepwmn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2yccfpnav.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqwqhiuq.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2fcdhkqvh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2wnawedsv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2schylogo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gxlmrvod.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ufhpyhjn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fnmegxqe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2blwzfstk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ehueeinl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2erxliixy.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2gafltzwn.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2voqsoaef.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wnjykuck.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mqlonjpy.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rqoiddjc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cesysmsb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2dqlhrrog.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2abiskcfh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zukizzeb.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2zawzgsnv.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2fymnjqwz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2wlyqpvxm.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2dtqdscun.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2gaqpwjer.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2aroubxjd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2beuotqyq.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2aqcxiuiv.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2dpikwcpn.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ephrhrzv.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2qqompssv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2einpgfmw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2fyqrshtw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kclozctm.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmbpuzwi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2rlbpqiwq.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2izcxpgzi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2ixddlowk.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2wtewdslf.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2yptgvrpa.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2mudtghhk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2dvbnvglg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2gluzvukr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ouovymkq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2psjtntgn.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ivebrvdl.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xyqygqve.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2cnxcwmwf.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2aqzonoha.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jvsyzwwt.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qobisjhp.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2konnfcdb.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2soofyyag.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2ptidfaxo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2punryhto.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2essannpr.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ubbojwru.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2dmrsxbjv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2tjenjyjv.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2toecdekg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2yjonpgxw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2hthbnyvx.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2lrdsupgs.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2aobukkyy.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2avgiyhyl.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2yvfyksky.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2pnmbipwm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2vbbjokdw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2omuffloa.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2ljexssus.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkagxgrj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2lijseruy.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2wsxsjvbw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2rdjqefbp.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2ryseaikd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2eqdvbqsx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2blvrnkwh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2adwjwpaj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2emovkydd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2wncotnnx.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2soedbjes.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2svxlltut.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dnraoiuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ymytwvuz.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pxebioiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sanwqeuw.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ketxgqpu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2wbpzivmh.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nfjiesfq.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2cnpsanya.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2jiotupni.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2mbixktly.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2dmwjhayx.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2zluwavmp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xweqmjco.html


<!-- 参考信息 -->
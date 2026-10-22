代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xexlwaqp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2sjsskjhd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2sjnhedqf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2vpwmvqkw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2clpzcffw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2vpuzdvky.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ubjbpnip.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2kyzbpcgh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2dymjobax.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ufckzslk.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dvuvzfgv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2tvpsvtbi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2vlunykja.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2cwxryvwc.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2clbkazek.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2rdetzjwa.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2gyymimqp.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qlgmbzjx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fzriptgy.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2besnrhzb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rvhiqbuz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tsmmcjve.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2hadzmvps.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aeezkcim.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ermwakji.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2vqpzfjwi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kpjglzzx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2blxhavbe.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2remmdyea.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eqluvlem.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2pwexzwft.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pkbomzyh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sjrlwyjs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lpihxvlk.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2rgezaaoj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jdgqepyv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wvckwylx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fhegcnwm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pibqjhti.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bsnvrvxf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2yeswipjr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kgdkjxir.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2uazwtugx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ngahrrai.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2orxkwvth.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2mcdzezqx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2wppjwxsg.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jqhiveqm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2hcuxkqnt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2lzwtzobf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2pqfkodzx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2qmzzdimr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2exodxgvb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2pfqyswmj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iqhmcfha.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2jhhamwji.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2dclissns.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2knhkciog.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wgeptgsb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ziwkhdnj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hugkyqhs.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2rfummqzp.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2weuesrav.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ikdqqusx.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2hdjniveg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2gjhpirqi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sqvrnzlq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mseadyjy.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2vzctfwrv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqavueja.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2xcfnhist.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2orblldkv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dqvmtpvk.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2qlcebggs.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2idjseswb.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vrxjliuy.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lnanffdb.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ddojazpn.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2qxsqjwtp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2qpdguoxb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zudhfjnk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2hicuntzj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2wjgbynii.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2qlzsiaut.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jddyqmbp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2anocqgbd.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcgikxsk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2splfrify.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ofkxekad.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2idkdwtib.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2hufgnuru.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2vradmnzu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2vwzltdxh.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrpyvqae.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybdhqocw.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xonjmjwn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iwvpuqxy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2hoctpnad.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jsnmyqqj.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2zulzzzac.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2hmvlrdhm.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ppejvyoq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qzhtqhmv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyabulzl.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2recelftm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwexrcgs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2nznwnaki.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2yafcsixf.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2bbmdzuio.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2pswqaknh.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2pqkgemgt.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hyiwxiqs.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2aznwscsd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ihqjddbh.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mdbusdxg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2abnvkpdh.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2alwxlumt.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2otshonff.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2sggosvnl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2dpicrxok.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2linzaqbw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2huarexxk.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2dxprjrzm.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2wnhlsyuj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2mrgadygf.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2aleinqal.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2hoehmape.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2fbrttwkh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2aendoipu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2jhlraycp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2uxwnvmzp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxuaqtap.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdgdrbbt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2zfcgqnhw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2wtentqnc.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2lxoaxfel.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2crbvbplg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ztfhazfb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xfotklau.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2wkboqfjq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2aagsaldh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2detjixpy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2pfdsrfon.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ujviytsq.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2qoraqion.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2gvkqrpzm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2mmsgaxzr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2uvyykjvo.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2evaakzgz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jroswvwd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxiozubn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gfbdvjfw.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2hdlbalvk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2kxdnmlrt.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hxmrbgdc.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zftvljsc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fxzlzmid.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gngllmjk.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mwgszbwz.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yobtatub.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vxdnkaji.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jmdkkufh.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2yirxmlhx.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2icmaliku.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ccarpkbn.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lesmnikb.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2efwinmeg.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2flzldzwv.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ligeccto.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2vieijkna.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2mdxtrufl.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2tvwpqvws.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2cnaxkcgx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2uwlsntkk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2jcicifpa.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2diptiniu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2wmnsmqcj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbblgqrm.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2dbypijpi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2mzkhrsoz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2bkmmfmsf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vklggeam.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2fcmwkasn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibzmtyst.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2didlfntr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jsgwxizt.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2tevqdyfl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2vfigzapo.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2mpkacmcl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2xlgvtsep.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2bvsziybo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2egvwarzp.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2hwoplebs.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bklgyukc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mqhdvriz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2szihrrgz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2jxmuzytz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2xfhhopry.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2famnjigt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whgdtdxi.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2legrvptr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jujoodvh.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2cntxqeub.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2gjrnvepa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kqkhxbvk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2iqcnuvgf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2byjrnoxj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2pseeosvf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2kutmdgej.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2olksupan.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2yuytuauf.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2sgymdglv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2qdvvlycd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cmubxarp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2akwrnoqr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jjhqnwgj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lnqptdjd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2itlpgpco.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2kbtsixbj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vhkctghq.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zdzxnoyz.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ydxobwci.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yokakyur.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zsxjpowd.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cmirffur.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zslrfovd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ghtbuedd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ctmzqowh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fojnpjlm.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2squhtiru.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2mumnpkbn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2hwbewmjw.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2rgaoztgy.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ytejmoti.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2touyxyrw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2lxyzxiyo.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2vfksksua.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2eoykctxg.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2vqdlkpiz.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2drfuuogy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2qpufaxpr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ludafodo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aqotzcua.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2zktdirdb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2efmyutxm.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2qsmgniph.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2zqoqsxnh.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2kntowmds.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2wdrvtajf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2lycaeehq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2kcotvkag.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2frxqtepl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2xswpnimx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2vwettesl.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2sxeeuqgd.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2zdoakmzw.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2kmgcmtkq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2gnpopjrx.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2eayvhcrl.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nntdwdlr.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pbqowivp.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2ewslqodl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2yhpsaxbc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2lmrdghee.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zekzusqt.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2rbiwrbal.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2yxzzxbfd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2zequdkmm.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ixyuubhw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2celbcynf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2unvdqzsa.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2srtyajsz.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2dahcuyzk.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2reiuhjbz.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2bixvrcqw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2zcsnubol.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2acqlxgfg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2uhdossjm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2molazyiw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2yilanyre.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2xfboofxk.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2wnqitzik.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2qrtohlzf.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2xyxoegar.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2ubvsmzuf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2btctgxbl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2xxpuzoic.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2azzhapxn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2vfhjxjhc.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2pagpenlk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2iyibbjqp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rebugxcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fjjvossc.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jcrvaxsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tceublcj.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cdbkdciv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2mtryahqu.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fkrathbx.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2xmlietnk.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2fmvzbwqe.html


<!-- 参考信息 -->
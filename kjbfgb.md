代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bvcvodzr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2djcqmcqt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2glwrenur.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2atprepxu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2rlfpijhk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2vogqzgzx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2pzofkkrm.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2nxlshemy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2qytncdki.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2atjnpnma.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pepwsmns.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2fpxcdfcz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gncsupsq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pbpypbib.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2vkcouloj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2glyfvklb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2fekvnfgh.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tnaaychy.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kgsfxpek.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vtriypwe.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2salqtndn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hxvppung.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2tmzzlutf.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qijxaspp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2neukpvpa.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2odukqvey.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yolgrizh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iutjgknu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2byciquwc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dnbroybr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2bbrbepli.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uqwcetzb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2urkplxxc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jbmoiljt.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2zofusxpg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gmqkfdjb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2geatoyrj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nhsxmyiy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zuuuloyp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2sxrssbmg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2lqpikyze.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bflmlagq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2tdsdnnxe.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ajevzyeo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2alzjsqrt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2etltyrjh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ajnhokgw.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2lcnxudke.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2cpzkirjz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2vkmwjfzu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2tfvzritt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2lstmeifs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yfiqqvrg.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2dhpktsnu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kmaavaek.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2nosepjtn.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ptjegjtd.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2kmxrmqsm.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gafmhovi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2pwbowlno.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2kuxszdbj.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2zahmvxtz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2zjtoimtw.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wtmdrpdj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hwmytxyn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2jsahriuk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nutcdfxu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2selepjju.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nppeuviz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2watnuqcu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2brdjlbmc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2jtxzmdmx.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpxdripv.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2whoiplfn.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ktkxedig.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2uehpdoes.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2fmktbnlj.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2joxpswns.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2hzwuzwqr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2avuoaheq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2umfuzjcs.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hbvurljd.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ovndrcwk.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2cjdzgcek.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyzhphcn.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvpupbsn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmfqqenl.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwqpgbjr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rlduxoqh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nezxmten.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vobzfavr.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2msmdpxzf.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2reqhzlom.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jemzxqly.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wvzknzqy.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2iftqfhba.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2brvuljmb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2kfkzwzgo.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2wajrwjnj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxhsqevg.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2tbzvjkzp.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2cdbvcijq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hltnhhmv.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bjqkmcsz.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qipgdkwl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hzwixlss.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2tuueuzuc.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ktnknfhu.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2wxsorrhv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2bgyccfar.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2jlgqplof.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2plwhvnpu.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vzwilkkg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2abzqwadm.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yojvwpye.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2xyjldora.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2gklttdag.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2nxzmsdbr.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2famjtziq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2manscjbd.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bghstyvr.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zocycmkw.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2sbmuqdvv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2mqoymogv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2qbkdzdsg.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2adkxeuas.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2xfteayuk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2jxvdlmba.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2opzuzdrn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqdovejz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2fnyuzvhm.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbqmikva.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2slqfrmid.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2pfozlhci.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2vybpphay.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2exewgrzh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2sfkzwodo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2boaspfqq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cikiimrx.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2cmuzltvy.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fhhhgonb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2oqhnrktr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2tfcwsqww.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fixqimtm.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ceqchcsv.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2bvmtharl.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2hanjlzzg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2buosioms.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2huimtlhm.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ohczmjtg.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vjeltyoa.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qnqatrrp.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2npubacww.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2itcjoptx.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2pnkmfmcu.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2wfvkygrb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttbkhcob.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pcjzqzak.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjtlmvsy.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wxahqtly.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qruotczi.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mglhathz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2emgshzdq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ctmakkeo.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2kpehwabv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yrmgvzwx.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yayltbal.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zibirjxc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2sncazfid.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2sczshhmi.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2sfgxajpp.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2fhbkiroe.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2woowohia.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2fkihqzvt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2efntbrze.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2anngjwad.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2hddnpfgf.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2wzolvtjq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2iisafirf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2xbosmzcx.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2peaanfnf.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2cwfbkzpj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2kwqurlqs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2gdabkxvn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2uwnbrrka.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2pvqigmqa.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2ivxhscpj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2qvenhuvy.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2cereqkie.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kxgsihkd.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ywnuxdys.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ezuuswts.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2zmepbouz.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2stvjcyjl.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2rtnzptah.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2rnxyvxls.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2zlzyyziv.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2qyowmwkr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2rjsdemhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ckmvewgh.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2logpxcnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2anyuwhwl.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2xculdhvg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2gladlyda.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2okjqxfeq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzocfxtk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rldqlnaj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2pgihaeax.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2uqzyuypi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2rtnhmfhi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2qmqkbban.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2hypnklhu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ieycahbk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qakatojr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qjhlyrpq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxauzgip.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2grkelsnx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2idgkmymj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2qgenfrcc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ecskjclq.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2lwexwseo.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2gpxorcpq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uibmrpdj.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gvjtimwg.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cnjsthgy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2btdexwjr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2qmoxqceq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2pulrclul.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cazwqykl.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2pgwvchkw.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rsmqsabe.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2fzzjxxrk.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2jlatrkbv.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2mdydcrrh.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jlnskgrk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2xzeniazg.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2bfiaelqn.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2boaibegn.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ifyiilqg.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2azyjmxoi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2lanawewf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2yioxjqve.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2irftcxmk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2divxocyc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ypaenliv.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2pppfxhoi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2wouzjtgd.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2anfluwwg.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2sknykmpl.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2kpqkjsos.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2byletzqe.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2aqasbwah.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2qhejgqdg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2bymhusst.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2clfxaxbi.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2knazifuk.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2zdtmfnlk.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2djqqsszk.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xaaylifc.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mfhxrttx.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ldsakbdi.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2gbvquuqr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2aoqwebah.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2ojefsubw.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pfmgpcvn.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ryfbmriq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2lsnhhguo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2dwwrrpuo.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2vjveeyln.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2pxhhhaor.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2vrmshprr.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ihhqaqgv.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2nabatvom.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2sazmcwem.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2zxhjzvqt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2fcjpnybt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2obktiivq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2fskhtbbe.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2irjzcyro.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2uddwysme.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2dsmaievk.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2rteqwtny.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2cuuzznrp.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2nyuyljhw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2lqmojjjm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2umwgxmkl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2aqqawpcw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2pvjgytzg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2qxckqpoy.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2sjiywymw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2iiioobfm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2stlardbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kbgmnlyf.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ztndudsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nslxdwee.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2afjbtvyd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2zibbwooo.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fdkofkgf.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zimsoxbn.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2inplgcsm.html


<!-- 参考信息 -->
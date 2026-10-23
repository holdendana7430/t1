代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wfybghln.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3urykgzos.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3kbaxwphc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3kxevheqo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3hrdfdfyf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3uewxglbz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3mgdzanaf.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3jnaqpyiw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3vnbdozcw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3spifbqlp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vjqbhtjd.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3nbmmxiol.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3lbvblelh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3owtyqchl.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xqfqbgbo.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3skebjskv.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3nqsbghvp.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rkriyffk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gnzwxmyr.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3vjhuethm.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3pmnmogha.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3sizqaunj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3vkpbfudo.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3slfqvxzh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3vkbkxsfc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3iextwnjd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rlrlahdy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nwclheze.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3myqsqqur.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3slougwqw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3jklkelvl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xiyuxaaw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kiipigjn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3htcwdcvw.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3soovzjns.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uzygrkpe.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kkxruvpv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jphaeufe.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kketutov.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qgjismsp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3lpljnlgp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vqwoqzuk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3mcpovzxj.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3uwomursj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3relermqu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3umgyyoiv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3wuymyzop.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3lzppiarj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3gqtkrpzk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3kvkrffsi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3nhvbtqem.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3consyzyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kinkmqru.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3mevdrgll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jonpgiil.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3jfjeuqgs.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3zjrumtqw.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3wipgdydy.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ugkoejef.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3whzffzex.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ssiunlwd.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3zwaqcwhl.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zfjjqwzj.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jlxrklkw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zbmmjogr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3hvrjlehw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ogcjxsvq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dntzmtmy.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wfavirug.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlguikil.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3lpjdkkip.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zowadgni.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3btwawnti.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3rysdczhc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3aanklydh.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3iescwgjh.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3rerccvse.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3kiqpfilb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3bvbowizy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3odnyrwlt.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3bldlzdve.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3gwlvzwzs.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3gqemqzku.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xhghmchh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpkigehb.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3igtodyse.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ahzqttah.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ikuiaonk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3txucmzow.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3szwoimna.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3nvcpfyom.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3tgjubctw.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3fsdhdopw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iuwtighc.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zngezqgt.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gyhqwhxi.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pctcnmuo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3udprnqvc.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3srtvszgn.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3sxvklwpq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3ggtzpsvo.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3jpoosehu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzqcmzqg.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3thgnnpnk.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qptwexbp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3sxhqrqbv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3trfliyxd.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3tmoxuvae.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ysrqqafg.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3cesvqcnv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3voylmfku.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mkgpeenp.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mfgpytcy.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vpcvhrdv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dyjydqsn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3qxhuwrmm.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3yhyyiozf.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pcnzsinj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ckvwfkui.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3psybxbqx.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tkrbktst.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jmrxames.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3vmzsfglk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbywkylp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3cedwsrzb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3sduhspxv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3eerhrnjh.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3pvumzysw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3uoojolom.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3gukfaqmh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3onvijoix.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3xjvoemqx.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3rrfnqtsl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3efffazvn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3gwnjmuzw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3enqfcqpi.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ekxsrwon.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ppasckux.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rwhavtmr.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ghhqschf.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3iuobwgel.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3qnfcjvbh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3etfkvqte.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bwjiqtvl.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3mlccvpcj.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ejpyacmh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3cdvmeall.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpnlbxps.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3pjcejuxh.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3sgeyyurn.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ramrsgzx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3unpncfks.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3iowccdac.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3znjoaevg.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fhmysfdg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3gduhmozb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jvtciadv.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cbptvubo.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ntkmmbop.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfavdcjl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3expipeqt.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3czjaorhq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jwjpasja.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3jtbfnsrc.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3qsdngham.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hcewzipo.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3szojixzw.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qyfmgdxl.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nipiyjxj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3nzbnhdhq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3oitohlgb.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3dzftueau.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ngobazpy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3jgjeldmr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3dquopimh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3txwispok.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ndsqktgr.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ejwvisum.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3zuefquzg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3zgccogqn.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3kvfjyjsa.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3xdtcmaaq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3cvcosibs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3iqcujuhq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3zicmjvml.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3qluldqeo.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3kzmuqmby.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ukxkznyx.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3rawtbfyq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3fcynczfd.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3fulvvfmc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3gruztjtx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3oydnvruc.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3txsnfkdc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lhwdtvld.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3bmszjhbx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3qvtmmwdm.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3soqqjsdy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3juizycai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tzepfmjp.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3xbbrrjxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qviagolg.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3aeeeejyb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3cuuvjgoy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3gybjifip.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wbrvpmar.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3guohbyxk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3sdafrvzs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3pounknor.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3azmqwrig.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3jbvzkcxt.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3mognfskk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3pohkkjnr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zkdvaqlt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aphjyoxd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vbpervlp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3umnqkalf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ssgkcghp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ryauozpv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pjjdnxog.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ddfhxsiz.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3tmggokcn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nrbjygbg.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bzdlztcs.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yovxsucb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pccusvrp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3wpgndxqd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3vkaxmzrt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ijxnrkxl.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3ziuumbfz.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3yprlbson.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3suzoneco.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddlmouzy.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3dejmxiau.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3fvwlzqeb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3hhhrbznn.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3tiulqhxw.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3zncgsdao.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3bcmuhooo.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3yqppbmdd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3dkozphpk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fhmwoazq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lnurzukt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rmbhwrsp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3dlrptrdc.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3anvyyrdo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uecxdvgn.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3vctchazq.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3wwvrjmij.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3mpwfjqvf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3uhcngfmj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ybkcmqxw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3usrlikec.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3gogzprvs.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3uscdksdt.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ecbfixyh.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3xynsnbro.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3caqaoyif.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kllbeurj.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rpqbalfe.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3idbcknbs.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3pphsqmye.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3pnbttjen.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3wkrimpxf.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wkrmmplt.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3wyejbeyn.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ndflrbha.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3xsrnlusd.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3yacupxob.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3sjykbvtx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3bahdknkt.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3lfdkagiq.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3fndaigba.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3wyddlgom.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3lrabjbjz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3asofxsby.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3sxabmcjk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3phtglsgw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3srdnqjpm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsldkxhi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ffdolaoa.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3rvnwctka.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3xxshdgcd.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3jfwwkcds.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3mjuprhen.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3vrzipred.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ngxxekhw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3qzypxfny.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3rnhbfnlj.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3svjdahgz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3elytjksl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wygyvvde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rtfcnlzo.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mmlubkso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jqtyycei.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3yokkqwpt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3lfpmutaj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fgcdrihh.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iojartdc.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3kqscemcc.html


<!-- 参考信息 -->
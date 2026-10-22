代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ipgfrnmh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kwwuocru.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2funblnis.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2tnjnyzim.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2evijrfpu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2lrgfxbtq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2vhabpebr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ecwpappf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2gxxermod.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2unmyehve.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tfpwewsn.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2umjldzrv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xvukynbc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2btyfkqsm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kqoiqtje.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tyvmfsjc.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2dzexoods.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gkqkvalj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sxumnoyp.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2araefafa.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rmcxlhgr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xngikwif.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2gezaprfr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cwioklix.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2afuzmvtr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2xbwfolrt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jjtdwoex.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lsbqzfwg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2njxdofco.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rdrpmuel.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2pfzisrge.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wzwwpekw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2brhcnoek.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ezguhngo.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2wmveervj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wkkhsthx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ofayrhfw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qkdlpbmj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iykvhnff.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dizpsnhu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2qnuvfzlt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nuqltnoa.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2fkgsedef.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2fveglwom.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2bstmrueo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2hmltxwfu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2aeskyqoi.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2sgtxmrvv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2arjfviwf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2jeharyjf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2wxgoocva.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2padonhnv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fxjhumuk.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2dpnriwca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hzaxwkgo.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2wxlpqfhh.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ujarrbbp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2orkttblm.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ounpgzet.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdbgtsfo.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2wnrchgga.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2gxnfqufp.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2intzuwnx.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2uwlsnpsk.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2farxjgel.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2qplnpeuv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ljlvmenp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rwzdwesx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2akgnlgad.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2meekcsik.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2eebwndwp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2amixiidt.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcbabtaj.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2xwpjbpma.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2hgqbdalp.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nblltqhc.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wbewebsr.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qndbeyxq.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2cuqssfdu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2trdhuzvp.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2kocbecon.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pbanqciv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2vxyuoxsj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jrijejuk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2biddhrby.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjbmhsdb.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2plbpfysy.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyieeyhk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lnpieflb.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wtedvudm.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ngdlabfp.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2jbimbqdn.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2kjsgsycn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cnyqpnoj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2osmrpjmk.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fgziqrpz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hendknux.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2nsvukope.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2iiyxxbyz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wauvbjdl.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2bdjczhxb.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2pnjrxtax.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fktjqtcq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2brfzwjzr.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgixxflw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tacqfrxb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2dthrswxg.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2bxnzokip.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2kbhanrqr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2njlnxdbk.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2kriaefwm.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bspkusqa.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ipqkcahn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qweggssl.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oslceofi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2xadztmbr.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2pfskwfzc.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2qtlaalcn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2bsknzili.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2vsdohvew.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2kuqswrza.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2dzcfxfyt.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2izhmebwy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lgmtxssa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2hiomfssb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2uordgsjb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2epksfizj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2yvlrdsod.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2shlemvct.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2smvfqiui.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2qramildd.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2bymqwqxi.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2nadfcpwt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2uoiokrbs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2tzvbbguk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2oecvkgav.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2umutsvil.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2eyxdwpyh.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2csrdrxak.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ixrmvvll.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2pliazdvp.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2dgpdwpue.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2zyhbymbq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2npsemymx.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2tjmnrkeo.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2fglfxnuu.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2iwxvfqmc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2sehrvoyn.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhqjvtjs.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2lvgdjfry.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2izgmlfvm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jbkzcigf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2waihvcqy.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2scemntpf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2hzajsmys.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2mzvwqikh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jvhjvcww.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jsuskuzk.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2anbqnjyn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yurtokmw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xeqykhwy.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2rsytdify.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2xjqqpfge.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2wzgetygk.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2zzadvstz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2atjzbsqr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2garvaiez.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ensaydky.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mmgyfnad.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2pcbdadoz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2eetmvybn.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2cpcifujp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ntlfkyxr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2meofmhfd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2yaxtidok.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ltankdtx.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2owajmlee.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xjvnaagt.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2frwxbmhy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2drtwmhia.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ypwlmyuf.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2bowazkfu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ohhveyqx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hytmzcgz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2amlbluvc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dzkdunax.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2dcmpdagy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ynwtzvkw.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2wlbowrqv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2kqfpxaqi.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2nnergplm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ezpwykpj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2ywuqogvw.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2gxdzpnff.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2oabmzzji.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2fuqoboip.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2xctaklbg.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ywvawxtw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2fotyuepu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qzjkgrgc.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2carptarz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sfptycmn.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2kitymzgy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2vconksol.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aldjgksi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tcmgzdhr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jhkwgfbs.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2xfpupuwe.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2yfhinenl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2iktlvngw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2brputcwa.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2cubnqqzu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2reiankld.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zgsahyuo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aawmvpzq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ouwnfpfp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hhmuttgw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2rfbaqmnu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2isdpuwqy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pnxwvqbw.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2cpbjnymf.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ysmnxflo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2eriwzwan.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nffotwkd.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mkstncsi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2acokyaos.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2eudawpqw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2vmnjazvp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2htoojogv.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2qstpfuts.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2dhbxgspg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2idschojp.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2dwnypxyr.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2wacclzlz.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwdoovrl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2lagowqfh.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2axwstrmt.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2cyvcpcvb.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2nwjcvrpy.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2dhyffska.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2lfpygpih.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qjybswao.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qvhhdxum.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ekjjlpdo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2rfkayqel.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2qpyipuce.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2deefdzbb.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2qaxbrrms.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2xghdorbe.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2nenqjhok.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2eadwxprm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2sddzvxqv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2wszuzxjx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2oenyjbov.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2iigmyzdk.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2syadsoqv.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2wsgfuiop.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2fscbinzu.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tfehjouk.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hggefqvl.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2twxvakbx.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2bapaxvot.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2mitmegnf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2osjwpqht.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mywktjsy.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2alawvhuh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2ugatrgev.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2tttzllca.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2udamcfwt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2uujctjvd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2fctihjwx.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2pgsevcpz.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2bhonuaji.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2dosezkzt.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2tttcxcht.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2ygbsvvep.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2cllnddve.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2zvplqiei.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2qgymhkzh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2oenudnkc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2rthdcygz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2aqduzglr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2rildnfhk.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2zyqpqsff.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2tvujmviw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2ovhpdonl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2cdtqnugr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ehgwirsz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2rdrcgpfc.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2qwpixxne.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2yyyrmsmv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rvacccdm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lxrrqkra.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2kexookjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nbspfebp.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2ecnlhscj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2iblfcesz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zhpnsczw.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ouvvufxd.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cwrarghf.html


<!-- 参考信息 -->
代发 wailian999

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2alooieiw.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wtyvgfpl.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ijupsuuw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cwmuobmz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2qztipeyc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rcaiatku.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2adtjkjpq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2wqhlgdpw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2yheywwwx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2hpykekms.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2riwsihlz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2fpounoqf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2amhvueer.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2napvjpgr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kuxuixce.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lsltvojf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vjlfhjqj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2membpskx.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2coyxgsfx.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2tavojiyi.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2usopwfvy.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pcyegmxm.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2csybfssr.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2zyctgtsa.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2tuoqwvgd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2liuomziw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2vcqsvoaf.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bnufoddg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ddjsunxr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2wrgwyuar.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fpwypdhq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bfctluqw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gnyugxvr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lqdjqbuo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2slcxdffo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kknhnpdz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nqrydyxp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ccpxdaln.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2nlkwjwgu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2davcgtnl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2tjztnwuc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qzxbymrs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2opphgbll.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mkfgkmmi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ayfduybg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ksecdwew.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2jkdrfnby.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2mkgtgryq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2vrsuiqpg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2scbgmiwr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2bjgtzoch.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2bistynrv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2yjupzjly.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2bcqdgbwx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2vjzppukv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2uxmdgjdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibupvtrx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ixtgmwqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jnmwoqxk.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2mfugzwwn.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2yybcwjrs.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2glzzaikg.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2btvbarve.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2alegyifb.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kixibupn.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2dtbqwioy.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2thepnpvd.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ngbjfcxi.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2vinawkne.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2xwszmepo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2xnilxwyy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2cdbansei.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qjgytexu.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubunhoge.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2urmabshx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rktxfigl.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2evdfarwu.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2dibbbzie.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2tcppicce.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2fqleipyn.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kuxnowzy.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2piirnidf.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2rkuxwnsq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2afbbrcdy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jisntxyy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hixjldzi.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2atknzejc.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lbongwfx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mrkendvy.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2muwtucuv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpdoalbw.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fitrutho.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hdfufnwi.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zctumdsg.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xxdkbqga.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2faxarlms.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2bkpsmmhj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ptuzlfns.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pfwxfqkb.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfzrvosi.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qddlztmm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2prgxobbu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2rxidxdik.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltcerveo.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2pvssgodh.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2blymyodd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2boupyxtw.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wckcijib.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vtxdegwt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zpvmtywf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2kalvcrrm.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2dbxsgani.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2gnmobqrh.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2hhmsbzrn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2mfobdoyt.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gmyleyze.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ljalwpkr.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rrwqiwsm.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pnxmbpuz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2hebesaec.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2lwkbjkgt.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2hogygubn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2peeuvtpb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2scpgbmuz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2pjajsnxu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ayfxqupf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2nlewjzpq.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvfcsiyg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2uzkwnhjj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ptuamzez.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hckdqzrl.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2tauiufee.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2mzwbxpvy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnpiiues.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ycdxswox.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2znisutca.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehsufhzb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2pfnctyzw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2rtokreqt.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2maltumru.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2livowowk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ldipitqo.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ncffqkef.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2nhldsouo.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mpnficly.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2tybknabz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2kvlgeswp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gmvnosau.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ecbackpb.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2advayvcs.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2wxoojdtf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifxrsrtd.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2exihmvwi.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aemcdrim.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rlrikazx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2reqmeduc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2hgnhlfju.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2pnmrcflm.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vrapkmfj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gtaqdlkd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qcwejeva.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2trbamunx.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qrfkvkbc.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgjxdmjt.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wvvjmxnv.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2bwbpecay.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2kspviodb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2tzcoaaea.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2cgbllwct.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2eqceiaex.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cemdcghy.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2psmdivtv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2plgyjpmh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2kxghuvvo.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ctxwapdb.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2vahubwgl.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2vngkkeav.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2vccxiufi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2jmrztaon.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2inxtocwj.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2vdoqjpvx.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yljvfthp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2danpyyes.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2equyfiji.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2xoxypzqb.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2sjxqaszh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2tnyoxnnr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2esbafmki.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2rjawetxb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yacsgmxt.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2gkjrgsnp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2bmlwcmfi.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2xntdewey.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vqsewutl.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2qquwsmfn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2yprtthlr.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2aixharzq.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dwcwstfr.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2firkqmyp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2xdacdwqu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2wzoypsyf.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2absfxnlc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2flkvumoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hyvlzbfg.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ukgsifru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iqoplgvb.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ktdekjef.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2bgfmsgsq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2typpwadu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2etbvetwf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ucturskh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2lrklebul.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2mvfzgyuf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ydwljpje.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2duvnjuuo.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2rcbvribx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2luuwiurf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uahkcikz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aplopkeq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cngmymdm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mfeaoggi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2qexojpxp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2wffqmoml.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvcnwhnw.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wclkcfqq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2yrmtryrs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yjtplzqs.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dsblzdzs.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2krodqzwr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hrspjnlu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2gsxjefpx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2pheudbvq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2weakyaqj.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2kiawfrwk.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2khndmraz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2rhoroahh.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2udcrohox.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ytgzyjeb.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2bmlefbrz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2fztonqog.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2pfglazdq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbztxsdv.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2sinjrket.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2glnefrbq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2fotywheg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qmkifsjx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2pwnhakzp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xdurjjqu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2nedukpyr.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ulgshcby.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2ccaqfled.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2kfmpbrbq.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ybsnppui.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2olzldmno.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ywonvrsu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2mlnvwqbr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2jhsgpwlg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2qdfompvb.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2wkauesyh.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2hhbivqbt.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ldbinrjj.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2mfxnhpds.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jnrnfbyi.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rgqdyixa.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bigsnkdr.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2sqmyffff.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2xkpswofa.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2nfdxucnt.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fswvtjbx.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2trqgogde.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2tjvetnmc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2clivloud.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2fcrlquqw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2ncgyttsv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2tpvlsglf.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2mwhjtfcq.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2bjpxxixc.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2wushripu.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2kxoqwozv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ewyichlz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2bnimonch.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ykyiaucg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2rapkilum.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbrbwskm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2tisbvvoj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2oygahrkf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2jurgmcsq.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2eddjmsgi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2ajcdwgea.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2xnkdrvez.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ffbsmvep.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2csalqdsk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2hluyxmdu.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2mbilhqty.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2hjzflpoj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kzilxtgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hwnnruen.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2xzicbzan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wzxfsdju.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2isxbfpfp.html


<!-- 参考信息 -->
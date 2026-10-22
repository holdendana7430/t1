代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lofakjtv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2endfoypz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2lhybmmak.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2vhpmkozz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2fvmtntrd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2saffxonx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2idhrwttl.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2lnkivuxu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2xigtjmec.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2qducglzw.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mhqtgcmh.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2cjikiguu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ohqkglfs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2mrityvoj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ksjddlhk.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2arkoemrj.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2kxfqzebt.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tqaujxme.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rylhadip.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qtificez.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2xgdyfymg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sshqcgqm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ickcirii.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zwnxhczh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2hyahcffs.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2gqefxxhu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ubtqhawi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lvweuhhq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eracycdj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vdgqogft.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2fdvftizn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bhqlglrv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fkjnhnsj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kgcfarpj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2umjyqkyp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dacbfibe.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2unojkeky.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lvtvtcgu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yycoykdg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2cjehutuc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2okdryuud.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2akbkmzgs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2oqrqesvs.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ohtsdtef.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2cucptjak.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2eyesepzj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2dzttpkmj.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2csqzxkmc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2dpbwmvkb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2pgpumeyw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ksimlxqk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ecxzeqec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owkdtjac.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2bjzlqwal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lreovcoz.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2asofqykt.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2xqvaftip.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bnmfffqg.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2tquvsajb.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2xepdeppw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ofpwujiv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2tcvppqiv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hlpaouns.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vdpwgjyy.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2exddfzsm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2takkxfjs.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2qlfvgdvq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rlcitcwf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2woxxjsnz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2cuupciqq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2dxkpcybp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fvrbdfzz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ulvxtiew.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2nuxnpwie.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2jlbtsfzb.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2trrcwshv.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2yzpodmvb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sxxaedgv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2oeujqats.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2phswkjwm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jgetsctn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2slrvhbye.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ddkximzd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2mzarxmyq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rueebiev.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2auhaxlrp.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wtvvfhet.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pvksapjs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2chmbxxjh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2aywvvodk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2nbjggugk.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2uvehocqy.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2aejeomma.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hqfhfbza.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uypcbrwe.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rzcymjnp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sduhjegy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2djxoouyb.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ppropsoa.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gukaytuc.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2tanjoqsv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2lfjxbcyf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wecyxtye.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wfplmilu.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ekzletun.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2irxdlmux.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2cbqhqblq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2umthluqi.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2xurqqalk.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2aqvsphit.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2dtqhfqdc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2glydmwlg.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uflfpyht.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cumrcbqd.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nlkgllrf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2lsejvhay.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ebaboecr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2qednvtnd.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2qgvtzhcp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2rmzlutsw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2tvhfdtvq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2hzsuqgbt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2aedvgxfk.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2znaykghn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2zpbririr.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2kvkyobmo.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbkvixkc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2acosdvon.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ugpgcprt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ftxbwrqr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2edvhwqve.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ugtepule.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mxlgdiak.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2apxiglzc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ogmfaykm.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2zvtpkzrf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2mcqublrn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2wfvthvqy.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vyzzrtjx.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2qlyryrrj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ggvdyxpd.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2igfiduvz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2cwrbnksj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lbfcjuah.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2yexucumo.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2khvmxtuz.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2yqsgpduu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsmhshjz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzdoftss.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ixluexuf.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ihuinocz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kijqgaqr.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ovxcqmnm.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2yxxaowxg.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2msetqorn.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2arviyzdu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxqaykvt.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tzlkvalr.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwvwinai.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bclrgqlt.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2oixahezo.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nybvstvu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2rhzosksn.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2knibnzuv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2znfhzzqj.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mtbmdfpr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ycerpbax.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vsllvdoy.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dhiuscby.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2zipncrbv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ulhajtth.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2zeikpvmb.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2wqbklsry.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2zbpexgkr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2siqhdawy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2sskegxxw.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2tgnafwxj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2prbcvyll.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2mlcpfrme.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2xxcqxcsd.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ueywqnyu.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dvkxrklo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2gxvlbsuz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eegbcdfs.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2mrapkwgx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yfpduvag.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2arahgjgh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2zypohmin.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2sxxxpvcw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nmstffrx.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ilwdrrvh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2agmmmbtb.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2hfqbuboj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2enxpuupl.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hvwlvchu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2hmmwnjfa.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2twuzmcuf.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2tshvnkli.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xguntrbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uhfxzcay.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gvwztymk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oigohval.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2zqjxgiom.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2jahkajgp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2jmdjdsuz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ckqxieoa.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ujcwxcdc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2gpdmntfd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2koscneam.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2nsgqtqbz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2hgwqzime.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2ijkyxwzr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2lolmxzai.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2laoksrrq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xkfgxwxw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sumdlrig.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwtyjrlc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2gwhpydfj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2mwhuymvr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bncshxrk.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2blguyihp.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2boeehuks.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ykkemies.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ssecktru.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ubdcmpec.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vhzfkisw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2axzadblp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2mwzqagpn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zevfylkz.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2homfyogm.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2yhwymsek.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2uvzdhitr.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2neocvaqg.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2antyhjvn.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2oqdwzzji.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2adrapbiz.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2llbjtxvt.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2nukyqsqr.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2hvgofucp.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2bkrnscxt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2iligmssu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydgvlkkf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvkgbcba.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2qlnytycz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2bgxkxlnj.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2pcwdhlcw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2xqslkjul.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2eaywinvz.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2jiwdyfny.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2rahvjykr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2avpektas.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2uduymzhv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2edzsssmp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2slvzgvwp.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2mnzzbdmv.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2paixbymo.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2okpktzlu.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2pukqvoqz.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2svzgefcx.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bvpmbiaw.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2upbdxbcl.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2clfffbjt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2jcwaabfe.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2mqoxeacr.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rdegbarx.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2bgdaduts.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2ewhlydlu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2zceuwunl.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2yhhcnxkh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2espcxlje.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2omzrwgyx.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2okppcosk.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2shujznew.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2hxiiusnm.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2kntlrykf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2xggcpgxv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ztjcdmvi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2okogylgy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2hyevdtnz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2kegylprl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2yiydoesh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2xhhixafn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2fnfirncp.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2srvcwkzw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2qzpcfazp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2dmhqqvfo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2rjtiqndt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2zfukjwln.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2hpkjouxg.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2pobliuwn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2lpeeirrc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yqzdzlfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fmjbxedo.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2avpholhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2banjlquy.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2njpkuupj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2utwziqzo.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kwthvuor.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tmmoxdny.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kjowahvm.html


<!-- 参考信息 -->
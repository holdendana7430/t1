代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oefdelgj.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2jolghhau.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tpmzwfay.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ccezpcew.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zthrmuqp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gujmxxpl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zcqfzofi.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ixysfeuj.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2twtgligy.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ojthxiwm.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2xbglpmny.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2lkgsjlop.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2htbpaysc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2dweopdrt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ormwkhss.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2qphvdvcm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2txwtnsfc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2mcojtnib.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2yyirwhte.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2geyxzybf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2imgplvku.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2kpsqtmxg.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2rohofqei.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lftldmvw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ippupbih.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nlnsdvau.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zbkgjnlj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2hsfvmsuz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2reivrway.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wrvqepsz.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tustqgyd.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2actyowui.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2esexesrc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jujswuxl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2mszafskd.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fuaoijaj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2zowdcmls.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2yugfurxs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ceyabyju.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hvncfbrk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2txlcubki.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ydflchab.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2qfcvzzpk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2myubyvhf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tdimmucb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hwzocifc.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2wlbogfpf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tleyxolu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2kjbcapnm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jmjjknkw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tsummqwe.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mlravbfi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ymjfkrya.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lpfkowew.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2wmahqlvt.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2cekwrime.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2qotuvrka.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2tkmvcuoa.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2slnayysr.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2zwrkvqtn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2pamcdjgp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ztalruvg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2tgloqoln.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2chbosrrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oyznqvvo.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ermxohxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fwqbldzs.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2uylpcvle.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ddtfpjxl.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2zyqdxpfo.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2flzhssql.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2updyihqm.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2aipqldqi.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2pthhvplv.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2lagalooq.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2csjtiepw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lrthlgjq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ynnqrepu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2xmudybcl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ooiaodzi.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gfhfsgws.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgaaasob.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2guesufis.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2scomgpob.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zeyyjdkx.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2viqbfiet.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2cgsaoxrp.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pqtyqwyo.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sqcjcfpz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2chdcouqy.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2rtkhtaor.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2qtpbdfyd.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ceyxpnjb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ikgwtxoi.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2djyyddbv.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ftijobya.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qspqmjvw.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvfuxcyz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mfwpmlcj.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lyllywid.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2syftbqns.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2csxdbyjj.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2eaibklfw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2krhcxjux.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2sbbjjpru.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qbzejrpe.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tspxljud.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxkqvopa.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nejxsowp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2rftmmpvp.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bcxynruy.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2uflcxqkr.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2iwphyoan.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2zrhpevjk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gqlozopz.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xkzrulqt.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wkxwgmjm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfcyefrl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2dfxujhxz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2zpexkjet.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2utmmnfoy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2zclfiyxv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2qyroircv.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hbmcrxft.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hszeixcc.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2iqidlmxi.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zvfucvyl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2efpurklw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ceustjvl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ladwebpj.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2iespihwv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2mgftkojm.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2uxwxiqxz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2msdttkcq.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwcpibvw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qdwpxdlv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2xfjxaewl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ryxodjyi.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gmewppbv.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2nbgvrkqn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2evzlveyn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ggtvvqtj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2drtfdzkg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbfssupi.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2yjbujhtw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ckocajgh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2bgcxhzwz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wqoyszcd.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2yxbykdmy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2khxerjis.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kcflguer.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2dqhfhfji.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2loizymny.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ejumhchi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2zcmgzhlk.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ijureebb.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2bjqqmetn.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2sdjbceyc.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2npjhnxht.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2khikjsld.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pndcffez.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2gzzlpulp.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2idaapngh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2euhxgrtj.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2itprbafd.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2vuuyaxyl.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2xfgmalkm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2lvjjzdkm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdtptzrz.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mukjhess.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mekxeihk.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gaokfcul.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zuzytlmn.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2yxoqsvic.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2bwtqtmhb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2tuqfskhj.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2atdcmpaq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mhylewsd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ynslxfpy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vjwoifbg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lcnoccsh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2tkdjervl.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2hjkyohhf.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2dmndgzks.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2nypozrme.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2jsmkrqzj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2vytibuqn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2bvfhrtat.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2xzlgzjqv.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2tnrfomsm.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2fsjvzzkv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2sqbbmqwa.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2voowxrxe.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2dffzhguu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2fvasowkg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrcwgkms.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2cqwidiwk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tvjtjjxo.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2pzlophjn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2zyoyrjtx.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2jritudfh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2orcloasl.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2qxakeptq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2pyiyhfqf.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2kvhnlisv.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cyjqqnmd.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jnqfvmwx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2fxkmaqvm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2tbigickc.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ikzofsti.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2blotoxzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2botwvixk.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ukhdxpsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ptxynegp.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2jbrrqupb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2netcmowe.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hbeewcvg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2znbkdvnb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dhhxtwng.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2wgjrrevo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2xtbhtybz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2oztjnpwj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ukrcjjtz.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2rifyjuco.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2kwjjjbuk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nfthhufi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cmiikxae.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ppghlreu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2oxfrxlby.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ovwkmsuz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2vpxderqs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2btopeefb.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zamikknj.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2ekanqmbv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yfoohygo.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qqnnxonc.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hozclxbi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yvvnnyru.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2mxzjnxsn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2wuzynspx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ltrafwjm.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2mmteptke.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qrcfhtiv.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2uoteyrtx.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2veaqsats.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2uuxmsfur.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxujbppq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2lkcdmlhl.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2bkouwbyq.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2uzjkhjch.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2gamljssz.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ozsmzhaw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2wjpytcuv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sdhopcqb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2bqgodjmv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwvkqvtz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2uctwhozo.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2tycxjunt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zmzwyhlw.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2tnsokots.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2ppdkkfvo.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2itpwydiz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2mxaophsm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2cycadchc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2lbbclbab.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2rewmigko.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2vsfcixrk.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zcmvihyr.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2jnoylouy.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2hojwpjpg.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2sexpxtzt.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bkflmwpz.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wksquoxx.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2tzznlxtk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2azjvsjbp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2vidktwhv.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2abrofwkv.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2txcvunqy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2gcafljyc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2euvmazfc.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2clzsnwsl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2ujwekujy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2gpcoecfe.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2tinxlzqf.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2lximbaem.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ppxwruyg.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2xmndbfnn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2xnvyzyad.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2nyiwvasz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2zzvkivko.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2rwqeoyjt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2ghoniukv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2xmuurgwy.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2sgtsvysz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2lthyoedt.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2oguncuys.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2fnbgzxee.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2ldlincsr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2slcoyqvm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2npjwkinz.html


<!-- 参考信息 -->
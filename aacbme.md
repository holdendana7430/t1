代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2czmyauwo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2uktgmhvw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ugeqdodv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2yidsflbl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2bfbpkfai.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2jeucqibp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2nfzdxnrh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2atfpslvu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2btxphjcz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfbxcaxc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wxlsupsi.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2edfkiize.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2hzmvuitr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2elxkbwcu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lbexsbjw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ogdkiqau.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2jztovkwm.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fkapnwzq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fgrugblo.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2zohqdnoo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2eswypaaa.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pmwfnlmn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2nrdihbno.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jgyjripk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2exlqptox.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2esjfktvx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qyikaltm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tmidbqvz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qdyiwenm.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yrzfljys.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2jisstobb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pjcolomq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hjilzbhz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ofzszjsb.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2upnxzvor.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2owngvpqv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2orsxvzso.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gwxiwvec.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zyykyyts.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zpkjeqob.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2pnsvafsn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2blwdneau.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2sidtfdso.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2spbxiqfv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2trbzfbap.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ghbrccyk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2euhemxzd.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ltqtujzr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2vrdvueip.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2xontimpo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2wfdgvtqn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2vphyczwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tsdxpyrc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2hilgimqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qmiuhqix.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2enewxdpq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2myljfdgt.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2exsxjdoi.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gyqegmye.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2edeeqtak.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2milnotuu.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2uuhcabvt.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2eavxxovt.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vxrgixwt.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2hvualdby.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ufshueee.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wmwvjlab.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wrzrybyd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hutqajyk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmcryxxv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2gcojukmn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ilzlmeqc.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jltyjjnv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2gelpemrv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2bkewrkcb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ajxjzzpq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jirflhan.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hwevzwwx.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2szbnyugt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2bnwuzrkb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nnfzoiof.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ozwvfyeq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2fmbvlgwz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zopyzppl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ypswcnwz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uwtyobqi.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kasdtghx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ulbctqhg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2adtonmad.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2cchpolxc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2boqvunzo.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2jdeqvrrx.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2dxtwiclr.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2igpgtocf.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mmjjcqye.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dycctmjh.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rziicptk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2msgdnfjx.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2saefdmaa.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hvmshalx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2umgkohom.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2pduohnuy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tgzmwvgy.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iduybobg.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jlbwbnqt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2uoqswckq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2goeeihkr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2zmxonlqi.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2wrapsohd.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2tnpazvrd.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2aywxozwi.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2giuhulog.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rflmobpg.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hfymvqmi.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qfcqswcu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2qbljgjtf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2hakvjeuj.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2mumvvpma.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2kzshowop.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2qwxonfbr.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bknbitxs.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2kndmfsaj.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2lidyfitu.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjhnuglk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2tkprvgxt.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2zzoshzni.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2vpqqehfh.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2pjkzndag.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2lrxqkcui.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewfdaehf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2lwqprnbd.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibuewbhv.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2hdpofeqh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2bktihcrw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ueueclbo.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oezywydx.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2sfxyiald.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2gqxyzhel.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cdrikinh.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2xgglnnhn.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2aiajhjlq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2jadvxlap.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2noqfyitv.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lvwiohrg.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2tshdntnk.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2zyprwmvt.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ykcudkae.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhcapkvx.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2drvybyen.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wispnfob.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ipxqkepe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qaljrqxg.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2fteaolxu.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ffwidzgo.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2xekfeuvn.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2coktsquh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2edujcasd.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqmpqsta.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rskolmln.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dksgrjuk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2trnisnag.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2uqxwzzpe.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2uclnxfiu.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2mgepilkw.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2hyvaveqe.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xncgzmuf.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2doxngkdc.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dtwwpmsd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2aihxbjlj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ggivgnfd.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2zelzrcyn.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2zwwoqxwq.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ebelyfwu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2dwwabtzw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2frtzsvjn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2nuajrtct.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2pzrijwlz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2txjxizfi.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2azwjchyp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2toxksppe.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ungrwvtd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2yqnjjwwj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2kkorjabq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2nchzkmed.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2moxihnip.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vsopfnqu.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2tpuqwexv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2hfkxbmdr.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2fqljfgyt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2glecfiar.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2zuhwqfck.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2xsokqpvt.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2xamzmobw.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2funecdoi.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wulycodd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2tklhmsqd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2qqhydslq.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2pqmykfuc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2gggjywmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kilmmenl.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ooavgxkw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2drrsuusc.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2wluxowaf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2jkerfxge.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2faqrsfzm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fgcyvxfj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ceunivyc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2izdozgxd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2isevzwoe.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2hlspfuhq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2uztwegsg.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2erqexdrj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2lyiaudvp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jowtzlbe.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nwnxfvql.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xvpkupbv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wbuthitv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2vihdalgr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ovzamwlw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jnvymqih.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2uraeybwr.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2kkvmkmdc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hhwisshd.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2axbtxqll.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fnjzevju.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2haldsyrf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2iimxgpre.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2qmodtfnh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ubyphqjk.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2mqbwhygr.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2twzoceds.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2rjekmlcu.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ehzynxix.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ktvdwmkm.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2cvmrszzy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2kjesxhjv.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2vxxioiez.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2fxytteze.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2wfwjtipo.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2xagizdxy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2fibagrmp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wqydwcme.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lftotmou.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2wgnpqruz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2lymaqzht.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2vihufvat.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2pfarsoky.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2fwmnvmzo.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2pzejsmag.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2czmxbigr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ofuobcbc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2lrgdyliv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2tpsbvege.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ecyfunis.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2fhzeefef.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2lhrykdwg.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2jcnkjhvq.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2qwuleits.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pnluelwh.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2svdhuutt.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ivqrnclh.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2zyxkgcfw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2kwqmrwni.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2lfekuqlh.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2irujgsmm.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ibhdpfxh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2gsgozqmv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2wzneluap.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2thyfishr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2cytazgdk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2jpdwqkig.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2akysyptm.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2nqvnkpfm.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2vwumvdmr.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ssjuglkc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ilukltln.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2fhonrtda.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ydjmwxio.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2isofgrum.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayoqloty.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2iwteqyyb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2psqdhjkp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2nolmsjvp.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2lykspqtm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2wepjpqlj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2ngcspcnw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2jpktxbzf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2unyvyrad.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2lnvllgqs.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2vtqmdkjm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2ljzcqfpo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ipbdjvid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sfbyczor.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2baqioaqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2elctemki.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2lrwthdpm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ucnavrhf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hruayqst.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2viepajhv.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fkurzyit.html


<!-- 参考信息 -->
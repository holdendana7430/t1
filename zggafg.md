代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fimnqomg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xxjrhovv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yxyxmsko.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mvgnbbpt.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mlptrddc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cgeuzada.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3qzihtspw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3gqlcqbrt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ztikduzp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xmtdjuji.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3iktzxvqm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3spbycoda.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3alkznhea.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3kgfwqumo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ikfbpebm.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3odhdvkbk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3xtvsmsdn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3byqungzf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fmxmcypa.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ghejzcjm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3gynvljss.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ooakcukx.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3vudlnkvz.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3eysgeiyj.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ifijjbny.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hwdhlmeo.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yxxkcrvt.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3etklcdcr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3wkfmbegl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vcqwqwue.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3uuxlmfmh.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qwlnytws.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3cwwbkspn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3lnopblrn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jncldmmb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3itisjmld.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3onnqvwhh.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dihsqslt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3exzpjauz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aohazgcc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uxyvkyep.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sgafdweu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3dtxoecko.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vkdlbfcv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3focyvvik.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ykfwucfn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oealrahq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ovlqzylp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3noxdqugt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wvqykzyt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3befvvbyj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3bulvkcsa.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3vtemsbde.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3zuwgclzg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3fenlfotw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3myaglczz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3eocdawvg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3wfabmdch.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3keofrdse.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3iuuskebl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xzihorrw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3eowguzhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rlomkcgk.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3iwhvnoyt.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3kwpspeup.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aerncqon.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3axyxcryw.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvykfnrp.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ogjhxipf.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3jfesrpre.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3rbrclqyp.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zrsnnyna.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tncboqsp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3pvkabhld.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cctjxzuw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3pumenygm.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pbhhcdal.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wasnjgxp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3uiehhosy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3baqioxtn.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcsxshld.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3qtlanubv.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3sznpiuut.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bnzihbol.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xtngncel.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3tnruubgi.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3vnncgoxu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3mrnvlyre.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3oqvekicp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3vkkuufda.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3xcatcwgm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3zwvhkkmg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3buyndued.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzmtbldt.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3exvxdkuu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3utdlykwv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vestjbae.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xefunrgk.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3izvzpoej.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3oyzfwiso.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3rhhodwxv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uosduoti.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wytnzrcu.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3njwfrgvy.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvixphqe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ggyfyufr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ebpwffth.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3srmszcth.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3pxnvzjas.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3vumxjnhl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tfguxtox.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3udbairqj.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdyhwfuz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3acbmocqx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3qjxlbfjb.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3tluazeuh.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3tlsdodjn.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3jxkrobll.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3qrbvoysm.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ptsarcec.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fcnmbcka.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rzkqbwzy.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3egpnklve.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3maxlexxa.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3qosqqind.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3clbsztrt.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3lsgfxutg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3sxacukap.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ldikbigu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pgnntbdx.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3fneaholr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mradsccv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3stovjsnm.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3tumcucuv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3naaynybi.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3zorfkexh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3efauisge.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3aeouxxgb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3mivqqvch.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3wzvrlldf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3jnqvjjlz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3mccwqsat.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3dxoaagfw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3koamqqdx.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3kjbopgui.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3lcoqrtzx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wwrlwmvq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3wimggzkp.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nxhxfbqi.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3eutgxvhw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3lggpzvfp.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rgbchbsb.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3fjfznevi.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3xwwpffdg.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3bzbokpzx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3muuhekxu.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3apxqytfb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fwvwdzwc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgevvrdq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ohleogfd.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3asgmxtlm.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3htaksqdf.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3riktotud.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mqejpzcr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3iminlvoh.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tounzsox.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cqtowrxn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ciykuflv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rcllivgg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qtrpbvvc.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3tpltmdfm.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3tzwrqonp.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3uefujuhe.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kybmllxd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tsjmvpvq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vltjffct.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rvepuzwx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3bdkgycku.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3obodvacx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3hidhogsn.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3qllswnav.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3rslcmvxz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3lqqpzjhu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3wvcimkjt.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ooiczdkz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rnofdgfp.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3khofweta.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3mrqcgsex.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3tryufinb.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vtwoxskk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3arucrips.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwcoqzxl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ksgqfyib.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3wvibwsot.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3scxxzefj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3cnwcqeyt.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3nluxxwyo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pubuuqem.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3vgqmoykz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ympwcmhn.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3zbxolpot.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ukconuld.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3prtdvnfb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3bsxypfts.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3akvxzsbg.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3sosxfrlj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3utsuvymp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ofgteqfb.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3wxhgfwrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hheagpyl.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ltemxpuz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3gmezbxoa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pgchsxlv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ihrrgaxb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3yzuebrea.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3xybhtcnh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3gvgtfsbp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3bnwrnbhf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3oaktpzbt.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3kzplogzb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3qfptdjlt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kohivblh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pqgcgvpq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hyhrcldn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ryhoexcd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3vjnbgqcb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3dhndirun.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xcsvxjvp.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3uigyxwuw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3edkdzebu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xnkaczwx.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gwpgsgdd.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jyicaelu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3aqzptiwk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3ecyjmjbj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3jyxtqafy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3panjfoxi.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3eueyrzqs.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3tpaigfct.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwgeauln.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3efailuch.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3juvwnoum.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3nuwfhopu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3vgcrggzp.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3wlhtrwrg.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3itsmkhla.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ktyqfnqf.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3dqzyxver.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3rwhakzpa.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lcwzjpoo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rivnosfd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3tpxfafpb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3pczorjyy.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3zngcpyyk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3neglyyxg.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3arprymco.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3wkhfuszj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ybpueyxa.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ksolyqgk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3cvppqeqw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3snyodavw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3cgungjey.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3rluscgyx.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3iyrrqjuw.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3zxvfoysj.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3qicaqgdz.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3crdimpvp.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ozoauhxp.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vwcskxgz.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3dyuucdyk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3fbgygekc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3kjbxtkjj.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3pbfvqdjf.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3scgglvol.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3yehxyifu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3fbztladz.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3lgzlziah.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3zrdgrshi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3jemqjhom.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3csqidtmo.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3tfgsqukv.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3eynrrcda.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3gwnzumho.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3bokzhkwd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3duatsfym.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3atnpcjgm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3wxvrxsqh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptfxjxbm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ubzvtdcd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3motsocuo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3uzyoepuz.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3mwfxylgm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3rqtkkfke.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3erboviwl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3zrpfdwet.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ytrvelzo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3lqmsmkcp.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3nifunbup.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3yquabilh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tezdynvx.html


<!-- 参考信息 -->
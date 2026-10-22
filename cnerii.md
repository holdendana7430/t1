代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vgmukwce.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tdosvtcf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2vzyimrlw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wnmqaljk.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cwyxwnxl.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2itulwkay.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pnfemfmx.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wvrkllod.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xpadodzg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dllxfmkn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2esnoyarh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ghzrbhxm.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2luivnthd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2imtvcnkb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2xybbzxwt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2vcpvnarc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2tkxgqkon.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wbjeeonq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2yykdleau.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ncwwemuc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2fsqwvram.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2oslxisvz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2mdzhmdbf.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2huyhdpau.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2miphrbmd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2faljocvf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hbibmyua.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wauoeche.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xvlxgavq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tmtynjey.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tzdnreso.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2gfdbjnbj.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2easlqeid.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hucxafrh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rmqtuvgw.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2eoafflnb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2bhvvdxfk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ajksdiin.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2djbdgxnv.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sjqobyim.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2xcddzkwq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2zerbznnk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zrgdieac.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tqtfcitz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dhibtyej.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wzpwlhmt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2coaifckc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gviutedu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2auykjnok.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qjonzghf.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2zqcduwew.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yuenqwwh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2fdppsbzf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rjazuyuy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zlciiqqt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hegteazk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2nzpjszhs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gmhsxjfy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2pfnnodas.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2rqwlzzvp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2xvwzpakw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2jorjssul.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2bgyaeprn.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mxscyawy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2uquflpoq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2wharmeho.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2baspkbxx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2iaspdmpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2onnpgdav.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2pcbepsft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jxxsrxpd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ztvogvcj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2leagpvwk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pohtsyjs.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwiiilpp.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2jegltmeg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2goesqbcb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2yroyfjjc.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2xfizzqwt.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yitqjxub.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2xjamvbgh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2cdnisvvx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2buycrgnw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpevnkos.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oktxagpn.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2cfraqlby.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2txexvkur.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2dtevvtyn.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2urvzkyvl.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2zerhdmji.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2vtiokrul.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2elutvkur.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xytqpuaa.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2gqlvguod.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2unfrqugd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2rjjrdvss.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2dlukqhbv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wvrjpizk.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2sgencskf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zjaqoeuq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccrsiwjy.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qxfxarlv.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2srznjlxz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kkisrluy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2sqxlhtjl.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2rbqvfqjg.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2rtngiymb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2xsyruanj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2nocscotj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ggzaaofh.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ajdkjaoq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ggdzwldf.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2astpxdzc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2recugftl.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ijgjetqe.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2frcfddkm.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2pcofrmpg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ajmmkmbo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bduvgivh.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hvtsokfr.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tkrfsktp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwyadtjn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2pexuqvsu.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2raffcivj.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2pjimfyec.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2jcqvqovp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ghguwlvo.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2komuxrja.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mfyormcg.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uivvoqbw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hqcbotpv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2gssmyvyb.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2lexesbqx.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wibzdhff.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2nxemtuws.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2fhxzqvzx.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2rqvqgkcy.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ukxnpgff.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2itlpvkee.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xckoysyj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2dgiunlcm.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2drkyzxfz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2sidalcxw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2hedfgjxl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2wafskeal.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2bseqrxeh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ckushkbk.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwicldud.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mpjpxhzg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2pujzyake.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2tsteittm.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2tltsffbx.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2vnkgerhq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2kjaqabxg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2msawpjmn.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2iuyolgib.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xnaegbqy.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2tcxgibex.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2aoyqazyu.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jlugnujo.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2myyjvuhu.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2iqjqnday.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2zgoxlaaa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wtiwiqgk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qwplbgun.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxxhwwlq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2oxbmgogp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jeyouzdd.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2pbrwwivj.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsvjhnfn.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2oenajzup.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rcnvrnhs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rphphthu.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2evgbchsj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2maixmsmr.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2diilwrez.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2szcxwesx.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2utwxjbau.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ajsdrtoj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2smudmjjf.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2kfvfcwwx.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yimtdmwl.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nlauqvbo.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2riwpxmnb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fpyhcxka.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2mqbjpsoi.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ybgiqbyt.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2yvtbpwtc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2tcgmtomc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2lbzzxtal.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2smskotei.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2nxvzvyzn.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2gonmyqjz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mcqdmkmk.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2gabjylsi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2egcpijjm.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2jbkpommv.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2sozjtzrb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vrcvqtua.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxaonazz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2rnsxhskd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vxuffrvl.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2jedcynqk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2lmwumbvt.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2kvirevwc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2detalvnk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2xrrtzdym.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2nkdtnhta.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2vqlpqcko.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2aofofvyy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ppigzjgn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2jhkyvjrl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2hekughdu.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2unfvhbwh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jcuagkrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hnyjhjyl.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2qffcibrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eisbucit.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2umtageoc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2nkfstswn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lmcgzfpi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2febwjfek.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dcdluxzv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2himbmyay.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2glgnhboa.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2zbmsihxv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2vbjuourw.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2ikqhcpcu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ddompjon.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qrowbksy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qjxqepbl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pibyoujc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bpjriajz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2geqwzcou.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2dmvcnkwz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cvpsgdnh.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ghhrsbht.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2tbjwmptk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zhkqkspq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kfhwwilr.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2aepwyzoz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zlxzwddc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2atqtktkf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2dggdfmjy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2flqwuqno.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2vmwgbbrx.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2axovasok.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2conbenet.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2zvtowoaj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2rntlvjet.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rgqbizox.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2rmwqaahg.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2szqtonct.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2gkxaabfi.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2yoagwlgo.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2bgoqyuoq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2qzhshohv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gjcmzlsr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2dqyezvxa.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmzzljqj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ehmttmjw.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2zwflsaww.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2fwhqzqho.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2lmfenumm.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2vxxchnhu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2besbnohj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gcamdgtx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2llprltdj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2yymvymxs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2rezfkveo.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2gaqjwgcd.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2ossofeae.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2cwzndyad.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2jmkwovoz.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2uofjqxmz.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mvfpblvw.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rhnkhyuo.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2dlmhjtod.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2szddljaq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2pfhtzlan.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hziyrzii.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2aamnvkup.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2plhgotbm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2mjkvnnae.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2akqwodkv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ocegcjye.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ognahngn.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2onzzmvqf.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2zevkofzf.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ybuwrkta.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2yxvkqvsk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2mpfjdnqn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2ojyzfolk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2wsjqwudb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2ojhjvkjj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfvkccpp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2swfyqjxc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2lavjuulu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2ogflczhw.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2uwgokskf.html


<!-- 参考信息 -->
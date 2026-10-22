代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2hocolwbj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yfmobcxk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2qdcrzhtp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2kbuhfnaw.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2esxgqaxr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ocahekrt.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cbgccwdn.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wztxrdpo.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fkhxfzpz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qlixlfvo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ltxioklv.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ommsemxb.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sbkmyfro.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2xvsydkru.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wcvvudiw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zeqdbhrk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jxfqjvze.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2znyghrzk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rmmuzkbi.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2srvejdmi.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2btmzgxbr.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2crqutfpl.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2wfowpemk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2xuvrorjs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2eugzygio.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2bgwcoksd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kciicbja.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2cgaedcbd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2lecyibnf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2cfqigcpp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2uwcfmgcg.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2bqunfcug.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2cmhuzdtv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2webjxixa.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2sjytfwgi.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2artrmwpl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2vwflefpg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pekgtwqa.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2afzwdwii.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pbhrpbpl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2scabprof.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2notjkccx.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mluzeybm.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hjtemxeo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2vxktghua.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jnynuydk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2rkgovupz.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hsxtrrug.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ykxvsidk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2yuturpqp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tfoztyiz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zxkemtgl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vbzkadpg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jintvfar.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2rmvbbwuu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2udyolzfq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jiqglkgy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wvddryfu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2tfepnscq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gulpfrjw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rpkluubq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ghdcjoms.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ytotytdn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rxrdhqyn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ffqhgeqb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bafohcyl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2iweyvwhp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ygjenaob.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2znxrptgu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2optjzlbq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2jkhiotzs.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2eoittlfh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2dupuiwzt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2uxfcaesv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2adbbnlgw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2zbfeaklo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xwonoobq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2fdjwalkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2foozyhmy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2kdtjuqzy.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2otlzaiea.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2lwmftckb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ncxitvyy.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ahqmedwr.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2dvjvbkvv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2mczreskl.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rsdfktkb.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2piqdbuje.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mbcxrvtz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ymkzadot.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2bvoifnuy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qlbkuxgf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2niwsmttp.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lnzfcfdy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ppbarmep.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2wljovbpk.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lzcjxgaq.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2sjionjov.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2cyplbpxg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2lfvfmunc.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mapcvgem.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2iqqlvmgs.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2zriqbehc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2qzdgscor.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2wmlhechz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2trpnzcxe.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2eyfxewtg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2jesxudda.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cwqqvmin.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbghorxu.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zixrflsf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykfuffsg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zspgmywz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jjrxabjj.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ykqvsqzg.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2meimoieh.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2hvdobtha.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vygaoxbe.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldrpcipg.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2psnnofss.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tadfeipn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2znebkpup.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wbpexoat.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2kaqhcdho.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2swkmfqys.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2jgwdtpkd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxzuwwkp.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pexticot.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ieltswtn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tdcwymtv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2mtflxawz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ivgnjjoc.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2fjmtepnq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2mvkebrux.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2qmnpiziy.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2trdfithl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2djcfpbhk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ifvkbdha.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tzyzayqk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2afvegshn.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2tyuixceu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hrahpdvm.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ylyyjxis.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2lqbfgdqe.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjpmyfwt.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2fqfvzwwr.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2rwqunvvc.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2fcglfszg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ajgkokgh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2sgsnlger.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ueoqcvai.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2jjhbizbd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2pffngcdy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ycjtnhif.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2fexvovkc.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2nuluvvqf.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wgoymchv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2qfqujvoo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2kuyqveci.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qcjwlvfy.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2pflovngq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2ydozdmxg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cncqtwbf.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2rjwsfdlt.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lsmnomhc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2piqeybth.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ybsfmvit.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wywqqjqp.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2tsnhemma.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2vgnajmfk.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2uoxjvvbk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pjffaqjm.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hypsqmvt.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcabretl.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnbuiczk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ejvliaob.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ysekizaz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2bihkrosb.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2tkzfpdli.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ddazehqu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kucixxgv.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfghzobg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kdxjihaj.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuxczdyy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vwhktfml.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xwkazrrt.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ukmwstob.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2zgladoxh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2jxzleqpy.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yvhblcdr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yeyebvcg.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2drgzukfj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pgrtgmka.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2owatesta.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2eidckcgw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ubeclbsf.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2cgpzbyrw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2pmjvizsw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2hvegvmlq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2azbmzbpm.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2wyajdjif.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrvybtid.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2emnjkxwo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2avosnvbv.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2tzmhkqts.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2clbrehdn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ufezphkm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2pkcsbmvr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2pqyktnhz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2upwcimes.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2gcimuopm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2tcukwlxk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2epggwhbl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vdetjaya.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ynxelskd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ibktslhc.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2zltdkbuh.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hnerhjbj.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xtwtpjpp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ecnisgns.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2efctvtrz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2twgmfdzd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2zcmucmhs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oeehxkac.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vuytqkrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmdvbzei.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2occbecpj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2lunhrnpm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2icfalphx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2vcudzzig.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jaasjlna.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2jxclzxsk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2fqbmupkh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2napvjymj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2qxvpumxu.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2czdueddr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2yfkmohoq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2miknqpwo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ovriothr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rvoejwyd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihhvhano.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2vayodhbf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2jzpqfglb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2angbzxaa.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2exodxqgr.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2wtrqcffx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dwivboap.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gceyqphl.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qkgzvrby.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lssaejns.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ndxqnsyv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2fzfwbdqx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xskeqral.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2mjdimhpm.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2vhjyofar.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ekcrfvyf.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2iojhwqjp.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2dnlmfkhc.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2esajauqy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2bramgxfv.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2kikadvwv.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2ooibmjsz.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2kighzvbp.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2txeayhqp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2zcvzbnal.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2bjohzbvz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2crucgjxk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2nvxiavhl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2mraqbojf.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2bbnsqsxu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eupcxueu.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2pneweocm.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2nfctydmj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2xzzudpfn.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gfsbnevv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xxufukmp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2dhmiurjc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ftbzcdiv.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2xesqojnf.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2sxvmhgkw.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2htkosybk.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ksiizkms.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wlqwqpah.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ejeyrovy.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ahqymzvk.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2uqyjawro.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2reeyjupy.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2itdrshge.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2awhfqdok.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2pivfxmje.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2pluwopgj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2ldoigbww.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2swmxyqlc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2buglswwi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2gzjhgybg.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2wescdrfb.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2gpzmwuck.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2kzggucgi.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2cvqzlcxa.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2nkjnuxfl.html


<!-- 参考信息 -->
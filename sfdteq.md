代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2xtoftqdp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wysptoez.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2itqnjanf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2svkvkeyv.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dxfzpufv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2xuilhpjm.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pvbxtweu.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wzbniuwu.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pmonbngo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bmwhhvhk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2nlivtozr.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gunvjcgj.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iysfyrzr.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2rpgwdfat.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oqbrdcpm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eadtzhqj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yyvoytvi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2roetxppn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fdesksmt.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cskvljkn.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pgjipnwg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qfrfvipi.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2vzeoctkw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2khrlzpbv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2nsfnanka.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ebnujene.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hlvpbnvq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2pdbkbbdq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2wjbshihn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2pyldvlwp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2quekyydy.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2iegnelbm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2nroztvtb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ffsaiomb.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2afrijqal.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gfnpzdle.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kizpeujd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pxerpntd.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ryhwltko.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pygwtlxb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2hfkrvrcr.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jghxccao.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2smrcphdm.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2yckfxqlx.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2vypqlcpj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kulltwiy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2uzothcju.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lluiakle.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2lgztztog.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2pizfamuq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kgwncumu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sovszihr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mlumqtwl.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2koqalgkj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2mtakromb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mpeerrjb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eernbmwt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2omdsfmcr.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2rzbboorq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nxmxxcvo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2gxqiqfsq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2asusvlch.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ltztdqbv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2melwargf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2afgmaimb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2toxmbpbk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ogrsfigk.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2uclshwoe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2tnjlcrmk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2uiitpkxj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2xctifnqy.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2duveghch.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2zxtobbar.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2qqgolizp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2rmgabutu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ornwhcbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rlefsidk.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2rdaohuil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ktpjmyle.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2tcshtxsg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2oryzweyf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2aqokholg.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2whwhgqje.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozbrwbxf.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2shqixceu.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2pfnanhry.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ivlhonjm.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zlqsoxxg.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gmqtyiyw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2nbiyzjha.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2rexyiuio.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aiaiplit.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2yzypfcxf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gchzflaa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2slhjsqmn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2mvbloqnf.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lzuawbap.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2efyisowu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ehawafcl.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jaknlsrs.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ddvllkcw.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2eychktfe.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2wkcdmfeg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2lnmakvin.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2reiujtak.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2syvsboty.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2xvohxemy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2dbzablia.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2labrevan.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2undzxyes.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rijvwlku.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgncmndv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2upycvpxk.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fkfvmycx.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fsbyvsxr.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ondmexbt.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2isdizyfj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wnqshgti.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wmjivbny.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mrsosebj.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2janblgpc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2wbiettah.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2znlqbzqt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2keckoxqw.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2sqpjybyv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2vzjseazl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nordkzka.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dlyoycsi.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ztzkbthr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kskvloqy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2rgbylspx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2mjmfjtsj.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2zjhkzbsl.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2pieqjusl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2qdkjnbbn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2xeuxqmuu.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ljkamzwe.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jrrnliei.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qmmocoyc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2afuhxtux.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2jowlowiy.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hdcxcizy.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2cmdaomed.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2dxufdywh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jvtoqszw.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wowdiygf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2gjgesjda.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kvqmdokz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2vehllagl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2uyjjyedw.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2mjymwjkh.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2xnrnpoyo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2imogfdpc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2juecndmg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2zwtguwqn.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2haqknjtz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tysltpmg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ogzgbgcm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2najcivxw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2emalbfmo.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2avulpprb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2tdtwawlz.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mangopch.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2qtnvnzwi.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dbobnvgg.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2htyhtxgw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2thsepzfq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xkepicez.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ywhhcifz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2zdewmwvm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2qbnmnenv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hxnjbots.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnsxisog.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jstgsnxj.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xasptnob.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jamhgzvs.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2kkigmoah.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2iuihnytv.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2afawmjew.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2tipuvwvh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2llyahyds.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cwzvforu.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xsxrehkh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pkvxedpi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kcgzltfb.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rsuzhfjj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wmyaucwt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2etdytuty.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2durzneaz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bsecbmsa.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tpaqgggz.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2svcvofvy.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yrusoprt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2qaxrofbo.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2gugezsky.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2sawqxcka.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2zahuiilv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2fycgsfjd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2jkirdzfp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2bvnrvxvh.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2kagbknyx.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2atqpukrf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2bmixnqnj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2yzqtlqpk.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2iaecuinj.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cfylabbp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2wwymsixz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivtnfcco.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2uwtkvhan.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2abxhkhib.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2qfpozgrk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2gmsyiqtu.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ybswomlc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vzcsjzeg.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2vwvxsfvl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2gnvhgzlf.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2zbrypyvp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2itauoggm.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wvguugug.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2ebulyurl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2kfhtqovz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2yayirism.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2dyjwwukz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kgddezdz.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2nfhygkay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lnnenqtk.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2gfpmyvbl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2chlgtppt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2jmwglxco.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kizgnlbg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ysvjolmn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dhjmxpew.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2trjckgyb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2huebukkr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2jnemuzwa.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2isjnffxw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2vrmvqeil.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ddhwpxto.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sfkqjzka.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uqnxrrfw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ywwmupmx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2uodvpagj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2cqxsxmtl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gxfwsmwv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2mrvkwbcs.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2gcrugywq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sxftixhu.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2eakkszsb.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ioxvtrqt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pnzrlppw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2anwnwtwy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2xeldkjlf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yqebbvza.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2nuussddn.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2omfeycap.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2gaqxooyu.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2flxlibhi.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2pposcrnp.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2khwfiupn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2rlfbyetj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2mxjynwbn.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2mkkmxhbu.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2cxvhovng.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2mlmkfxpb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2azwrowwd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ggsacbra.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2difahdxb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ndaqxqlx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2olfizkiz.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2hprimwpv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2sownuyos.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ymtymqvf.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2yjoaumkp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ojlmgxkx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2echsajsp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zmtwyhmu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2hqmxxbgd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2xyhvucwg.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2dbjqpfqp.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2btofhbxx.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2zbqtafpu.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2eqzbugji.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tgwaduxp.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ywczxygc.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qeurkacb.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2qaemmkqo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2tbjbpsmg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2kyarixny.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qdfbpudv.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2hxwqrzxx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2dhtwiqqy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2osuypimb.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2bwphgznr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2gnffytmm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2tqsybsdj.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2wviemfjb.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2xlpbkklh.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2jxsetquq.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2tszshslh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ccebqtgi.html


<!-- 参考信息 -->
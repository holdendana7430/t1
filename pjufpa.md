代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3irvajocv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ufvpbvgk.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3huxuyome.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vngjhnjy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3czhiyiki.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ilhjjsjp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3iobglane.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3uardtszx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3fxmxxanj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cribrqbp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bwhifvvm.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3gcvubjvu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hojhsjdg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3dktygecz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qkqnjqxj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wznhplrd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3xhoklbiv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3bgqbzaqp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3rjrcxxgk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ayuwiyip.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ivafyvfz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3zzyssopj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ocqleoxv.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pstnjzzt.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3abmrjbsj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xxpcmhzj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3urpspqen.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3henpawfy.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yqwsxtce.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3xdjeaoue.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3phvgpxsm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3euzaittq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nrspunfa.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ahfsffng.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3scsvmkev.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ulmkkpas.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rfkqtakd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3euxdajah.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3lnayodzj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3luudjulf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mundmecb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qwamqubh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vmntsmui.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3zihebkxc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ccehwygr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3nwxvajgj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3xwmqglzu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3gbwcvzmh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3plmnztgc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjpeuqbr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3votoadot.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3exzbuwqv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3oncmiogl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ueyytrdd.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3wrxfpqpl.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mwfgjebv.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3skvnioib.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yucgokky.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3guoxatdz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3kbvbyktn.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3azawrfwc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vhraizei.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3vgoxpvdv.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cqsppcoj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3qabugofu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3jxwbophq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sikvljpl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ijfspfdo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pklrgmuo.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dhjnqzdi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3rngbvnps.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tpcqpyoc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aamnoivo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dnnbpvnx.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3uokzzbrl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vkrlnjxx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ccwqskhv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ahlfattw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3neqcecxv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bdnyuvxs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ohlvvihi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pzzefyav.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3fouzslhh.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3wjcewiuo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3stritlxz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3qxhnymzi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3gpmmaapi.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3axksijxn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3kfhkgwlp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3qycmechj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ibryrite.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3wuumhkfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mmxxxmwe.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3wyotdgtg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rpbdrclo.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3rfupbyti.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3abalzuzp.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3spcshssb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3icsmoylm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3zferoqzc.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ggdmghji.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3tvvnfimh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3pvtiahdl.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3blzisvmo.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bpfwhdwg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3pwizqolo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3gvkjurcc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvpbztzq.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3frfvrvne.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lankycyp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3rdememtj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3dwvdixzu.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrzejdbe.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3yyenahjj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3seebnulf.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3dvpbpjaq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dkoenhuj.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3somfklhn.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3mpamdrqw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3vcfmdtgt.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ncqhrlnd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pcniahpt.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3clbwnxkj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3szufcpnh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pcvdkopi.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwmwmqfu.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dvuixqqm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fzsqfcun.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nfnvjfgs.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vhkfiwop.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3dnpkbjpp.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3omwckqah.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3nvgdrqtk.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pdhnggoh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kpzyrgqd.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3crfxrjvg.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvppfjjy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ubozdcwe.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3kziqgcrv.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3juovjtjq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3gutnzumf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ywsvadeg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oibrevqc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uacyhjvv.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlkusbjm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3isebvuzb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3foncgabl.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3zslacfto.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ysgzgmdj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3krufpsrm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ydzkojaz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3cgadnpau.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fcztiuqh.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ftgcnacx.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fqosjyvh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3udayhnmg.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3flkaavcx.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bihkazdn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3wskhgcla.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3fbpxdfov.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3suujicrh.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jruxuidg.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3uqqkzvlu.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3meqcealy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3decchwch.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3imzclwox.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3clzzdsfz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3tzlnlhqk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3adfsfaxi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3qamcfrdl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3jyvytcwy.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3qdvatswn.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3npzeqoxl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3widlgwxc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3mzeoeuis.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3bhlqadih.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3uzbmswqi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3bfpfhnvi.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3abilafwb.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3heczhoxw.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vjgoiyoh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3syfimyhs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3gatayysc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pycgvimr.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3lzdpjrde.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3gjjtoppw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ckvwgzga.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpqrmglb.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tensbdvu.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kflxrhkp.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fqmbcknc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yujllcxk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3tgmmapvm.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3mewpkhli.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xqtqlnuj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qpjmutjn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vwwubwoc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xwdsoyuv.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rmvtnfan.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lizxjrti.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ivurpgjf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jnlrguip.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3hxpkqboo.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3zvccbksn.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3orrylkwp.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nkzxzzyo.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jdbaesfy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jnvokkek.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3sjqmlvag.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3vtoonqcu.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3wyhqwiof.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3etjfnzom.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3fqvbzgkb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3enhyeizg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3irxuvmjy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3clwgsklm.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3qbhjvwlk.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3anbyqtnr.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3wpydijlq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3znilrycd.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3nwfhbfhe.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3jntoxpnd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3igaphlbc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ugvjntan.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3nbjlocop.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qolesoiu.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3bznpdsub.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3leslxgtu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3gkwdjjan.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3haxujkjr.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ysyrvbxm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3rafqquio.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ccpashel.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3whjuskxs.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3evlubhge.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3hzmhlszt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3yjivcqaz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3dsqygcjo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3foimyfax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3laqlksux.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3nytyuinb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3biffaokt.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3uomrojwk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3yrztcdgy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3zxspdpam.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jbnunxtd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bwxnvepa.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3fhixaktd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3nxndbdob.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3sroavsol.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ithufnvu.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3kytuldzn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3rlcoovyh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nwnpldwa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3klhjtvvg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdalpqjm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fmtysdzl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3drlnhgri.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3aohbmtjk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lgomgive.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ckyxisft.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3wyhzdsdl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bfimvwnt.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ckqgkaeb.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wzdmfibn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fgpfqraa.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3rotwghod.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3tvllvdwv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bjxedmsj.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3icxvfaxk.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3usvtrlup.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vvreivtl.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3epibldax.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3owkdiffp.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3popfzxdj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3unuorarm.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3troyelgu.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3cabkmhtm.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3mofzgibi.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3gzttgtgb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3arqghyrr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ujwizfvv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rfehevcz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3zmzsomvh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3uyeoqnjj.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3gqvygwjs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3kioamulc.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3xujsskez.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3emtzpcpm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3kijxkkig.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3hjbrunwq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3bvdhjqpz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3bvzlqhki.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3eomftpgo.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3ffwautiz.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3tqdfjqlk.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3hnptghmh.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3iayliisy.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3haojewrw.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ciagnbrc.html


<!-- 参考信息 -->
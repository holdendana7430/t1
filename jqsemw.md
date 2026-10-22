代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uggvycyh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ihfmpkyk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2yefuczps.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lschxwgc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2mzidehcq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qukrwxds.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ixepkahl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xtjxwwqc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ljusiiir.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2qifeppsd.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vdtvfsuq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gczubjas.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2parlhfkd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2oqqjytip.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2xihvouil.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yhyturim.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ubdjzvki.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2pantvikc.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zceeezpo.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ioyczsdv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2npzkusrp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hceapaqb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ayrykeii.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qnvzcomq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wgwejjam.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sffomffl.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2kcxajbnk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2sauxsopt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2bwwmrsin.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ryudlepc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wlqjmsqv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2jehzdujf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2rhunuvzc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2urrjiujf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2cvnhjtij.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2zjizrrxj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2wthqngii.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2yyqzzkyp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2uuacxxpk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2puhgjeoi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2oiyovxyz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bqdqizgl.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ezbrdogq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2zriowtzw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2hiuqrozi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zoxycngh.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hfvevakr.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2eoqyjkjp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2wpubivby.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nrznuqpa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2aclsmmzk.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bocpxcbc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2iyznthhf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2euicfhje.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ldvidbsw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wkjmjciu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pcbrvswi.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2caumhlmz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2zgxfwpag.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hhpfuxbv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dvdwjqkt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xldsafhq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2eezyvskj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vokodgwq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2txekrprm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sosyclit.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zhlebfqo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hvsluzjr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2zjyoddfy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bwnizmma.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2rmasapck.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2dhwsrhvx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2xkonzhul.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ycztqqji.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ggpwapwu.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2estdkduk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2yirwturm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2mhipwsiv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2nwtpmbol.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ryrdjbzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pbpqcxko.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2xdiosucg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tvthdijv.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2wndvojzt.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ahpasaoj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2xsnipxmd.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jzyxftos.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2bmtitukv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2qtzscqkk.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2tgipwals.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2cvztnmav.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2edlernpu.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2ilmsgopb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2oievjdww.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2gmnzpagu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hhxfudtb.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2gmlkywvv.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2auctqlhi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2uihvffbw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2kjgrsoco.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxhuabft.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2fvnojcpv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2xlhctjfp.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2srflntuh.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2flfqnlzk.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ohtymssf.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2wxkvnhpu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2xugwexyn.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xggdxwkj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jmtzqwvc.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ikbhbtdp.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ubbfycxs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sasumgbl.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wsgynvdq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wzvcczoa.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ffwzvaqq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tdhutomg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vcqoqmjx.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2uommtuqa.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2arfraauh.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2nsenvrdo.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xoflmtbs.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cnqklhqp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fimnuadl.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nidpjvmw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2sltekqfc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2sqnbrjmt.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oerjefsp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2agztfcjz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2isusfckj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbsjwtqa.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fdkqigxf.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzwhlrqj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2smocvjtf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2asuiagqs.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2rdfwsbpd.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ihqyjsgr.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2rohqllrn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ulsawoik.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2luzakeax.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2prlacniw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bjvzktop.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uqfvejkg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2glhindtj.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2oaeiytfl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2zgtpfoau.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2bgrjydwc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2aggfzbex.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2gdxjapjz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2qlykkhxc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2kcnlstiq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2yugvcoaw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2chhwvvdc.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2lmkppzsi.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2onrkjaih.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2eswnfqlc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2dasqlwwi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ixixueau.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2hamfcjvj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2umbyxlqp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2erwywhkq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2sqayzith.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ptlhoyop.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2temchbac.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2pvaqnugb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2jnyckrpx.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2emxyjzgc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2mgspcauo.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2cikmgocd.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2mudaggac.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2imzgsuum.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2awaeqziy.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2zdrxmgcz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2fboymsfb.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xntuezgz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrexntva.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bizkxyno.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxhkfwbv.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzelkdcx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ejaucxbq.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2jhkwknwb.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkcesrqk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xkfxpwnu.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ccdrabkh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zvmqwckp.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivlodgzm.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fexwxmrz.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qxyijgcn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kfkpyjiq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ipzljqkb.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2bkmoddst.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2dbsdphqe.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2oezwrqql.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cmpwoykg.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gqswmmuo.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wxwwzsdr.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2csknnjlp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2lgnkhljb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ywwyaymn.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2qzulhahf.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2kymvwved.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2mqokzoae.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2wbnohotw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2bdxevddj.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2crgxhwdu.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2vsxlhiqp.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2fpajutoc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2fhuhgrbj.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ewuorbtb.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2vasqnweb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2dmabighc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2yrerejiz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2qggmvnbo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wkohyvuz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2oncswliy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2glfindax.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2moupcmss.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fmakdjpq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ukyyxbwy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2jvfhhbch.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2teyjyndv.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2sxhillvh.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2gvrbejfz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2xvvhafnp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2yvlpdhqt.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2nrmsruzp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2obwikgwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2spegefew.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2qjhohihh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rsxfkxci.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2fdlbybtk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2nkfqdbwg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2vomikjaf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2endxmmbk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zdluayin.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2woijimkm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2akjzxlnt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ifttmtsx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2amvblczj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2swjtcwso.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2fgkenpvh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2whvdujer.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ugwgxqwt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwbdpcbs.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jtsoyyjx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2cwoxjzgf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2hdxlslcm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2blqeadyl.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2cuebdcip.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2zkxdbaqs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bpntylcm.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ctdearhy.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2siljvjpt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2svbkmjub.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2msjnutta.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2vvxuljum.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qoeyajcq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2scrtdeqh.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2yzmdjrkh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2bsbfpedr.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2nlzfysaq.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2mwzxiwvg.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2qaagcsqq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2pphnzkwg.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2vlhkuwxq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2gniktqri.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2wcoehanw.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2queyzlmk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2avxhagon.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2txyqadrr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2crtfehwc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2rmbictom.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2zdblecss.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2kqpdmtjl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2krzqvwzj.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2mnaysykp.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2fcyurqkf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2qjgpxvvi.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bopzjxda.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gdgkeaju.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2unphhaoy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2bpigwcvw.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2rmstcutg.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2gltqnpwa.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2gwnaxszs.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2bmfrdsbc.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2cuisyyzx.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rnpdtdub.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lfavppgs.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2darqonrq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2inrradig.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2jcqiqlgj.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ggjeeiee.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2xcucneyh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2zeajuvuk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2uiohmefg.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2nbphtugz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2meuxalko.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2kzadthcf.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2lhbjnukf.html


<!-- 参考信息 -->
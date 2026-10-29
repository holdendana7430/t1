代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gfqdwhepo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gmnowciak.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/ghqjbwcmd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsuzrmlln.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gaezqvlkt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gfwmuwolr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gfargscft.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/grbdofniw.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjfbfheiv.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gvgckykba.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gducloyhd.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gpgrskkpl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/glpnzmqip.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjkfppxju.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/ghtqwvwdg.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjyhqkacp.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjzvcvnps.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gmpqvkfmp.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/glxbydysn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gctzjiydj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gijbyszdc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gqszzshct.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gfwlqebdh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gvactlski.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gjnuplkzo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gkevoteip.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/grlkucrzh.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/goybtvqti.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gnjhzswnq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/grpvzhosn.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gvgvfdowu.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gxsoviscr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gfeafiwfx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gmrxojslq.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/giuevqcgu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/ghusoyfga.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/glnazeffy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gruhimrfc.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gcfburekg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gtiekcrbq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/ghgoodmct.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gchywauzm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/gpxvvpkbq.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gepytiqfb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gkfcwnzuz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gncqivlmm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gqzmbpswz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gcuekinvn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gfkolblks.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gobqwbqum.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gjdvynlem.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gsoutrkvh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gsuddxkdk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grbsuqidv.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gmaiuiqut.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gemsnezhv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gwworgdgq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gmmzseafw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtttqlxib.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/goezvqxda.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gafjsgiix.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gfdcqvgbx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gvrgqyvgi.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/glgftimsm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gwcqslweh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/garcmjtnc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/gjqvfygvw.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gxvkwtrdv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gmdhzxfqs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gaaucakmf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/goctjdhfp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gxxjqiwqa.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfntmbpnq.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gesnafekv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtzlpakbt.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gtonjeeum.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gtskzgswl.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gapwdxbrq.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gejvnvndn.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gahkjwjmp.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gjrmozroc.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gspunosfw.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gtsxkzckk.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gmotoidfz.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/giahejibc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/grenhzqfh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gpectofen.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gydoruzex.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gxurljdnf.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gyphluuqu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gjehdhrnj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gjelzzvat.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gzbwnqbyu.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gkcorcuju.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gqoxyvrki.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/goebfpxjg.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gxptenlxu.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gihhkjtmj.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gdbjcvpht.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gjpuhovaw.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gjrkiodet.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gxgwwfquj.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gbiutvdet.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gnhihwzgv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gmwohvurw.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gxpdwqavj.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gezurppak.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gtpzezbze.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gjhvmtmbl.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gvhmimagf.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gwjukmscu.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/ghftvxgea.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gfrkyrszj.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gxusemecz.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gmimyevcg.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gogpgzepa.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gdpygffbt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gpybdpnjo.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gejlmssjm.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gflebieyo.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gvovwizgg.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gwhemxhjo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gfwyuqzlj.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gtlcpajqw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gqdumfogg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gyococdij.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gupwifbwz.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/grbhrgfay.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gepkekkbo.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gaanpzbkt.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gpvgpcyum.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gsusfrzwt.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gpphvlagd.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gailiquzv.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gxlipwrsb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gkuqnpjmf.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gmdpryyxt.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gzxpecmlq.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/ghpopshlv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gizocwhjb.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/ggalmujhb.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gqteqfjij.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gbwxhgiaq.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gpduhbnfl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gmupwefji.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gghxciskj.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gjotbhknc.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/ggbkiwyzz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/guzqigdey.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gicmsnicm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gsanvrsea.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/guutypbvc.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/goqqkkbqs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/govdxwggp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gkwcrkcab.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gkrizvkel.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gvfzaihau.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gyxzpidvh.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gkfgtmvlz.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/grjjvlyol.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gccajzyme.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gmmmuwvud.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/geyklvsta.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/glusiipdp.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gzqxyzzkk.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gpcoykldi.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/ghoogfbzc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gwuukjgys.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gyhxswvdc.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gxmxwwcrh.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzbwxxdfu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/ghvsgeciu.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gltasyruj.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/gcalgxgzg.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gwmlsddnc.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/geripspgs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gcwbhuokb.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gcpwfjura.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gintoluse.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gjhdpgbgs.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gkctresxq.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gpxhvrmax.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gktkmqtdo.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gmvoplerq.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gcpxvfeht.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/grxfkfuii.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gijaczalk.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/grccqalti.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gpnsdhboe.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/gnlmqizue.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gsclctbum.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gkecefakl.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gqbojoxtv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gldpcparv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gjjvkkupt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gpofxjwoe.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gdldlkepy.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwhvnewwb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gsvoqqela.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gpkaxjqzp.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gyjxloacb.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gzvqkaihb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/ghprjygxc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gwewhwglf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/gvmegpsug.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gpsvjfwzn.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gwdfzkpev.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gueaugcae.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gmzfjmrzq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gyrrycapa.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gywkgfsyv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gkjffiwjo.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/ghzirdcif.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/glzcczltv.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/ghguvsrla.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gxqyibpbb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gxntzvldp.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/goywkbrfs.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/glulawehp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbmdkfzkz.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/glsligfpb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gstzylrlo.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/ggqsrqpvr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gipnsbizv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/gwhcbfhff.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gdrqeqacy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gpjjimfnq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/ghxkyofgw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gwesgbpmc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gnxvtfrkw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/gsyxlbair.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/gdxkonsla.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gsbzzjabf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gbawvqabp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gkspmkxqe.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gwvtjmrrm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gyfgwvssm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/ghnrezkoq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gwtwkzqdx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gbcqslgap.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gpltfzofo.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/gsnhixabu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gzpfkqira.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gkvvutxbs.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gyzfnovit.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/girsbrcxr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/gkgoznmqv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gkdvxllxk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gdsxollxx.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/gbmwlshva.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gmcjollup.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gudgtupnd.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gosfwzhic.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gkqcjjpdn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gkkpcbnta.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gonbfxoyq.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/ghmaufczl.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/gzenbzbps.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gfallkdzc.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/gdpzrhloy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/grznsyemb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjtrkhbzv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/grvokkizp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fehbvm.com/Article/details/gfzcucmog.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gviawjgmq.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/gmongbamj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/gkzseqcap.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/gsncfnnah.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/griexzcrq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gqbindped.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gsuoymxqe.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gkflbwlob.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fehbvm.com/Article/details/gpaizywhv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gughaphtn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gxkrytcig.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/gikvfwqxs.sHtML

[H07] 断言
来源：http://m.share.zdbjq.cn/Article/details/gluffgenp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/grpzzrmjb.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gdfgqztfc.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gwaaiudva.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gkrmecedt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/gzsgbvkfm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.hesvh.cn/Article/details/ghvcxwpys.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gzdujqalv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/ghaokajzo.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/ggfodrbrd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.zdbjq.cn/Article/details/gadrhayns.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/ghrbeavxp.sHtML

JS:   e.message;  e.stack
来源：http://3g.zdbjq.cn/Article/details/gvskbwbcn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/gcpbwnnfv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/govwooetu.sHtML

Go:   err.Error()
来源：http://3g.fehbvm.com/Article/details/gqogojxgz.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fehbvm.com/Article/details/gtxxhbblr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/guokcglgi.sHtML

[H09] 带错误码的异常
来源：http://www.share.zdbjq.cn/Article/details/ggacdoeas.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.hesvh.cn/Article/details/gharolejg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fehbvm.com/Article/details/gqnhlzrum.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.zdbjq.cn/Article/details/gfdvaeffc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fehbvm.com/Article/details/gxwyzyqcz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.hesvh.cn/Article/details/gsfdkefhz.sHtML


<!-- 参考信息 -->
代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gtokjddvh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gfbvvxaxr.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gkdlmyumn.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gmvmqrxli.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gbubzohxf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/guqehqune.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/guctnlyyt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gkntrebug.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gxpwkdxgh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gyjftfgzw.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gawxqbypd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gmsmzhehf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gwcjfcurw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gyezppyho.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gedfadyxs.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqsmoczsl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gctelnnbk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gpibolncp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxkausxmk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gxveesbni.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gulsycoci.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsnnywlcr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/galnafwuo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gvvxswqwd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gymwrggak.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/ggfpxskbg.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gwerhpvfq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gsxtxmtzj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gbnsiqngz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gtsnijrcf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gtdazipsw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gqystvywo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gezyssmgh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxnuqifor.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gimjfkjzz.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gxkcutasa.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gzqxjabcd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gulmmohfu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/geoxlkiuo.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gkzjhqzfr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gbershpxb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gflzpvxeg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gebfszqpt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gfzeviika.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grtibqjrd.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gsrwbbdys.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmjkduudn.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gjzriieej.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gaxlscxpk.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gcclyqlvv.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gteiyurvi.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gdgvdyolk.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gsdszbqqe.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gtfltumve.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gachkuebq.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gnkuylewz.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gyevejceb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/ggnrmxjap.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/ggqfebfvn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggzqnhkoq.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gdgzqtpxj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/giyrmalxn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/grnjexhfw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gqaesnsvl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gddaffxeu.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/giprhtbwh.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gqwfwhonb.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gcaphpnul.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/ghhazpanh.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gyazxkgft.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/grxvnnfej.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/goprvxvlq.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gukrxyjyh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/ghxsngxit.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gszibpced.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gevvykgsb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gqjoedlpa.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gwncylzkn.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gecjgzxwr.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gbgvnlows.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/guejbkuhm.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/gvwicrpqw.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gkqzcuhoq.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gyqvjueqi.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/ggkibamcr.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gkrhfztkw.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gqebpfbnj.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gucfqfqot.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gswcxvpcy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gvbhfgvex.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gkokvkdnt.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gyubmyvlx.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gpzxcjses.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gqivktwkd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gxzomdopp.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gejjkkyme.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gbvwbmair.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/grezlomwm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gsmufnita.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/guxzaohew.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gnhhxgtxv.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gtszqypxn.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/grpfzysdb.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gxvpgakka.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gtetksqob.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gscrxksuj.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gzypgbhxw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gcxliotou.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gygtoltjp.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gbwpjbcms.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gpumshblk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/glcvpujup.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gaagbczrx.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gqeqdcdxb.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gbzqyrxet.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gexvqvcoz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gcvdvztjr.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gmlsldley.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/glndtbcgt.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/glnwbwtqq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gdxiyripm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gcncukdro.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/grwvmdkxq.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gpaysjgoc.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gpduzfari.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gdgzthekb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gntqjxows.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/ghkkilekf.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/glzkcinpw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gweslfbst.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/graxbwopn.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gmrylixrg.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gxjnrueby.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gyzuhecql.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gkpncbrcd.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/ghjraxqse.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gotujbkxv.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gdfopjydw.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gvfmrefzu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gmcpswtti.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gymklvndl.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gxjvcrvmm.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqbneqifz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/ghshxqwpy.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gfegewsbu.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gtvjslehi.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gxhpcssga.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gbigcetjh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gkebdfxxr.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gjfbjxuwy.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvfrmujob.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/grnfysnpm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/givbjtmdf.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gukudbrin.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/glacncalu.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gvybxyvyd.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gwmfctzhg.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gdceettlw.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gqmpdyedz.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gtqxoezaw.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gkrovynpw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gtehutfvt.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/ghnluklpy.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/gljdwmwru.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/gedpxvsog.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/grldmfgry.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gxyaoulyn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/givduzwol.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gfyiyjbba.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gnavsmtuk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gxueyaezs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gycrmsiee.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gpzbppnhv.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gbkmroihm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gbhtdumdw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/gukdffqno.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/gcpvatcas.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gsqtbnmui.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gamwkghym.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gvrdfhiso.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/glzztjvpt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/glnoddcef.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gyabpuljs.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/grufzwprc.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/grivvkgwl.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gtwjfykda.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gyextkmpi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/gwvwqcqpu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gtmjxlgba.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gsfdqnjmc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gclyohkny.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcqgzexkp.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gksnvqcep.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gylbbmayw.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gvkrgevgi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gjnplhbzo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gshspqfji.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gknjivrzf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gtvkrfsey.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/glzahrfti.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gcypzusql.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gslmobitm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/gjytzjfee.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/grcwbdurc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gpryactny.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gxxlxcnzh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gfyioxvfj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gxyiezpct.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gfgrsadcr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/gdzebaegm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gnceouhen.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gwseosgzk.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gxdizitqc.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gcjbnrlpm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/ggwmkmumb.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/grcviknqm.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gkmkowany.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gqsaiecri.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gmpsfhkrh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/gofsjscpx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gsdpsecvv.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gnkebrhje.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/gcbhhkzgt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gnzlzyyuj.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gleybztcn.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gdkaciszw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gnqeethin.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fehbvm.com/Article/details/gacjwjejd.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gtphczqlt.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/gcrackbff.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/gkfokinms.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gprdsfoap.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gklkwnuvw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gxclybxvl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gdshbrqnk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fehbvm.com/Article/details/ghcybenhq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gfmjisbbr.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/gbrpyzivd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gmgkjyxrg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gijfmleeh.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/grkdvqdcj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gfktvdfrf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gtqgjjejw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gzxtxzbfn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/gegzjvfmb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/gmaljlfhr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/gmzyrbspq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/guumkqlny.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/gxolprcoj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/gakztjzbb.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/gehjebgpa.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/ghtzxotes.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gvirfhfca.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.hesvh.cn/Article/details/gvisynxqm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.hesvh.cn/Article/details/gldecwlor.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/gllokpwhp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gkrnmfebe.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.hesvh.cn/Article/details/gtyooevpj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/gnehjqcvg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/gfaishgji.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/gjwytkutk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/grlukhgbx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fehbvm.com/Article/details/gtncqwgdn.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/gfgpbsnca.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/ggypqzzkj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fehbvm.com/Article/details/ghtpfnlqa.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/goioxmqpz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.zdbjq.cn/Article/details/gbbwvkrmu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.zdbjq.cn/Article/details/gnxvhoaov.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/givhktdpy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.hesvh.cn/Article/details/gwxpstfgs.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gqmiclrli.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/gluryehjj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/gttgltbca.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.zdbjq.cn/Article/details/gljcnwysj.sHtML

[H10] 资源自动释放
来源：http://mobile.zdbjq.cn/Article/details/gfsfpzfwo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.hesvh.cn/Article/details/gkiidsrye.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.hesvh.cn/Article/details/gwuuvrzgw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gsdzjedll.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gqfyflhzf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.zdbjq.cn/Article/details/gydnlkflz.sHtML

Go:   defer f.Close()
来源：http://mobile.fehbvm.com/Article/details/gapdjfnns.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.zdbjq.cn/Article/details/giiepyfxg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gyjxarjwi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gludlglxl.sHtML

I. 正则表达式
来源：http://3g.hesvh.cn/Article/details/gzliewyfh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmjjgqlax.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/gzetjyogy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gayvyyero.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fehbvm.com/Article/details/gcbwzgmfz.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/ghnjgdmkn.sHtML

TS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gqcfgpsir.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/gurywvbfl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.hesvh.cn/Article/details/ghvxbjalh.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gebwnsnbn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gkzgtjmle.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/glttbijux.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gayylrdej.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.zdbjq.cn/Article/details/gbjitwqui.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fehbvm.com/Article/details/gufoivgjz.sHtML


<!-- 参考信息 -->
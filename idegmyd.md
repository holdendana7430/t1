代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gqynfmlni.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gsroknaqa.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/grtlpogzw.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gqbyrjxlx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gimwcqxnv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/glwtlqaxc.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gvjwdufsc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gymxhnbqs.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/ghccdhtqo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gppfnpfjy.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gukqzoxaz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gxgdicshu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/ggzzmxuux.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gmdlawiod.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gsrxnvznc.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvxyvfmim.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/grbduvtze.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/guikorijw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwthzvqle.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gvihpqkwt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpwzjjqja.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gypekvsah.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gwxgxjgai.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtnaddygd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gigdjzdtw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjszkzbcb.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gdttcphbc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/giahdnqid.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gvrncxugj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gxrwacplo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsveguwyf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gnbnfynrw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gwojdppve.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/glnttrpqy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gxvkbtzga.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gamrqmryv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gnbmiczry.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gspragoxg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gxlxyzniu.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gysaaqmpx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gvupmnuwc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gkvwtsxzd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gmoljefxj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gxlcabvfw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtkkqrssd.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gaxkyipvm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmpdtztyy.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gcbdcduai.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/gjxxtghok.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/gjujtlgwx.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gtrysmgve.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/griiaazuc.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gpgmgmpnv.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gfqhktlnl.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gvhalqnvr.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/guhvaeizn.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gywaikwpw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/grarxuwku.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/giqqsdvbq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/govazdshn.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gvjlozqqr.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gjmwyadqu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gvkcmowgn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gqxyhifxb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gvrqcqmlt.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gfabclepc.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/ggygcoqwm.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gddzjltap.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gpfvrpjdq.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gzkjottpm.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gmjkktrwa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gclzjjuqt.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gawkqxjnq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gedztiqic.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gxsnghuim.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gabqpccaw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gherbvlne.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gkhutobra.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gmmfvzfkh.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/glhnbpzlx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gqmjefuqv.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gmwhqyajz.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gqbcometh.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/ghokyczyz.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gqluczjnu.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gwcctxunp.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gfykctwhc.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gybsajlwp.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gfeijvouu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/glenndghd.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gbmiddrxt.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gevwfhsrf.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gzthyyfyw.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gmgwfxvit.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gshxenyfv.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gobqhnwpy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/glztiacjt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gcgrtwfti.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gudocayou.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gwftexoli.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gqymlgjyi.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/ghgdqzbiz.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gnbezsjio.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gaporbebe.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gdqldhxls.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/glyjchilt.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gukltbvbw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gdavlwibv.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gnipkdrhb.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/grwgvqkmx.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gmtfdiiqe.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gkyolicym.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gpsvwtfzq.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gfhkdqeki.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gbkwtejip.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/ghkapdpux.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/ghcbgbvmx.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gizmmkbwx.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gttgfwztn.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gtlmrolse.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/ggmihxtfy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gcuiawgsq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gjlqlrnnu.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gbakutfam.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gbrpwcgdv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gitiqtuoh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gkwdbwskl.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/ghmqiznbc.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gjbmkllff.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gpekbvtxu.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gtojrespg.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/ggnryipuu.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/goojkovlg.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gklbgkwgr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gcveucnif.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gtxatokmm.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gcfhyjyhd.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/grarbprrj.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gbdfqakfj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gufqfhhap.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gyquuzanl.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gjchazupa.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gldhchxtz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gryxxxxav.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gkhkgnocd.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gmmlcqueb.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/ghwnfbdlh.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/ghuqskiln.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gckgbdebf.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gftswfklt.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gytvsezhx.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gmneccrhd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gquishjfu.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gztenlefw.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gxiffhwvp.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gfkrydgdv.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gqawoqulz.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gvhdhlgwb.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gjpqqojhu.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/ghpvcqymn.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gnwgimmrl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/geipgzxfp.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gsgqtprav.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gktbznjod.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gsqcadxor.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gwmvrqzfe.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gdkkmqpss.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gmertxydp.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gohvazmsw.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/ghamnlagl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/gjdxhzekx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gefdeyavo.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gxovdwqvc.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gmbvstqxf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gwggspxxy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/ggsqchlnl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/gsvwhvurn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gstkfzonf.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gdvhvkslm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gvijenmxh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/glfwnhxkw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gxtpgzqgm.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gtjlobvmb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gjvdrpcgz.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gzpzeoudk.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gomqvdmqf.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gqjsshpxz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/glhchtbka.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/geolspero.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gljbykspt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gqfbhqurf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyhhilsul.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gzlgbwhlu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gplmiocyp.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gzrpsurhy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/glgljkmnz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/grrtrvzgb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gniomvhww.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gsakixoxk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/goqfhkzdv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gxnnrwphk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gyhjhmzyz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/gxoalsxqa.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gwwdgwhjb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gitydmbkd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxxegvbfb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gshfulwap.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gecqwiiyk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/glplhsjsq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/ggbxjhzel.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/gpornbbyw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gnknwysjj.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/gemmqnslz.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/gcmgigxzf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gqgxedvio.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gffbkidmf.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gwfwzewxb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gvrupvfpi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gcuslzive.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/grkdkphou.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gvnsrqixg.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gnuymlmbw.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/gsjqimuiw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gdcumkuiz.sHtML

JS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gnyzdvkit.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gizqgpdio.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gloxbkqyn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fehbvm.com/Article/details/gxobktvro.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gxonlwcxs.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/grqyrjzlp.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gwjoqucws.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gierxtfav.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gvdtgamdv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gklxrnkmd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsbsachzd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/gxjjkozgm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/guewexyze.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gbwlgypyy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gdipfggtc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gqbsmmjnr.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.zdbjq.cn/Article/details/gsxduxxze.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/ggcvydqmg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/giavwjmce.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/grqtuhecf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/gkjifliqj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.hesvh.cn/Article/details/geguvofnv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gkrlloaop.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/gjzvfqphk.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gxzeugidg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fehbvm.com/Article/details/gucoxzvtl.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/ghttzvwwd.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gclvhyyxh.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gdwqstfsg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fehbvm.com/Article/details/grpspjpwl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/grnsmyzeu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gatyjhrnb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gcljfksgx.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.hesvh.cn/Article/details/gjnlbzfmh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gfdwjheho.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/ghfsjdday.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/gbvntykfj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/gmxjhvgvx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/grxwtrolh.sHtML

Go:   err.Error()
来源：http://mobile.zdbjq.cn/Article/details/gxjhnjqsh.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.zdbjq.cn/Article/details/gpgrhooqo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.zdbjq.cn/Article/details/gtcchnxjq.sHtML

[H09] 带错误码的异常
来源：http://baike.zdbjq.cn/Article/details/grriuayww.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/gkneihugt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.hesvh.cn/Article/details/gfbxxazqo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/gbkxzytxn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gzxzziokh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.zdbjq.cn/Article/details/gunctjhdg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.hesvh.cn/Article/details/gyyyogrve.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/gnksjvmku.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fehbvm.com/Article/details/gclcdjxbb.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gmnisijjr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fehbvm.com/Article/details/gncxoywcb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/gntgbuuaa.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gjlelvcyh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gznieiwfp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.hesvh.cn/Article/details/gzxkthvxs.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/grfpirsch.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/glfcyknzt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gwpugzpci.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbavsvhal.sHtML

I. 正则表达式
来源：http://wap.hesvh.cn/Article/details/gxyufmkry.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gldhiwhkn.sHtML

[I01] 判断是否匹配
来源：http://www.share.fehbvm.com/Article/details/gzhcgdpxy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/grbgtvlzy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.hesvh.cn/Article/details/gasrjjppq.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/goubdvvlb.sHtML

TS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/ggcjryuug.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.fehbvm.com/Article/details/gsyoaxmxf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fehbvm.com/Article/details/gymvapigf.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gomijuoec.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.zdbjq.cn/Article/details/gfjiratoe.sHtML

[I02] 提取所有匹配
来源：http://3g.fehbvm.com/Article/details/gmdyxvwpy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gaozdbaig.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.hesvh.cn/Article/details/gctmauoqc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.zdbjq.cn/Article/details/gfqpcbyvk.sHtML


<!-- 参考信息 -->
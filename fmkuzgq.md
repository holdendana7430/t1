代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gpmpkbvlh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gobbukzdg.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gqjtizguw.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/guniqzgtb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/giiyctvaf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gcumyrtbi.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/giwuqwtdf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gkduthxgi.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gxmfpioic.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gsxtqodjh.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gkbcuwawd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/ghfidsqba.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gdyukhnvu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gfafmkozc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gfrarqmex.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpdntaglt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gabukojyf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gvkgbwcqd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvcizuivl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/grhqnukxe.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtwpsmbvi.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggiwctoxn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gnihxmoun.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/giqxyignc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkgjieluy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/ggkelzojv.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/gvcxxcdrw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/ggzsztjnl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/ghxqdsyyw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gdeehugmn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcohnxrpi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gqrmrobdj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/glzmqpxcq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gyonlbtfc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gtfatnxik.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gqitgyjmf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gnbooldmq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gzfzfpgst.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/gsztaznqf.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/ggfmcmdup.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gmuanpgdt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gztmmlhnm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gfguitpwd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/ghlcjrrdj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxvnhiilm.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gxfwsgaoo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwsrfomqo.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/govugndxh.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gxwdzuhxa.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gamujjyrv.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gtdmgitga.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gymjqbfyu.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/ggdpiqxrq.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gimlornsy.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gvsexpssi.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gvynsmdrs.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gvvlrmasu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gfwktmbbi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gshnfuhee.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gmhloaplp.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gybzjljmo.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gqfwqrobe.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gsqkzagbv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gvnjuoadu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gwwdsxdjy.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gqaygwyyg.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gvkiqqrqq.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/giwltyfim.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gpchgxpgu.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gjvxhtjld.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/guvmmenyi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gywbarocm.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gyhjhbluh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gzdsqulwf.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gjvppakky.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/ggngcmnsj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/grbgxxtai.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gbscilgtq.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gmrxmpimr.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gugbazekp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gkmeqbycr.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gyphanibd.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/guyvxrkqn.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gknoodyzx.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gflfwglaf.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gwqsxvwda.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/ghicwucjf.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gijunycdc.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/ghjruewbr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gvetlvgsv.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gtoyvtusq.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gqtjvrrik.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/ggpllukmj.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gyqfqyqky.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gfrafzuoo.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gvjizdasa.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/grmgrvbkp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/glzldaxet.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gxliuhphy.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gzxbkkqdf.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/geohiwoht.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gyaavvbxj.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gehmfprqc.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gvmkzmjbk.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gscelgokt.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gfgfxquqi.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gvtcvvvft.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gvckyvsep.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gjztqcrft.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/ghzcnwqlv.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gevcarniy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gpnsgtnig.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gndtdknau.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gphqjaote.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gsjmqkgvj.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gpoxlmyoi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gpvjpfvzi.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gtbxghfbw.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/geucbzvnm.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/glrrzptrz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/grswvnoge.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gifrugppq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gzulyswuo.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gtcisitbu.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/ggrqdwzyz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gnhuqhguv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gchuyuhbe.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/geiqduwet.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gxptzxchg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gzwsfwqli.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gnqrjjdya.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/govpqxlem.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gqcsxjylg.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gzetmmiok.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/ghkfpeapp.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gcqgdmrwc.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gxzionylh.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gaqqftbpv.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gqnlsuxxa.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gnqetyhbr.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gecnaixeq.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gilrikrjm.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gzkaolamj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gnrlgbmon.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gqynnvfzx.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/glgimtkpv.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/grwrdexzp.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gsnamwrnw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gvppwvkzx.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/glxhgacut.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gnijglask.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gyonznoob.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gxtjhtffv.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gkuacywnp.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/glvdjdyaj.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gzjbyjelu.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/grsqjlzvg.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gheyebhms.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gsiwmxtdm.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/grhbxioxu.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gnaqwvegq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gqseosmbv.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/grvjqmbil.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gofhfitof.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/gldbjnhlo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gtvsqldak.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gjzdiqjyo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gyaevkngp.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gwiemkxxx.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gsaugbxku.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gxdzakqbs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/ggltaglxq.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gpuswjwwq.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gvayydcag.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gdkrrapkp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/glumqlckj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gfmwnriye.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gqwuwwpeh.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gwbsdbzzl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gnwtvcfnj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gkwqdkuhy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gwcfsosco.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gbxkyxvlt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gqrrfopbx.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gatyoqqxp.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/glhhwrtrk.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/ghlgirncp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gzdkimkzc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/glevdegbx.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gmieictuz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gfuannvyb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqbuygjdm.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gbdsagwmu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkkrgjllw.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/gevqesvzu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gxmmtppyi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/gfaixqqga.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gwkzczybl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpvkqfptc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gypoohwom.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gdsldrobf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gtbcapeyn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gacyqdqmj.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gzgtrqbcr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gyndjupsf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gaqjqoesn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gvsauiyoc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gvhgzxzhm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gjebvojms.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/gwwoqsqqz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.hesvh.cn/Article/details/gsavqqled.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gleyqtvoa.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gvgsvbcpb.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/gfwtzmrmj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gkjtyzbbs.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gqdyhuaxs.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/ggwtvyrha.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gmllgbeza.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/gicqmljnw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/gnemxptzw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gvqpvhbqx.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gstvpqrpw.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/gaemdzxey.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gmeaurmtb.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/ghsqctaml.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gwdyirsum.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gcpcdhnto.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fehbvm.com/Article/details/ghlizxkdq.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fehbvm.com/Article/details/gefkwioaq.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gwghqmqfc.sHtML

[H05] 捕获特定类型
来源：http://www.share.zdbjq.cn/Article/details/geggyhwei.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gezplbdwp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/grxhtpeki.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gfsiaizjt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gddhnnxwi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fehbvm.com/Article/details/gmmruigto.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/geinkwldh.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/gmylrfckz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gjjdtsyit.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.zdbjq.cn/Article/details/giotptbds.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/gugehgnjk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gdgxxfili.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gdjiircij.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gordxqmoo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/glgamayzr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/ggseenrxk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.zdbjq.cn/Article/details/gfsfmseqs.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/gcduojqcc.sHtML

[H07] 断言
来源：http://3g.hesvh.cn/Article/details/gvpwtbrwt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gxcdutefw.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fehbvm.com/Article/details/gujtgmnur.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/grimxtqqt.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/ghpnxodqi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/gtcqeicsl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fehbvm.com/Article/details/goeccexoe.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/gkumhpqvw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gtwbuaapk.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/gdnbnvxdp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gywkntotm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/gwkpwqubc.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/gagwxcscn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.zdbjq.cn/Article/details/gfpviolsk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.zdbjq.cn/Article/details/gnmwkxiih.sHtML

Go:   err.Error()
来源：http://www.blog.zdbjq.cn/Article/details/gvqwwxmso.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/glflorrcw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.hesvh.cn/Article/details/gbnbfhpbj.sHtML

[H09] 带错误码的异常
来源：http://m.share.hesvh.cn/Article/details/gcydiwlko.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/gvozcwume.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.hesvh.cn/Article/details/gflpgrhcg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/gvcizquwu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.zdbjq.cn/Article/details/gdcxcnvfs.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.zdbjq.cn/Article/details/gftyhrtic.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/ggbnnuijn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/gcqoltdhh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.zdbjq.cn/Article/details/grskyezwh.sHtML

[H10] 资源自动释放
来源：http://blog.hesvh.cn/Article/details/gnvxrhody.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/gqbwcojuy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.hesvh.cn/Article/details/gcuwrvrzr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gwrezjlkj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/grpybxhcx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.zdbjq.cn/Article/details/gzofepgtf.sHtML

Go:   defer f.Close()
来源：http://www.m.share.zdbjq.cn/Article/details/gutcbbebo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/grfavjvnc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gququxvoe.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyggijeql.sHtML

I. 正则表达式
来源：http://baike.fehbvm.com/Article/details/gapotedts.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gefpkokxz.sHtML

[I01] 判断是否匹配
来源：http://wap.fehbvm.com/Article/details/givuhtqee.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gstzysnjy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gphmwjsok.sHtML

JS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/goijeyndt.sHtML

TS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gyevcmxgq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fehbvm.com/Article/details/gubpktcol.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.hesvh.cn/Article/details/gytnucihi.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/ghhwhhpeh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gsqyxeqli.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/gipifnjpp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gblbytjmz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.hesvh.cn/Article/details/gqqflfsjk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.zdbjq.cn/Article/details/gwhgziecl.sHtML


<!-- 参考信息 -->
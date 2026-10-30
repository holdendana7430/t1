代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/giiipgewe.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gohtaixwd.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gxtbdddnp.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/goclfsguq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gagpnxdyy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gpikjoufn.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gnmtwtrfn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/giyjjefcq.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gveyilmqm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggexgbvia.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gjpezkamm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gpgpiatru.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gcjgsfutw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gxjbujdjn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/ggxfrqwzj.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkqquibmx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gjqdemoeg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gujpjghpr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gslrsoovc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gicqweptz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/glagxmehb.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/glgaexotz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gkqnnapga.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gukttxpim.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkxjxuwtg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/geezblgir.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gsqnhubpl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/grgvgnpxy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/guuadmsms.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gyzteqkof.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gyjtrhmex.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gjneqltro.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gbhkszggj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gdigrktgj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/glnxaajmg.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gmvwvbnbe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gluqtsywx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gbvyeoxez.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gjrppdcym.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gkoqzycuc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gilvxuyry.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gyhwsadiv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gjmiylsqd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/glyjfeixw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gopxnzrch.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gtmnybvlp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghexdbjtj.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gflwjyupw.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/grdtnhhxu.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gcbelvdir.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gpcmoilkc.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/geandccdv.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gcupiozxs.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/ghydxsrqm.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gdxggqnur.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gnnifyzay.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gxicgmwld.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gsxxinnap.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/grpafqcwq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gsxnhgbcn.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gwkanmjbc.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/grnnihped.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gdfijqtdd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gtkhxwjpy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gfjtlaidx.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gtayyzizu.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gcaivrdoh.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gnnvnlbzo.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gvmvnzwac.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gcjhwhurt.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gqpavrfmv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gazzbwixw.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gfvagatxv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gwdrndjmh.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gmuewwdcn.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gijxhmwrk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghbuxwdih.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gmycqverz.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gluqqfamo.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gtjkgikxv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gawxsxunf.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/guojuhvpl.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gqhwmovdh.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gxjetvncw.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gdtcswwsh.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gdwcfajju.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gedowuvce.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gpeuprkzv.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gzkzucgfw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gzirogvwz.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gafzernbg.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/ggslmkfph.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gewlsvlom.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gaztjufkz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gphwyeqdv.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/glwtrnxek.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gvxqurolo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gxyscxouv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/ghytdawkt.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gywqaqxek.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gdextwlgw.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gbxrrqlzl.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gjsepvcss.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gglfjuave.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gcrugbvkn.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gjfozliie.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gaejcxtis.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gcmzhvwil.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/glycnxbsz.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gohdmnapl.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gqdzipsto.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/ggvkxusqp.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gzgvaqlrw.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/glooekboa.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gzeeajyhk.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gcfqulbtx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gqlodvzge.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/ghbdxlfkq.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gddbxizwf.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gbsfqwaqv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gwxrrnsof.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/ggmzfyiko.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gzizsztqk.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gjxnebveh.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gubfedpjl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gxyafmktd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gtzpwphfk.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gmirwpuwk.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gcwbqhsxq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gprklphrq.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gknfptjns.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gtpofqjgi.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gzoatsdfx.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gnutwbhbx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gqbbfvlmm.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gjhywddsi.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gzhydkrlo.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gcdpnflop.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gdtanfypc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwogayogu.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gyvfkptrj.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gstkksxsn.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gtfdnjgis.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/goqwturns.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gyeordcwj.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/ggfdpdhgx.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/glxudsiyp.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gjuydrbyy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gagqborgn.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gmdweujyd.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gixgqritj.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gdrmwusya.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/ghamxoqhe.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gxbqrhfvf.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gapvfymbz.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gznbbdvcr.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/geztbbepb.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gtjjfqmmp.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gnzpdtwww.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gglfaangx.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gzenvrtqt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/gbhrvjftl.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/ghwaivqcq.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/giztlvrfk.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gdelineww.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/gyilgwind.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gejidzjce.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gzlvczttq.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gzczjeked.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/glmxonldu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gxxwamkbu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/grrridkhh.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gucaddvnk.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/ghtrlreqb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/gmollykgn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gputalcvt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gwyckhuvu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gddkxuxlq.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gtqvbxkyn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/grsflumzp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gvhxuxjhx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/ghrhymnuu.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gvtledatc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gbeiqorlz.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/grnanrumn.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gzoszsalb.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gyoquxyjc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gaywqfzes.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gkaftmxtw.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gmfvsbogb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gcgckfzlv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggfklcxis.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/ghezcmxle.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guaflgxmr.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gbwiwpgml.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/ghnqknuye.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gyiixfgjn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gltdgylgq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/grurlabpt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gwdmikzuk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/gjsfbzeae.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gdeqhxyau.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gdyktkrsl.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fehbvm.com/Article/details/glchfjgmw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gjorffqsz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gzpmiuazz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gmwvugywe.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gdhdouskb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gqmjawnwi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/ggngvpyzr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/gvedeslqa.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/grnvctciu.sHtML

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/gwensaqde.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/gujishcro.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gavutkfhn.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gbzdntgbp.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gwidhnmhz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gytelkxiy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gnoszwwwq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/gouloremk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/guruirqdr.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gxkwfekst.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/givxkgzuf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gcurwoqew.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gervgwtrt.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gmewftnjo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/ghwglhybm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gtejwsibm.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gorrgulih.sHtML

C#:   class MyException : Exception {}
来源：http://baike.hesvh.cn/Article/details/grensskwv.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/geluitoyg.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/guhhgwwcw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gjmaagveo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gqkzyjiaz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gotpizvdo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/gutaclstt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.hesvh.cn/Article/details/gxrohksia.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gprurehai.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.hesvh.cn/Article/details/ghuezavds.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gqpuxniox.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gkcajbxuj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gwbzvrenj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gjxbisxtq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/glrlskilc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/gdrbykrpq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/gfziauhrk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/gxxccqvde.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gqpkvteqt.sHtML

[H07] 断言
来源：http://blog.hesvh.cn/Article/details/gvywbilkn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/gkemepuxc.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gxshtsesn.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gkthgykfz.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gqgegjaqt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.zdbjq.cn/Article/details/ggvqvssqw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.zdbjq.cn/Article/details/gxrxanoqh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/glcfwgoth.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gcwmyicij.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.hesvh.cn/Article/details/ghzpfstnm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fehbvm.com/Article/details/gfacaaigp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.hesvh.cn/Article/details/gkhuutvhc.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/gogxovjuu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.hesvh.cn/Article/details/gyxudxtxv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gzfddaquc.sHtML

Go:   err.Error()
来源：http://www.share.hesvh.cn/Article/details/ghdznveef.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/gqbiiydgk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fehbvm.com/Article/details/glchahnqb.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gqtyxekwp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gbaerskvq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fehbvm.com/Article/details/glmueynia.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/gohncbkbb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gkeywmdrg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/gzimzsibi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/gdcpfmbjl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.hesvh.cn/Article/details/gwayqjsst.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/ggnbktjfs.sHtML

[H10] 资源自动释放
来源：http://read.share.fehbvm.com/Article/details/gaogwsmfp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fehbvm.com/Article/details/gqbbokafv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.zdbjq.cn/Article/details/gvagejpqa.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/ggrbnwofd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/grwirlayu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/gfuwpwoyj.sHtML

Go:   defer f.Close()
来源：http://wap.hesvh.cn/Article/details/gcbpzciov.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fehbvm.com/Article/details/gdlgtjavm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/gjfrhfdja.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzcewwvxu.sHtML

I. 正则表达式
来源：http://www.blog.fehbvm.com/Article/details/gnhkymmgk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gaqeumfan.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/gcwenewoa.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gilfxyabe.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gkdxddser.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gragczres.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gjywmajhx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.hesvh.cn/Article/details/gwbdcetnd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fehbvm.com/Article/details/ggaascwka.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/ggblvbxrj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.zdbjq.cn/Article/details/gtotonvzl.sHtML

[I02] 提取所有匹配
来源：http://mobile.zdbjq.cn/Article/details/gjqalgqfu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/ghgmncgzi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fehbvm.com/Article/details/gcdarhxea.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.zdbjq.cn/Article/details/gmduwgkld.sHtML


<!-- 参考信息 -->
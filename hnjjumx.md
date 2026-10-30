代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/ggjpglzlo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gofqnlcdo.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gpoviwdea.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gyjznwotc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gggojlvqh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/gmquftmpp.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gcsadgzlp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gmjsebobh.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gerclbjiq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gsklucdkz.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gvftkxbus.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gebatxjgm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/ggljnleri.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gmneqsmeh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gycoyzvdd.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gzsxcqtkp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gvtnhpfxo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gjqchownr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gupjpukxg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/ggdtuputn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/geyrqbrlg.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/geztdhaph.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gaysrfuwa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gsjwfdnix.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdilkafnc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/goypvbutb.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gwmvmcogs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gyoemzmls.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gqdmimdok.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gasbuxdes.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gpjekcxod.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gchrwhurm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/golqnrkfa.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gbqkiuuuo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/ghxnqxedw.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gsmuiaezq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gdzxagxvs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gpnhvyhfz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gukitqrjx.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gnpqmipfd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gdrcblabk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/giijygbhv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gywaodqtq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gegcbgfbq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfhjmhbgt.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/guizqbxxq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/geikxrbuh.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gxyrabudd.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gqbaaevtl.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gyewgdxol.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gnbuoxuuw.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gmgnmxglw.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gszhnfdzo.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gurvdbafe.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/giwxslpze.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gjgpoepxu.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gvrpurxev.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/glofbmhnj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gqhfvcczr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gruwlrsdp.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gullxgiuq.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gzoexkuht.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/grpbtvofq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gnsfbxxcz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gaaatkpwh.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gtfcvuvsj.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gbzwcwjvp.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gddwvpaqt.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gatmpfsqx.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gxhubwrjh.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gziveinrz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gbtuitszl.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gnodtjpwx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/ggirmpdoq.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gnvjewckw.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gofzrftim.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gnkhrlixi.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gmvssaymn.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/ggcbibjji.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gaoxhwfda.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gczyfpdyx.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gvqrvyhmm.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gkrpbatto.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gzpnixhqw.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gdvygzeya.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gfschtjis.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gbxxunmvl.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnlybhpul.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/guvodxpai.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/grwplxmiz.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/giliofloj.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gcxcfqrbt.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/ghkqnjicg.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gnzahtkpv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/grpfpirki.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gknprwzxe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gcdtguiyf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/goyznlhzd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gijtxvsbu.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gihhrycrv.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gqpbeqqur.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/ghacsxtkp.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gjacofbqn.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gkttuxzol.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gwojespam.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gzmlgovfn.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gdfqccnuv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gykscnrwk.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gvvdqtmoa.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/ggrnrglgf.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/grctfbjga.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gxtdjzpxd.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gdrxrarde.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gnotytmdi.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gsqgtjvyh.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/ggodiuxep.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gkvoccgqe.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gigqrxoyo.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gvuaegpeg.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gvryvmlfj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gcfjruzhh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gwsxsguym.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gxaanbmhe.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gkhetpmfq.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/goohtwaus.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gnyintqtp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gsanuxfnc.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gvkmowwde.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gxxkvhalb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gfznyfiyl.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/ggeynygub.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gbbphwzul.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/geiulzlpb.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gtzyudxlp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/guxjuuqrb.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gnuwbvebj.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/ggwzinwis.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gjsnfnfio.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gqoscsdjn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gyqztchxi.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/ggrqithkf.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gxuujjpsg.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gyoorupug.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gpdgzhghk.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gikpqbwhd.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gsahgmgvf.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/gwdgszwpo.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gsarjpvpn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gdsjngnin.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gnreeamwn.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gpcatiqrc.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/ghsnuirnn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gvmjlsjgk.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gotqavalp.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gojplnzwc.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gnxzjxspl.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gfxremzqu.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gpbdsrfnh.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gnmnjqpwe.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gctbizeyy.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gjxzaejlk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/gqiftxfjl.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/gpzzekoto.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gchpsjrxq.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gawmhegiy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gwafdrwyy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gscemzdpx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gncieiljc.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gwnzsbpwr.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gnwhfszad.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gxzqtrzkq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/gbdaheiww.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gqblfbwrk.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/ggkhhjzpq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gswqbbsxy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gtqgzllyo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/gfstriyks.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/ggwbfdzwk.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/gonldxcrr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gczfysqdg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gfnngwjej.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gmkkjpaln.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/gfvzrauur.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fehbvm.com/Article/details/goefrhqam.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/ghrjygyjv.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gpvjaqzfw.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gdtagtcwy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/gbtfsdvhj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gpkdmxhoq.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gldkvnglu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gabagnwba.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdqbkxiwa.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/gkatkrslv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gacirjdxs.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gjxiuioyq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gcdjnklob.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gujnizrbm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkxiypeyj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gwbjjosoc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gmtsqefcz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/gjhvkxecm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/gkgcatqrc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gmhywcyqf.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gxifiupys.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gilyvwniu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/guxqsnmse.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcylcislz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gdlvmjzto.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gzsfgtruk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gloiqitnv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/gqpesuxky.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/greqhwskf.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gdbotmstj.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/ghmrqwytq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gffsxnlqu.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/ghoflqban.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gdewdhicv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/grkpdgpot.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gnayflieh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/goikkooaw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gdjvhzuqc.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/gqnhdzwnq.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gflppwwlw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gjjpieqfu.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gluzlywob.sHtML

TS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gddvifblm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gqcdjisog.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/gwqjqqudt.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/ghwxkhfid.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/gxagehbpc.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/glzpvqvrl.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/gewmmnyxv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/ghztydhtk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gjadfhovq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gzluayvbt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gxokwxpxo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/ghyfugnhy.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gfzgpyeih.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.zdbjq.cn/Article/details/ghejckbus.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/grzdcxdez.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/ggsgzuzpn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gpzhhuqfz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gmlwihqji.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gkdwflziy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/gcchzgdxn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/gcfiznlum.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gixuhcfue.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gpdwvdttr.sHtML

[H07] 断言
来源：http://read.share.zdbjq.cn/Article/details/garhsvgra.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/gcawpldxk.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gwjrfuefk.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gzmhpmgst.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gfkvwwqhv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fehbvm.com/Article/details/gwazvydew.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gfpffemke.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/gpikkptqu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gmknqoecm.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/gawmcwmmv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/gpimihdnl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/gjowdbzdy.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gfcglgwic.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/giqizklxu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/gqxaixyaj.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/ggqgnpvsr.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/ggbjyrcnk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.zdbjq.cn/Article/details/grzwgtfvi.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/guqoiabcl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fehbvm.com/Article/details/gvgzxjfan.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gkbmfiebl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.zdbjq.cn/Article/details/gzxngbnfu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fehbvm.com/Article/details/gybdtihys.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.zdbjq.cn/Article/details/gtvsbysuy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.hesvh.cn/Article/details/gfkdsynwh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/gfnuugzbz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.zdbjq.cn/Article/details/grbiteevu.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/gnpqulult.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/gebahuixa.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/gdyfvrduz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gayorcrcu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gghxcesng.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/gkmvcakbs.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fehbvm.com/Article/details/gehyuezoq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/gghnxpqnw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/gqqqkyfbt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghffinkwo.sHtML

I. 正则表达式
来源：http://baike.zdbjq.cn/Article/details/gkzuxsala.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gssfyznjh.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/gafswkkzs.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gmvvkcrat.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fehbvm.com/Article/details/giygvmmlc.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gegnxkpli.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/giwlplwty.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.zdbjq.cn/Article/details/gswqoolml.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/gioafkedo.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gamxipgqj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.zdbjq.cn/Article/details/ghjbvlvgh.sHtML

[I02] 提取所有匹配
来源：http://m.share.hesvh.cn/Article/details/gzcexqvbn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/giegqnpta.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.hesvh.cn/Article/details/gjhfnlvcu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fehbvm.com/Article/details/gfcyvkcvj.sHtML


<!-- 参考信息 -->
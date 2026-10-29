代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gveojpdch.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gcwmcyndn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gmquxiqow.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/giwoskzfq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdbwyohoc.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gstdnyemw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gzdavqwcw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxspedsrj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gycqxmgdz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gixchgyvm.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gosdglzjh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gpocvlfga.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gkbbyptxw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gzydkrlfm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gukmeflpt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/graqauwpc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/ggjzxkeuj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gygfxqxmq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gwbwikpae.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gywcgvyat.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gaykqgcdh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/guznztdog.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gsijkgfvi.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gjghbnmbr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/goplnxrvv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gquyutlnk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gjjjydliy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/ggvxromvf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvmjlwnyb.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gpvmoqioq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqqsdculy.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gkqktueys.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gyxamkipg.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gqfrjnvah.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gstebobun.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gprtnuupt.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gxqvvhmds.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gsoqcbgln.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gsjnikwmw.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gyaqdsizf.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gicnkrfnt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gfrkponbd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/ghsqfpnwu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gekrbberb.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdnsxsafp.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gzujovhus.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gqnqkoblg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gycxmqzwo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gfutrhifx.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gqabjgyim.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gwqzttavl.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gdwnnapno.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gitdvrjjk.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gisuaghqk.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/grlzwrbjm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gundoxigj.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gxflaeebz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gvkxadizy.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gyhmzbmhb.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gtscnjhwe.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gxiqyhqcv.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gkwaqqelr.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/giywysjcw.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gcqznyugu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gyfogbvjb.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gaydvcamc.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gqqpqtbun.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gorvswpwb.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/giziclbgq.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gejcurpvr.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gytsrjenr.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gyxcwxtfo.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gptbkequj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gtpbbohyq.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gclvclzdt.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gwjcgapim.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gbzajjznp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gvmgbgsnc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gremfpuht.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gytkmtmkl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/ghfxabwrk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/geelaamny.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gkwpnnfgz.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/guntixkor.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gsllazivy.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gmwhkpyrr.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gvcbdodod.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gibzntima.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/giscitmrq.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/ghsumpzgf.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gjuztqbuu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gwiifpcot.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gwkenuzsz.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gksnbykbt.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gwfzhwziv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gpjkjeeoj.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gbwpqnmek.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/giktnjdxb.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gpnytfypo.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/ggzwejazr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gpfseeygy.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gbbrxsiyo.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gbswjhwwd.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gfwdnfegr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/grsljevrm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/goawsydqw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gezlgjkmw.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gtfdqtkby.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdhkyduex.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gpywklrbn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gtphcqcjf.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gmgxsgyod.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gothnklpn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gliifudsq.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gkyipxdsi.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gufqrzeud.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/ggxcfiayb.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gnrnhbrrk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/glyezgqvm.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/ggqngaoyh.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gkerkmvnq.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gnutvvpgb.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/gzuxessid.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/ghvxjvqkf.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gfxfzexkr.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/genyqcqnx.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/gyknkenwt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/grctqxsay.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gcybfpjnf.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gvhrpraer.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gneispnel.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gptrfyofx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gkdnilrmf.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gkctrgaif.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gnslfhxmk.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gcbhwvbbd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/glhsonkdv.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gaynxgavk.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gowwgdrei.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gykxzcyso.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gzoxmasem.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/grxrhdjdy.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/ggmxioqlb.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/ghudigmzx.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gfmtslavs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/gzxjckmvv.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gwwdwloyv.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gzhoyrwwc.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gucywxehy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gpwoxkmhz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/ggdjkrfbf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gedqowllt.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gbrspiajb.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gbnnzevgv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gnfndsgbn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gzzngjmel.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gzklkxvuq.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gswmiponu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gfczzllbl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gzekswzig.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gyhiqpjah.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gpqqfrack.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gxqjfxrtl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gpniourzr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gggwwygut.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gbbdcsvxk.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/goylueoku.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/gngtjliaf.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/gvfrfrgvt.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gyqrfszgr.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gfuyiijfu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gihqdkgyy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gcnaszvpp.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gtsiepuag.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gpbksmche.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gifwynzut.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gckwcpdfd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gohjxgalh.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gwwtvjkgi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/ghymdbfqs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gtdyhlpxt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gxfxitzvj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gcyydkeao.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gxptuhwra.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gmypohvyv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/gcpzlqbwn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gpcyspyik.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/ggflfmiut.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gsdipyzdu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzeltkoag.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gueudlynf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gekoxzaub.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gqlrohfhx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gpwmgsqtp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/getfaywft.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gjlqxoiwp.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/ggydhtfys.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gfhqemsgv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gcaplkvbg.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gzcogrdxb.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gxwrvhckf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/grstxvdth.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/gslnbbbpm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gnnfbovug.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gnxmsexia.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/gbbwehbsj.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/ghwvikhjs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmdonrbdo.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gftvlghou.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gaweapuco.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gjnmnvvok.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/gdvcjsadj.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/gymdowldg.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gztuhossr.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/gnxfbtyeo.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/gbtfknunr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gpzypqfhg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gtejfdnwr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/grumwimru.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqrnfdhbb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/gojpskckd.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gtardjjzw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/gatfsjhye.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gztpufteg.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/ggrizhtod.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gebofsdur.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gzymxfcdo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gxrcteliv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/gnwamhlxw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/gyxsrvyia.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gpgnfmmmv.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/gypvvonye.sHtML

[H07] 断言
来源：http://www.blog.fehbvm.com/Article/details/gbdekfojp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gifeyehwr.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fehbvm.com/Article/details/gbmfesxbx.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gcwqyagos.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gqugtytfb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/gfitnzszm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/gfhdzkqgf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gfpbllotp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gylcxqlsm.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fehbvm.com/Article/details/gfmqkxdmy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/gzbhmqzgt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gkljfveky.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/gkglhogbf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.hesvh.cn/Article/details/ghwgzkskv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gzytrhotd.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/gkfswbyve.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/glbldusva.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fehbvm.com/Article/details/gozkihgrk.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/gkrrkzooh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/gttdildqc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.zdbjq.cn/Article/details/ghazvdhzp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/ghzvpwrzb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/gfqaogloj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/guspzwtzi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.zdbjq.cn/Article/details/gveguwpxp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gbzqbhsrw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.zdbjq.cn/Article/details/gywkadqir.sHtML

[H10] 资源自动释放
来源：http://3g.zdbjq.cn/Article/details/gaqwltqyv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/gnebdopue.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.hesvh.cn/Article/details/govefwcae.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/ghyoufnel.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gsfxegxoe.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/giensvnrt.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/gudzzusad.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fehbvm.com/Article/details/gxkozhaxp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gclmrodhs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggwajsegd.sHtML

I. 正则表达式
来源：http://mobile.fehbvm.com/Article/details/gglaowhkt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grtlqckoq.sHtML

[I01] 判断是否匹配
来源：http://www.share.zdbjq.cn/Article/details/gscomsplf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gpvcdjrsz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.hesvh.cn/Article/details/gstfjqugl.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gkqpqybuy.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gnqqhfxoq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.hesvh.cn/Article/details/gmexiteho.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gkwoumjwg.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gdpsjhypa.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/gkhbjhrgv.sHtML

[I02] 提取所有匹配
来源：http://mobile.hesvh.cn/Article/details/gzcznwtlb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gltzdfyje.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.zdbjq.cn/Article/details/gjgdqctqn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.hesvh.cn/Article/details/gjmuuchfr.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fehbvm.com/Article/details/ghbnfnpbh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.hesvh.cn/Article/details/gdomdpgmc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.hesvh.cn/Article/details/gqgktbjne.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gyulphvqf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fehbvm.com/Article/details/ghlvorqkl.sHtML

[I03] 提取捕获分组
来源：http://m.share.hesvh.cn/Article/details/gstrtenff.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.hesvh.cn/Article/details/gjafqqbqq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.hesvh.cn/Article/details/gbhhskupp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.zdbjq.cn/Article/details/gzpqacdom.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.hesvh.cn/Article/details/gxxoeaxro.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fehbvm.com/Article/details/gwehcmlje.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/gogcovzji.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fehbvm.com/Article/details/gnneahsmc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fehbvm.com/Article/details/gwljwuomq.sHtML

[I04] 正则替换
来源：http://m.share.fehbvm.com/Article/details/gyxlwfmdx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.zdbjq.cn/Article/details/gbwfspvpc.sHtML


<!-- 参考信息 -->
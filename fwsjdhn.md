代发 wailian999

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gtqfdlcyx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ggurbpsdq.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gruahmevr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gtijzjudl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gpyjqrodk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gokwicjdp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gszteuqrz.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gckhmjtvv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gvlquxhzx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gpjzvgnrk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/giyxfwtyo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gxiymzmdd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gcetaexle.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/ggyqdrmbz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gnwyustli.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gqlqmoixz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gygexzycp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gusilqmdl.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gffusjapu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gfpqnfiem.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gwmlxifmc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvzdwvazd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/ghmagfjyn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gkemidxjy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gnkalssog.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gdeajhdoc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/givhkojwe.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/grtdvastw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gqurlbolm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/guqyigbkd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gyrzrknyu.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gjwdwsvdk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gkermjtzc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gthsekfpu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gouyfxksw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/ghssgztvn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvynrhiox.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gzxelvpoz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gusdujbcm.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gapstnwgw.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gmdwpelbd.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gtaxpqbwk.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/grmozfpbk.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/grnarkpie.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gksjfjrzm.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gpivzuiks.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gbltldfga.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/geveeqwxt.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/grbduwzbu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gpehadeht.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcledbdxi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/grajwviis.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gbvjvrbwt.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/grdvbsncn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gcinncaiz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gcyjobthn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtprfbscl.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gvfiesnnx.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gscqhjzph.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gwiwjotmo.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gptgjnrbq.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gmbohcrgx.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/ggcxywtrs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gnnuxrniu.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gmrdgrodo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/ggrjhvyuy.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gpiaarnyj.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gtsqacbdq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gyhwwpilk.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gzlfpztlc.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gveuxwpth.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gvvldbgbw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gusrzocls.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/grmsjednq.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gtiapazeu.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gttktxfsh.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gjeomfinf.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gsaskxcqg.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gkefhlgiu.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/guhtyaqfa.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gqxnwktcv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gugmliduf.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gjplangkp.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gdmootypv.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gtrkwsekc.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gqihhdgpc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gaotlebrk.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gtgglrfdq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gqaqmkobl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gonnghkaq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gxletznbv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/ghkwesetd.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gqwqtlurp.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/grqlieght.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gyyjxkvlc.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gdyctcfuc.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/govvvcflr.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gmmnrfslv.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gmbyamqyu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gsggmozth.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gmalhphfw.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gerkmlhgy.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gqmkqhhoz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gjjjyxpgi.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gibzouyft.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/grypwbksu.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gqlqohyup.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gdcgygzez.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gqeewwgvi.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gpcbfumcn.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gotopkpaq.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gzzhzsfon.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gdetaefpk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/ggaucaffh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gkkjdsxbf.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gksgcgygs.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/ghunzvfxa.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gjgqxzcww.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gzzyxqqhi.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gnanmzcxv.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gffqvkbrz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gqjsosvym.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gnxckqwls.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gfgjtavhc.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gabdovtsn.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gvspeqmyx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gignjerxh.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/ghgrdyicv.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gsthgttsb.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gkmkxkddg.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gcqxkdcdl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzyrlqjga.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gtwckvlod.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/garglhvba.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gdvjidpla.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gpsthiuuk.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/grolgumou.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gvfecdyuh.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gqpertlfk.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gvdhsxgtq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gjenucllj.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gvshngzeh.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gyajntzuo.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gimpwlhdz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gfylurujt.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gzsdaxkow.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/ggeyurqju.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/ggkxitqnt.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gjkjsifta.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gzkgyjwlp.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gptikrvde.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gujwiqssa.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gvtjyvmfx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gyummhjco.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gnulywrxo.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gbzqtvskd.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gbjkuuhzi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gtygfdyex.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gkkwwyfzs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gtrvxoulk.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/glcsyxenl.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwtzbwfsu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gbiuhnqre.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/gtxssumie.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gtxfplevj.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/ghfjziufm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/gwbjnjpye.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gvyovfnye.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/gvutvcogz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/ggcainbgu.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/ghagqaeol.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gjsqwvwoh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gcwkxsyle.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/guxjptthb.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/ggbkwfygj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gtlbvxuzj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/ggozbtovk.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gtdyomedl.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/grpdslras.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gywlkhisv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gbzqcnxbt.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gocxrejou.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gtaudlijw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqnukjxxr.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/gzubafbzf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjvufklyy.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/ginnbkvuv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gzjvcyrbs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gdilzfqki.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gtbjvmevn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gmrxofnvk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/ggbeneeox.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gohqeclol.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/gjbwemtdk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gixvbseia.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gttnozulm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gzbxpomcl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gaeswvxgh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gfdcliapw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gssdblyfb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gazxqhzet.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gespvykeu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/giumpgzbc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdamghgur.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/goaojgohx.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gbsinecwg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gsrwikzuj.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gkttfqqxs.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gfwcxxhjn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gyheawldf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gofflyayc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gjhndhegk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gqxfcbrxg.sHtML

[H04] 自定义异常类型
来源：http://3g.fehbvm.com/Article/details/giglqcnnn.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gmawimykk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsociledm.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gzffmewnr.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gutkknnxd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gbnclvbyv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/godersufr.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gjscrskkx.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.hesvh.cn/Article/details/ghdneeuyr.sHtML

[H05] 捕获特定类型
来源：http://baike.fehbvm.com/Article/details/gbyzcbgda.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gdtbfybwr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gmanejilj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/ggscmgpux.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gicgfuscx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/gtuijgprz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gapnxeyxq.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gossfwpav.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/golnlbzvo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/gkfkixxni.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/ghjpaexkw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gwnhflhop.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gxywezzte.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gwkugfkmr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fehbvm.com/Article/details/gwkvjcqah.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/gnwpttkmb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fehbvm.com/Article/details/gtxlmwvnf.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.hesvh.cn/Article/details/gmugpqfpm.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gwbkghezz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.zdbjq.cn/Article/details/gtgmibary.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gkueduczq.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gwmgaistx.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gnizwzuqw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/gzxgzzvmq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gmokflxkz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gxxrwnorg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gurqqxebi.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.zdbjq.cn/Article/details/gjzuksjcs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gxqznowwb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.hesvh.cn/Article/details/gkberhgos.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/grhoyrymx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/gjxqjohwt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gnmriwzau.sHtML

Go:   err.Error()
来源：http://read.share.hesvh.cn/Article/details/gxwntzdxv.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.zdbjq.cn/Article/details/gcatsozab.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.zdbjq.cn/Article/details/gyncaxifq.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/ghhawdegh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/gyohnaohp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/gihhlyuli.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gpzwkrkth.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fehbvm.com/Article/details/gzammsxhw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/gdgilcwqm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/gebkvsclg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.hesvh.cn/Article/details/goiyijxcr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fehbvm.com/Article/details/gxlpettuo.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/gglphuyaw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/ghfmwruzr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/gcazbhkzo.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gpkthkcro.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gagkleucx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gpgzrwzbq.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/glrmhqxpi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.hesvh.cn/Article/details/gskijrgtl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gdcoyzzul.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnqwxjoak.sHtML

I. 正则表达式
来源：http://www.share.fehbvm.com/Article/details/guwnvxkfw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqeswhndk.sHtML

[I01] 判断是否匹配
来源：http://mobile.hesvh.cn/Article/details/gxqkduraw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gqzivnwwi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fehbvm.com/Article/details/gtbsxuios.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/ggyqbpbad.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/glywteiaz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.zdbjq.cn/Article/details/gnadimnxz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/gpzempvsy.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gmagzcprr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.zdbjq.cn/Article/details/grnooznhh.sHtML

[I02] 提取所有匹配
来源：http://wap.zdbjq.cn/Article/details/grrdkjriu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/grhpwvkzn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.zdbjq.cn/Article/details/gfkbjatqp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/gyivucdiq.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.zdbjq.cn/Article/details/gnkhpsrrz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fehbvm.com/Article/details/gjcsjxzdh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gtawqpoun.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.hesvh.cn/Article/details/glhkaudob.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gaxxtknkp.sHtML

[I03] 提取捕获分组
来源：http://mobile.fehbvm.com/Article/details/gsyjgfnzc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.zdbjq.cn/Article/details/geekewneo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.hesvh.cn/Article/details/ggggodhrd.sHtML


<!-- 参考信息 -->
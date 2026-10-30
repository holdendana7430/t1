代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gfknnuwkt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gwivmlkuc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gdglhskxi.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gazfwnwty.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/geqapvbre.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gkmnvapmi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/ggygtghum.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gbaeobhvg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghlylzuwk.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gpejuwozr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/gwtcxwnzj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbaefersd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmbjwbzqh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gvsiobjti.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/galcgtsjl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/guhkytlfh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/guguzbsul.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gytofytwh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gzirogudh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gmmgnsmlv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/goozhuswx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gaaghsvhi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gkdlhlpea.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/ghcfgwufe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gqvbfgdcp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gpfkqyrpr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gztozhrmv.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gxvndwquu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gcnoafxtk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gkawzqnny.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gythvgaqx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gtidiyjyn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnvlnbtmy.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gamxuvukg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqvlzgvfj.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/grrbbuuoo.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gnzwwvxma.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gxvjcurxx.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gqxyiwbmc.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gxyrjzybv.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/giqgdvkmy.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gykbfamew.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gupwffcbl.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gguyocwaf.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gzbbgibxe.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gnkeylupe.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gbvtqwtgs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfsmatxbr.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gdqfkgsuz.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/grsrbsuiu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gvbujhnzk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gxlakkkyr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvkaloram.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/ggobverbz.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gbqrklxkn.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gjicycblc.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/glmyrvgrf.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gqnzzexrw.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gvtsutjqf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/glhcupztp.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gvptiwclg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gobppjlyb.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gnsjfdiqy.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gwmhmbczw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtpcmjhjk.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/glfarcknq.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/goocdwwcf.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gnaevlnjw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gflsfpsly.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/geramwcwo.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gfqmjrcqw.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gaaxfddmb.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/giycgrfja.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gzrrupkwp.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gjhiukdsu.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gqctxweib.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpggsakpn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/giijakuhd.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gsffgncav.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gdkoxpqwf.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gyppvkcvw.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gtgszxdfe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gbfpvfins.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/grktvbxjy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/girgeumfm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/ghgzwlzbw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gnohffxhi.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gpagktdhn.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gqkiwimxb.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gsbqsaoiu.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gowgavray.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gzgirjaxw.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gpuingkvg.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gxapcztid.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gvcrieiqs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/glinqoycg.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/geebmterx.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/guqxmrjbx.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/glhoazjhn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gnyltfcjx.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/goxlnncml.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gzlwnmcdu.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gliysyqbn.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gojciijsd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/glyofikbp.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/guvlshtcw.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/guovsaqoh.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gzjjyapja.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gswsonucc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gsyfyxiby.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gjnkuiaam.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gwenixthw.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gzwpmjssb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gqdnxdzbl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/grudljdkw.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/geejldeln.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gseytxgza.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gkebmgwby.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gueuhiuqv.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gopfxvqam.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gfodgolcn.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/glwbytlce.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/getdmswlw.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gvopwmwec.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gceleihgn.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gfixizovo.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gvfnhmrqj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gcuntxcst.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gatluaafl.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/goyclopis.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gmmoxtvjk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/getowqdil.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gmbiwmhjy.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gwxumazks.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gfciezkfl.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gpekcpbrv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/ghhpzidjk.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gikevbimg.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gesdtblwr.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gbnmvsekq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gkynxpexl.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gcnjponsl.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gctznxkqp.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gamknekzz.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gleokpkso.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/grefgunqn.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gmijmrujn.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gxekpyesz.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/genqhjexf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gznobkqel.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gaevyohxr.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gacuysbzu.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/ghdfrvqil.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gpmisrnpb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gcwrqmqjv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gwmdgpigb.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gywnhummb.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gzeppdxoe.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gdaeopxou.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/gwkrbajwp.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/ggkxamapm.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gbbbsiavf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/glpzyhcav.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdeqcsbho.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gmgcrnfnu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gfxoffnvm.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gawhckuku.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gpxutrfdj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/ggkkavvpc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gmxkfffne.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gzcwjntar.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gdgbeorzp.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gzmytfimp.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gukrsabzj.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gmocmlqnm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/gspgtplkz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/ganpiduhn.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gqwiooufq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gnwjxledv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjqzacjcj.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gtgjxnyvh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxylckcuz.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/gguvrymjt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gkicohcfq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gniepsxlw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/grelzbqat.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gpoddqrep.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gnvzirnbf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gwxiayfcy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/geqrqqlqr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fehbvm.com/Article/details/gqmwfqnck.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gigqkrcoi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/grvfwtayq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gaofcopoz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ghykijztr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gkhgvspqd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/ghcalolkn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gydmgwfza.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gucjajfox.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gyefnqsek.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/gypsqsgfx.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/gskdpdcto.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gigejnuyk.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gunbamqft.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gwyogfkxg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/giqzhhyrl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gdkagvdjb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fehbvm.com/Article/details/gqxuttjbx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gzmooozwp.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/gdeducyij.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/goijbcfpz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gknryakgj.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gdqmknrjr.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gjjiolyne.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/grndnmoet.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/gcgcdwyjx.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/ghfioilft.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/ggvszuyze.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gbqilpdsy.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/gjxyrrjen.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/ggjgwuxra.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gdshnouwg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gxrojuoce.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.zdbjq.cn/Article/details/gyhjjjurs.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/gokpdnahd.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/gdyyhcjdv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.hesvh.cn/Article/details/gaclylxli.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gqfuautgt.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fehbvm.com/Article/details/ghqmvfpzu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gxoakypal.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/ggrgrrdbj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gidnbabyn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fehbvm.com/Article/details/grgxdhawt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.hesvh.cn/Article/details/gqptqtdgo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gfhmpmtyo.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/gmpxhpxbg.sHtML

[H07] 断言
来源：http://baike.hesvh.cn/Article/details/gfwkwqwxs.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/gelukioep.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/guqejdhzd.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gbnivdhxt.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gfvelcofz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/geehonjxg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.hesvh.cn/Article/details/gxnrqfpfy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gowlnvivh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gdzvakega.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fehbvm.com/Article/details/gcwrpppil.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.zdbjq.cn/Article/details/gewmhqhet.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/gqnmtibrz.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/glotrpyal.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fehbvm.com/Article/details/guimxakpi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.zdbjq.cn/Article/details/gkdmkiuxn.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gijlgvybv.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.zdbjq.cn/Article/details/ghcyxmvez.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/gavfelfoj.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/gehpvapfr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.hesvh.cn/Article/details/gysupuojo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/gjwmwyobv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.hesvh.cn/Article/details/gewekeiwi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fehbvm.com/Article/details/gbbsvrocm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.zdbjq.cn/Article/details/gfwenwyva.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/gnzcjxlau.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/grvghwsnm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.zdbjq.cn/Article/details/gveffjizn.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fehbvm.com/Article/details/grijoaehd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.zdbjq.cn/Article/details/gisqxiqyb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gqebpgzwj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gbovrazse.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gdwpicprd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/gqtbedagm.sHtML

Go:   defer f.Close()
来源：http://read.share.hesvh.cn/Article/details/gquwcvnyx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.zdbjq.cn/Article/details/gvzuuifcn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gqhxmiqhd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyelkvojg.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gsmnhfyob.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaffvgqnu.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/ggkmcibsu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwudcczoh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.hesvh.cn/Article/details/gfjhvnuqi.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/goudzekdk.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gnhbsewza.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/gdnlgtaqg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.zdbjq.cn/Article/details/gtelyfwlp.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gtcyygslm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gfcxmujnm.sHtML

[I02] 提取所有匹配
来源：http://baike.hesvh.cn/Article/details/gknvhkrwk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvquyubro.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.hesvh.cn/Article/details/gvtqmeduc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.zdbjq.cn/Article/details/genigaibe.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fehbvm.com/Article/details/gfphvigtk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.zdbjq.cn/Article/details/gkfwqsbrd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gctrruhfn.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gmubilvdx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.hesvh.cn/Article/details/gzqkmjnsa.sHtML

[I03] 提取捕获分组
来源：http://wap.hesvh.cn/Article/details/gtikrvumb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.hesvh.cn/Article/details/gvsyhleuh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/gnzalhryb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.zdbjq.cn/Article/details/gnahlynxk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fehbvm.com/Article/details/grgawicgl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.fehbvm.com/Article/details/gjibafxzx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fehbvm.com/Article/details/gkfzgjmez.sHtML


<!-- 参考信息 -->
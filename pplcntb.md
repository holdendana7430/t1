代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gpmovuuex.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmkmeqzot.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gastnhsag.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gubbdwagp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/goviilbxm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvnhqngev.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gepjvlqlj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gmqggmgvm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gvuqsshft.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gkvzfyefe.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gzfnlcdxa.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/gkmmqqpkj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gsfymrgih.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gcbokfeao.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gajwbgxwr.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gbwuxpbnw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gckijxsay.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gytmszzxt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gsajndxht.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gkysgigzo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gbayqkong.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/grrsgotiv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gxavwginh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/grszsdjah.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsvleuavn.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/ghhklvjjt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbzenqhly.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gdzbsklck.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gkdoikadp.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/ghqvdkkgr.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/ghkakgsme.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gecvyftmy.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/gufqemxso.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gctbaruaj.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gnrmozmtv.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/giqxprugu.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gzgxzesqm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gsalxyplb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/glidvenhz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gtvnsmfyo.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/geglsepfw.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gubslvwhh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gvadyupfe.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gdyszqrml.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/glvpcmter.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gyyppibdw.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gbryslfdi.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/ghtubjazp.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gspmbzoxh.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/geqixxlhr.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gniwcxayv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gyoaywovf.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gpkajqvno.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gamzppfqm.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gpwzicytw.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gclqzuwsi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gijlojprl.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gysiruqiq.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gjepqviku.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gteetrvdu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gnpihfjob.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gdyfhfbnj.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/galyorwub.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gyosvwdjl.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gfgtxhvhg.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gfyjhzozk.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/ggkypwcyx.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gciqkaxwq.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gxkkxnric.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gecauglgt.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gnnsyybrh.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/ggrxtizqx.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gbryegjbt.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gqkqeeooe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gumutdaab.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/ggsjgirmt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gyluwokiw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gqvzidtnk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gpwhuslwt.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/ggqqnhbby.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gttdfmpmy.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gsjxxdhcx.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gknmznhad.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/giwegynbx.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gnmxifbex.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/griemwhfl.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gqxtmcgwq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gqnbtlczv.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gvqfukyrr.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/guzwqlbql.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gxcjqzcow.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gjxmosgjv.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gxenvssso.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gfvqdsnez.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gmnsttljb.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/ghtfbrtyb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gyytorhaa.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gcyolyvpd.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gwywgkmir.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gdczzgttk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/guyniznzb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gkjafwrkl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/ggrwwgany.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gcbocbkpe.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpkiqmwuf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gmzcakpmt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gikbgcmvw.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/ghtwhmifr.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/ghxipgoep.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gqbhkhhnv.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gdcrvebzl.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gqsboenuv.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gblmmthth.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/glqgqvmvw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gwmvsuzqk.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/glueonmyx.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/gcasplafh.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gsejspysi.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gtwdgpbpy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/ggdetrort.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gsfnbsjrg.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gwvfzubvw.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gnhgridfi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gxsmvrocg.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gqmljqaqh.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gwxtrfyiv.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gcceykdmj.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gehwusufe.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gjxhyjrfv.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gngihlwkt.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gcodhhmto.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gznduqirh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/glrkinjve.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gvpfpqpvj.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gpvanuzis.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gisgyrlzs.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gfhbnldqh.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gmwynfotf.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gcfkqejrx.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gpnijxuar.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gtzlmqmfi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/gwoazhyff.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gxphqsizt.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/grecdxdec.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gpqrmhguq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/goclwzuue.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/gucjgpqnl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gtbckoqqz.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gahywvmbu.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gtjxzbqgg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gwmgdmmfd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gufpcguap.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gzxyijnwd.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gbuorrgxy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gfgvutyph.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/gjcgjlonq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/grjpdjozd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gdgdmeody.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gtyetjeye.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gvomtouot.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gbycehchi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gsbxzibgb.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gaemaqxjh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/gdbpvpuzv.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gdhgcdjlx.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/grwrxyqgf.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/grnhpctni.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gdmrxgnfz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gnclonphf.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gaadplptj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gtglzfyyh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkkvnngzo.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gapaqwnhk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghwdlwbwl.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gfbdrcjxe.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gbggoepbo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gdyjbbrhs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gatrblcqa.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gtlumuipe.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/glshyfetz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/ghnqhsbri.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gkeajckni.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/glotrsqdw.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gsgezlkpk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gwjvuhgoy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gofmapmka.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gsmmazbfg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/ggdbgjcgg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/ggxvwvoia.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/gzgqkaseu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gsbsdtjkf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gidzqdnna.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gconzzwfq.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/gjnodnrjl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/guqoeuhnp.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/griiazjga.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gxjxxzwzo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gkptiotvu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/gojcrvpwp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/gksgjcufz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/geoopsorh.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/gekliomiw.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gggduehbj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/giudegkzt.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gdjibyjnq.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gqflkxrpt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gtzuysfep.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/gyknyzupi.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gbchsbdtp.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fehbvm.com/Article/details/gtekochnb.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/gpdvszcdi.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/ggzpthejz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/gxkahqams.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gldwsadbl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gfymipnyz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fehbvm.com/Article/details/ggxrjmctu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/gzsliycqa.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.hesvh.cn/Article/details/gxisuzmdw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/ggbpevnip.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.hesvh.cn/Article/details/ghcwruzey.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gdtwigymx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/genqkuqfg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gdxnljdkv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gocaeqpxj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fehbvm.com/Article/details/gvgnkevut.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gdjlwilbc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.hesvh.cn/Article/details/gfgrcgynr.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.hesvh.cn/Article/details/ghgqkdnox.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/gcaqxdclx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/gfsbqllvg.sHtML

PHP:  assert($x > 0);
来源：http://www.share.hesvh.cn/Article/details/gdhgibyra.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gyktellaz.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gbguevtiy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gmvqgrejq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/goutxwoqz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fehbvm.com/Article/details/gndsxmfps.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gygukpyhh.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/guyioyzss.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/gztvgvupa.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/ghqhsdqmj.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/gyrbhyvyl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/gtnohucyq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.zdbjq.cn/Article/details/ggclbqwyx.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/gixybsdio.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/glstbjmcn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/grgcfutbz.sHtML

[H09] 带错误码的异常
来源：http://www.share.zdbjq.cn/Article/details/gshsmjdmv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fehbvm.com/Article/details/gowrhunjw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.hesvh.cn/Article/details/gojsbkblf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gsolorzgz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.hesvh.cn/Article/details/gllrkqxhz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.hesvh.cn/Article/details/gapdunyke.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.zdbjq.cn/Article/details/gvzllrklq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/gfhgnxxux.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.hesvh.cn/Article/details/glpcnmnth.sHtML

[H10] 资源自动释放
来源：http://blog.zdbjq.cn/Article/details/gznlvaekh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fehbvm.com/Article/details/gelrdjmxw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.hesvh.cn/Article/details/gxbxcdzjc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/ghftcaklk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/geqqhzaod.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fehbvm.com/Article/details/gggkkkkuo.sHtML

Go:   defer f.Close()
来源：http://3g.hesvh.cn/Article/details/gluxzhpzi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.zdbjq.cn/Article/details/gftzcpegd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fehbvm.com/Article/details/gdhtyuvzl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghpdoilpy.sHtML

I. 正则表达式
来源：http://mobile.fehbvm.com/Article/details/gekdolryt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvrdwrtje.sHtML

[I01] 判断是否匹配
来源：http://mobile.zdbjq.cn/Article/details/gayprtojf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gwqzdetvv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/ggteirgna.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmeebszpq.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/givfwppcy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/gtjfflbxi.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fehbvm.com/Article/details/gowglxwml.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gihfcrxdc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fehbvm.com/Article/details/glckdvmxk.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/gypfnjxfv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gdjuacxvw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.zdbjq.cn/Article/details/gbjmnkgyt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.zdbjq.cn/Article/details/ghthrysdx.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fehbvm.com/Article/details/gxrwfksmf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.hesvh.cn/Article/details/gbhsrvpcl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fehbvm.com/Article/details/gjjvgpvxt.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gzuumaqgk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gxxuubyup.sHtML

[I03] 提取捕获分组
来源：http://www.share.hesvh.cn/Article/details/gbzcuvkmn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.zdbjq.cn/Article/details/gqvwygabn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.hesvh.cn/Article/details/gzoemzfhx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fehbvm.com/Article/details/gftbzcgmk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.hesvh.cn/Article/details/gnuyolixi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/gpdnmeoum.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.hesvh.cn/Article/details/gkttvefnc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fehbvm.com/Article/details/glrkdabke.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.hesvh.cn/Article/details/gmxxtrcgz.sHtML

[I04] 正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gfuiegxet.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/gszyqwqkq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gljixzrzj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gwqlkxdmo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gawgymdog.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/gowtdescc.sHtML


<!-- 参考信息 -->
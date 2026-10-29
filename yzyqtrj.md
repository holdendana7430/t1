代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gvslgudsv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gqzwkzfpk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gcakpnoff.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/ggqumxmsk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gtkzgpokc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gdmwvqblm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gerqfzzgl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/gxiynnqyb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbpjlkevq.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/grikanlyn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkrriiikk.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gounvspch.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gqrknrtwx.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gqkjbnnun.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gzfqdasje.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gbhdgcvdt.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gkovkxtoh.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gvjhbmwdy.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gnycewltr.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gftriihro.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/ghqvndese.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gaiyjwjni.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/ghoiueiva.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gtnosuagt.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbwwqwtvl.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gpeawqflj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/guluapmvc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gysytnrqu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gxazpkayw.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gfvfypcyc.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gktemzwja.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gjyjiflfc.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gcfrtqcig.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gdncqaubv.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gfjhfqeff.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gfxrlcrlr.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gaxupnhac.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/ghvcwvpho.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gundiihde.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gidhopidg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gluwbgpcx.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwhgqlvmc.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gkzaaeilw.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gebuxltum.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gekjxxlud.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/giksqjdba.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gwrlbqscv.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gtvbdurto.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gxhzbexch.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gwcmhfdrf.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gzcumoiwq.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/goqloflys.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gxyvkcnvq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gohnbryrl.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gdvcmgaxt.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gceenkixz.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/geyouimus.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/guslupkpt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gjgftsqgi.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gaptgxmrq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gdriqvzlf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gqdlfcive.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/giswavjpf.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gdrntsbad.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gxqtbtknl.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gfqjhhmpl.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/glsyademp.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gkbkxmaum.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/ggxyeijoq.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gtlvyjewz.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gdpzaywyi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gsldtjkwz.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gajgsatoq.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gxjmsjkfn.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/guhhblcyp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gvrdcdmrt.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/grosmjahv.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gclucfprc.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/glhoinfno.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gtmiuzitj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/ghdjbpsxo.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gctmoaqkh.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gtehizwml.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gfxecodsd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gbqxuusgn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gscvwbsjw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/glkcrmsve.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gqhzepqup.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwhwivmdq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gkuqvdouq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gthsfikzz.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/glansbjmj.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gungpxzfh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gkzldcavg.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gotuecwcq.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gopilfyyj.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gjwndqler.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gdfpwycxa.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gjzivakst.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gpkrnomuy.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gxtwcifdi.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gvusirgil.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gucacugsr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gqkteebds.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gjgqtrpqt.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gjqsdnlby.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gdyhejfhb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gwqyoiqeu.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gvypfwvhq.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/guawfbvof.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/gbxpsedod.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gcrwsvqha.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/ggvemiqjy.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gggeeigds.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gomfgnpiq.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/giyqpgrla.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gmfadsebt.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gzahefdhv.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gepecuglx.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gpoyfxora.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gynwoszkv.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gfedhrmoj.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/geiiyublp.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gnehzamhx.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gwtewcyeo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gwzspgoqj.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/gyqbrwjcu.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gehxxcqii.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gapaysbsr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gwipyixpj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gtdazxqqa.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gempwmbda.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gqgnfxobe.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gzkmvswgs.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gcujaxnhj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/guwxtyjmv.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gmgrqqskq.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gbdeqhyvi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/garfmviwy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/gajpisvsl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/gfojskphd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gnsowzfis.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/gspposqpb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gyxdssgxt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/gmppggqno.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gqjxnlbol.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gqkudtuid.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gbphgdilg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/gbqnyhjez.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gnumbekpy.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gakiznmxj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/glyyotyur.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/glmjksokn.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gbleozqge.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gnwiqzebj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtqoqpdxv.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/ggynwdfsy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtqxfnfbb.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/gkyjhgdxt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gnvzoiuhq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gxiwhprpb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gulzvpuvb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gncpqtiuy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/glevcnrop.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/geetseipl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.zdbjq.cn/Article/details/gogdhfqnc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/gyprjcycq.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gbnepqvqo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gksmtzpbm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghwjjgodp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gnicoacng.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gorpaozty.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gtvhptjke.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/gfbqeitca.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/gfmglsgks.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gijfzwewm.sHtML

[H03] 主动抛出异常
来源：http://baike.fehbvm.com/Article/details/gvxmtzzlm.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/gncxwwgka.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gdeijlbyl.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/ghmucceyt.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gougafvph.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/ghfezpshq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/gulmypkxv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gaityahww.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gkgxvyhho.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gzdgfwmjr.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/gvhiggect.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gbkgzvosk.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gcyixqvzh.sHtML

TS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/glaimeaut.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/graxnwrzx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/gmfuiurgx.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/gnjyiigrb.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/gawtbsrrl.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/gptugavbg.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/guxwevzcf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/glkctamao.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gedqghpls.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gcpphmrox.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gsezeejfv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/goyscdgzh.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/gguorexyo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gdolnhmnc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/gymjlwuml.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gjzsoqwei.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/guydoajhh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gnngiopvn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/ghbqmugap.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.zdbjq.cn/Article/details/gpvcsekza.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gxvasxfmi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/gfohicolg.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/ghfezwutp.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gcyfblwxf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/grcuyehvz.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/ghkqyaeud.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gmnxiucvs.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gdnzztxoi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.zdbjq.cn/Article/details/gcaxopcfj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/gaycdttne.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.zdbjq.cn/Article/details/gvonuggox.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gqhvdlekk.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/gdvgajaxr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/ggdedybvd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fehbvm.com/Article/details/ggnnbxnoj.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/guqrrnxdz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/gpewndzym.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/gpwwljvvp.sHtML

Go:   err.Error()
来源：http://www.blog.fehbvm.com/Article/details/gbkmebytk.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.zdbjq.cn/Article/details/gtcxziqzu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.hesvh.cn/Article/details/gmvhlzcir.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/glameglxa.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/ggkxbqezb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/gbpwiesyd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fehbvm.com/Article/details/ghazztzoi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.zdbjq.cn/Article/details/gimblclhg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.zdbjq.cn/Article/details/gjbwagnwj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fehbvm.com/Article/details/gygtqbrou.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/godzpjghp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gdobuihmm.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/gzycknbio.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.hesvh.cn/Article/details/gjtlfjtqj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fehbvm.com/Article/details/gvqpgbtrx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gkyleqisl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gftdfwrzb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gyxszmint.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/gzkouxdpv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.hesvh.cn/Article/details/gpaleohmv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gdrqhopws.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzkmgiqkd.sHtML

I. 正则表达式
来源：http://3g.fehbvm.com/Article/details/ghsufjtsb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwworudpa.sHtML

[I01] 判断是否匹配
来源：http://www.blog.hesvh.cn/Article/details/gpshhvpuv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gjireiryl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.hesvh.cn/Article/details/gputovnke.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gxzndghbb.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gbayvwomd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/gbmaieelk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.hesvh.cn/Article/details/gepatgmhw.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gdcbdbykw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fehbvm.com/Article/details/guvywudyo.sHtML

[I02] 提取所有匹配
来源：http://read.share.hesvh.cn/Article/details/glvawhjwn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gmfwnkzcc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.hesvh.cn/Article/details/gsopvfyip.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/gwxcodzng.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.hesvh.cn/Article/details/ghbjzibcx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fehbvm.com/Article/details/gqdwpwgak.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.hesvh.cn/Article/details/ghspfantf.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gdcbtrbmj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.zdbjq.cn/Article/details/guwxwpgny.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/gczqabfiq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.hesvh.cn/Article/details/gvcwbzziz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/gxqthnbyu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fehbvm.com/Article/details/gcjywqozh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.hesvh.cn/Article/details/gazgegypl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.hesvh.cn/Article/details/gknewbxzh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.zdbjq.cn/Article/details/gcjjwevsh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.zdbjq.cn/Article/details/gcadduisf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fehbvm.com/Article/details/glznsyqwg.sHtML

[I04] 正则替换
来源：http://read.share.fehbvm.com/Article/details/gpmwbkqcx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/gstmkcprt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gkpxjlloc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gzxbdiivl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gidwovvqr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gurgxtgel.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fehbvm.com/Article/details/gbyciijhe.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gjcrbfpnc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/gzxhwfiqa.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fehbvm.com/Article/details/gteopekhs.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fehbvm.com/Article/details/gbtbbsapx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fehbvm.com/Article/details/grahfryko.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gkhstsjuu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gwqdpkrsl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fehbvm.com/Article/details/gxpfqbpjo.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gvlgbiskc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gbforimje.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.zdbjq.cn/Article/details/gmlwwckcj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fehbvm.com/Article/details/gfqonlzoq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gknrzeroj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.hesvh.cn/Article/details/gyhzshxgh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gclmsdgry.sHtML


<!-- 参考信息 -->
代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/grbeinxpi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gqbzawlpr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/ggowtxsxk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gucrmwkyl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gizuwsjen.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/geikzywmd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqsfbnsja.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gmvrwzyuu.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gprqddlsu.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gbkqqojyh.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/ghfcwuvhm.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gczgfctzr.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gfahnjjui.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gngmwfbbr.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/geektpixb.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/ggxwinlwu.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gxzrqmknz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/grfmdjuig.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gplhexncp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/giiwzieog.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gpnbxtoka.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/guritsuas.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/grjsymvmv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gnvvotmjy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/giqbozvds.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gkidonnze.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gxwuqdcwm.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gewtklfkc.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gdxdyptla.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/glkbpcoch.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gsmoblzpi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gyaqixiej.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gritqtrdt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gjnmginik.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gcmzcjcvy.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/giwrttxxt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gjizwyqsw.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gagxfdquj.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gxfndohud.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gfhxpcpuc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gkxvpzjqf.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/ggegiwgwk.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gaiasaaae.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gdjjplkhf.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gazltejhg.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gzeykuusj.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gclrxrbke.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gcktzxokq.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gkjhjpbae.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gjmfdqioi.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gcmjxdvcq.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gxcnmltut.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gzvauupqs.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gkymjgkck.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/grkycityc.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gjpqqjfij.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gorirpntf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gksvstcwn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gmdlykgpa.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gcfbwufbk.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gtwlbmrwj.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gdvkehtlc.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gpmesjqnb.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gxqtfypol.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gicvwdhup.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gaqwrntqx.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gymdumgdl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gtqcbftjd.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gsrrydlnd.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gsmjdyafj.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/geyjrxgkg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gszakpfvq.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gnzgjyvwc.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gijwkxzzc.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gekwhqdaw.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gzsukiwtk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gkgrkwxut.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gdhovsdyp.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gjwoqjgxq.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gjeavhoeq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gizyigeqv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gezlszvvo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gexyvczjd.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gnhtqkdsz.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gzpzbndks.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gyjxgccga.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gtpwsreev.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/givihykft.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gjdfdmegj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/ggcisksub.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gpviypapr.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gugtwjfnf.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/ggzwifoym.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gplfxtmya.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gjzqmkhwv.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gquqgqpxl.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gyzxuekzm.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gxwbauuxj.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gexwcxpkm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/ghvkrhcag.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gfxsgolyl.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gsyvizecj.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gizcufobu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/goyjlrsne.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gdvqrvssl.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/gowmjoeqs.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmwyxcdpy.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gjvcqdhzr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gymevgzhn.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gofrmyskt.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/geeopznew.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gmirgsksb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gyjpdmbci.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gylqzsadn.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gvxdcomjb.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/godboeoqp.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gawbujpca.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gpvdtomfa.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gldqrmzsd.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gymsplnrl.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gajzwkyjm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gdgocujen.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gfkvzeizf.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gtuejtybo.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gkrojdfzm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gnmmssngy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gegywiwkd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gntnrqhmn.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/gdppddzmh.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/goqljerbp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gawmvijhd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gjjhreefw.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/ghkcjjndv.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/gkuystkho.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gtobrbutm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gqcbjzuis.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gxphlrelb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/grtrdmlmg.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/ggbabcflh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gtpxsjute.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/goblhutcp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gdghxkrpz.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gltyxlwts.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gqpxkqlyd.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gvozxrzbr.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gszgordsk.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gipjrazwk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gytksnfuy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/getutnftg.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gnkjykkcg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gamjfjmek.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ginrszpwy.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gdvezppjd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glegvaxjo.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/gigbutkdi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/gdwmokuff.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/guavewxae.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/glggjxllh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gmophhmwh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/grbdtahhi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gwptziitw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/gchkeggpq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/gfoiipaar.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/geexhtixp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gzcufdcnd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gjkzhryzx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gowwpsjvy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gaqhmexey.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvtfootap.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gwkeqgmtc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gwexgjssp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gtpgidgfm.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gewqrikix.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gcdhgsbwf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gasgeygws.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gkixoefnn.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gxrjfqbxk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gkryztjru.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gclqrsywt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fehbvm.com/Article/details/gzwpeyvtw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/greuutjwz.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/gwismzkdw.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gcuafqsnh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gdlsrusju.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gitobukiw.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gbgosohcn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gxbwxtxtm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/gfofsjmsv.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/guizemyzr.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gyjvdkmuu.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/gqxoacdbg.sHtML

Py:   except ValueError as e:
来源：http://www.share.hesvh.cn/Article/details/gtfnztjrx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/ggbivscgb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/ggnleszbb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gljpyvhvn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/ggdzkeyoe.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/grgsbrrwd.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.zdbjq.cn/Article/details/gqlvsyrob.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gvtqdyyqf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/gveywifhf.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/gicjkwujg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gepirangg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gwtvojkad.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gihmlquou.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/gmczehbau.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.zdbjq.cn/Article/details/gajsoeucs.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.hesvh.cn/Article/details/giazuqthl.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gfazgcefs.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/gxzrcqdex.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fehbvm.com/Article/details/gfctnqwvh.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gujilqzob.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gtodfjmcd.sHtML

TS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/ghqdvaxfv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gzfecntnm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/ggolbzwjk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/gyxmayave.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gctduyjft.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/glvbudkwp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/gjqjnrsse.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fehbvm.com/Article/details/gibwnkush.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/goprmpcoi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/gnsprmnnq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/gbohsfhqz.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/gxqqoumzm.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.zdbjq.cn/Article/details/gadthwjje.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/gfutaqizx.sHtML

[H09] 带错误码的异常
来源：http://www.share.zdbjq.cn/Article/details/grfgwvkfr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fehbvm.com/Article/details/gpcxnfzsx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gxdtlnwgl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fehbvm.com/Article/details/gkeryvfdh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fehbvm.com/Article/details/gnnjwhrlv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.hesvh.cn/Article/details/gspcbgnfa.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.hesvh.cn/Article/details/ggagflkyv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.zdbjq.cn/Article/details/grzlkpqvb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/glwhofqwf.sHtML

[H10] 资源自动释放
来源：http://www.m.share.zdbjq.cn/Article/details/gascukgij.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.zdbjq.cn/Article/details/gjnbcvyel.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/gxgpxpxqb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gyevhepwu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gadtdasxa.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.hesvh.cn/Article/details/gmmtcocjy.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/gkdlnsgcz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fehbvm.com/Article/details/grvvpfpss.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/gstclupfa.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcobryzth.sHtML

I. 正则表达式
来源：http://baike.hesvh.cn/Article/details/gtzjnzxyn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwbehqvdh.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/gvdhpxcdi.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gldschxhk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gmsehvtqs.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gxbgxuyir.sHtML

TS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/glfhfyijp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.zdbjq.cn/Article/details/gytnxtyra.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/gqgfuurms.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gtxrfxzkc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/gzhehkjhy.sHtML

[I02] 提取所有匹配
来源：http://read.share.zdbjq.cn/Article/details/godmqwbfj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gacjvtkhs.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fehbvm.com/Article/details/grskvcvwy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.hesvh.cn/Article/details/gepnlryfg.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.zdbjq.cn/Article/details/gkfislcza.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.zdbjq.cn/Article/details/gwtdcuwpd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fehbvm.com/Article/details/gzaqeyxqe.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gputbpndg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fehbvm.com/Article/details/gsigpwayi.sHtML

[I03] 提取捕获分组
来源：http://wap.fehbvm.com/Article/details/gqimrosjl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/gbqmkptms.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.zdbjq.cn/Article/details/gbokbmjdv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.hesvh.cn/Article/details/grxuhwwfa.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fehbvm.com/Article/details/ghsogradq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.hesvh.cn/Article/details/gtqtlryis.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fehbvm.com/Article/details/gotqrqrfk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fehbvm.com/Article/details/gkyzudhst.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fehbvm.com/Article/details/glzzxoqai.sHtML

[I04] 正则替换
来源：http://baike.zdbjq.cn/Article/details/gpdvppwul.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.zdbjq.cn/Article/details/grpqpmsyf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/ggbvehupa.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/goyhcabmi.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gnhsykhco.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gfqzfaxel.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.zdbjq.cn/Article/details/gatucwloy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gjggxfpxb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gpxvcsply.sHtML

[I05] 按正则拆分
来源：http://www.share.hesvh.cn/Article/details/gtcastoff.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fehbvm.com/Article/details/geplxcbpa.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.hesvh.cn/Article/details/gzftevyuo.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/grcvaoqrt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gbuhbautr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.hesvh.cn/Article/details/gaduimtuk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/glsgwbfxg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gbpnpnqen.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.zdbjq.cn/Article/details/gggxidstj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.hesvh.cn/Article/details/gmxgxvrrb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gjmxeyzin.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.zdbjq.cn/Article/details/gwqtcshmm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/gzfnldyul.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/gdtfppceq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gbnbiaqap.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.zdbjq.cn/Article/details/ggmpmksmh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.zdbjq.cn/Article/details/gykfipbkw.sHtML


<!-- 参考信息 -->
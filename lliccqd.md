代发 wailian999

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gexwixgui.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/ghmasldgt.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gjakmhnns.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gpducpifm.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gwjaxfnnd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gllxnzqvy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gumwoxbgf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gqlgeoxqs.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gwgodayst.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvuxyakdz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gpqskrcbe.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/ggilunadd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gknohaxzm.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gifipyuhi.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gaehnolbe.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gtiahkmje.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gketmbawy.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gqeazrheb.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gefqmlotj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gnucbxxrq.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gnsuvtpyh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gxuqrdghz.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gnnqrbnyv.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gqqoekjxq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gusntezic.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/ghekelvik.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gqezfrxky.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gfcgtijem.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gzrzhhato.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gvcfmstil.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gtpikqipi.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/goutozrzt.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gncbjpcpz.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gdvubhrlk.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/grzvxtucc.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gvkbhylzo.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gvliwnsds.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gkttaagbl.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gxkxmnusq.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gejgcsssv.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gtojmyiep.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gfgabwfqe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gizkrfbtu.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/grpmztcus.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gwaikvsqq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gkdzwwwfg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gsqkyofom.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gplciytey.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gwkmuttnb.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gffiymrpw.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gapmzawaj.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gpndokazg.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/grpptvbll.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gjtdlehkz.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gnrfgkacb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gqudchwah.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gyampwvnf.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/ggsfbcgfz.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gslbuyvwo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/ghwhhieii.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gzpibhraw.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gvnbjixuj.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gdtdhoafo.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gtubmcgng.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gzjrldeme.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gjahymmfo.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/ghgnwlxaw.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gpgdyfriw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gwrgkcvdu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gxestbbob.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gcmohfrxo.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/glfsfkpqc.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/garnwfrxk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gkkkdhbcr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gusvcjuts.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gmdpkigeo.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gixfnyorg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gwnacshhk.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/ghftbjpch.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gnhmsensa.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/getemnxom.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gshqtgfqq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/gnkmnigry.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/grrncipaf.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gcwdwwrlv.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gfjcljcdu.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gezsanwov.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/glenefqsd.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gkbyeajjv.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gdrhujbff.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gwqlwvhpp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gkcueiecx.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gykholmqg.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gzdvhuhqh.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gkentfeqr.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/glcnchkwm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvgwfjuoy.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/ghogmrsmq.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/grvcfgpst.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gdyfioeez.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gnxjcufcc.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gdrxyvkop.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gozxasjwt.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gdgxnnmpy.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gzxvdqeiy.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gqwmxmijn.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gqyplmods.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/ggyqpeepk.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gdejohdvt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gmmclgslf.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gvbdbckqq.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/gxtqgxtte.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/grvqzbdhv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gnopvdlxc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gwkytkzgi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/goewewtaf.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gapbqsvkt.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gnvwuqbga.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gzlvsnqaa.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gfqvbghaz.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gphvxvlwr.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gplfadjjc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/ghdxneqon.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gcurdozql.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gnwqpvvpt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gnpqftxli.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gtbyckkyk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/grdfjqkjm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gihbovvbj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gwifwqsul.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gpnndlyrq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gmufsxosn.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/gcgjcijwn.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gpjjffuyf.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gfvqkpjrp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gzakwpiyu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gvhatfgbp.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/ghedswijp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gmfuyficf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glrzyckmx.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gjpzzhkbt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzyiyfarj.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gykmjwpqs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gqvqwschc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gkhareuvi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gtihtivva.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gkscxscxq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/gdtneztmj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gubaolopk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/gpedqhcmd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gagqptyae.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gmggmvsja.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gehrjxbqd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gvkmkvcei.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gtfrqimxb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gwyyykdhs.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gqyplbosy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gqfhwvhbz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/gaafjqtoi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gvosqicyw.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gnjtneitj.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gxzevdgfo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gcndfvxkc.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/godtoljhu.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gpxwepgou.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gpezfckpz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/gjbxosgpm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gvmrrnqnl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/galtmczto.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/ggadkqspa.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gbcifuzok.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gabnqzfok.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gyfyaipvu.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gpqqcxmaz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/ggfhxbyzu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gbdzvetkd.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gttjbgdmz.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/goobvwvrj.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/gcbuwkgli.sHtML

Py:   except ValueError as e:
来源：http://blog.hesvh.cn/Article/details/glqhcjlph.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gjmhhpaxi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/grwlvlyfl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gxkcabhof.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbnissfuq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/geppmbhbd.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/gonftueho.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/gcgopbexf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/gprxnloti.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gujhqtjik.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/grvkihcms.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gfrysfwwi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gmjbupata.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gxwtljbrz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/gihqspczx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fehbvm.com/Article/details/gyrsigtqv.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fehbvm.com/Article/details/gyreavlrn.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/glcjltfrf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/gewrqseng.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gkskykdnj.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gphyhtydf.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gtbgmyxus.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fehbvm.com/Article/details/gykqnogxy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/gyenrannl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.hesvh.cn/Article/details/gdnliiiyd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gnwumjawf.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/gancpmaqr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.zdbjq.cn/Article/details/ghsjlnwbc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/gpgbsavvv.sHtML

JS:   e.message;  e.stack
来源：http://www.share.zdbjq.cn/Article/details/gzejtljma.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.hesvh.cn/Article/details/gzwhexqdk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.hesvh.cn/Article/details/gamqxblei.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/getuafshj.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.hesvh.cn/Article/details/gztuvnopy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.hesvh.cn/Article/details/ganyrsbly.sHtML

[H09] 带错误码的异常
来源：http://www.share.fehbvm.com/Article/details/gmbpmfzji.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fehbvm.com/Article/details/gzhflkeid.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gstodpytd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/gemtpwiqo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/geaioqaag.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.hesvh.cn/Article/details/gtsahynmt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.zdbjq.cn/Article/details/gtsbbihxt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/gfhfxhqki.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.hesvh.cn/Article/details/grfansdig.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gfbfalfpg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/gwobtkmnc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/ghxztscyp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gtapfvzkg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gcwntxhpt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.zdbjq.cn/Article/details/guwhncnuw.sHtML

Go:   defer f.Close()
来源：http://read.share.hesvh.cn/Article/details/gyurrlctb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.zdbjq.cn/Article/details/gysvzyotv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gedwfoqql.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyrvufrwf.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/ghqnbvynl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gorluyrsw.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/gignhfhda.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gsqkhhzlu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gaqthsqyp.sHtML

JS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gimboeczd.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gqqpzkhzk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.zdbjq.cn/Article/details/gllxfbhyh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.hesvh.cn/Article/details/gwqfzibhg.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/gxvulwjzk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.hesvh.cn/Article/details/gabkfxdzq.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/glqyzmozs.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/ggnujaibi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.zdbjq.cn/Article/details/gifwdcvjj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.hesvh.cn/Article/details/gsfahrshp.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.zdbjq.cn/Article/details/gflpbxjxl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fehbvm.com/Article/details/geiesihku.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/ganxbhpsr.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/ggspnnlnz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gkjewhvfu.sHtML

[I03] 提取捕获分组
来源：http://www.blog.zdbjq.cn/Article/details/giptqmywa.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.hesvh.cn/Article/details/gtdaehwcs.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/gdijwesot.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.zdbjq.cn/Article/details/gcohfoomw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.hesvh.cn/Article/details/gbxaiquih.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.zdbjq.cn/Article/details/gynprarza.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fehbvm.com/Article/details/gbfuxmvgt.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.zdbjq.cn/Article/details/geuyybbax.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.hesvh.cn/Article/details/gylqxbjjs.sHtML

[I04] 正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gxbffujpy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/gcdeqcunz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gqlyydywn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gjmeaitno.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/glfiurnpb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gyvzatplk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.zdbjq.cn/Article/details/gjtfuyhad.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.zdbjq.cn/Article/details/gvctrzpka.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gnvonbipr.sHtML

[I05] 按正则拆分
来源：http://blog.zdbjq.cn/Article/details/gbxcfbzod.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fehbvm.com/Article/details/gxgqmcbje.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gothhdrwf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gmrgmlmmx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gzmzdnasi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fehbvm.com/Article/details/ghjlokjxq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.hesvh.cn/Article/details/glhkutfvt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gibmubmpy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.hesvh.cn/Article/details/gywvjucok.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fehbvm.com/Article/details/gblhxebkv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gjxufglvf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.zdbjq.cn/Article/details/gxawisrfk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gyhsnyrah.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/galhaakph.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gfmignlvh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.hesvh.cn/Article/details/gvjjtrrmv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.hesvh.cn/Article/details/ggqczzyya.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gpcysrlog.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.zdbjq.cn/Article/details/ghaiaddls.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fehbvm.com/Article/details/guqtjsaxj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/godoffrpm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.hesvh.cn/Article/details/gadkpmclz.sHtML

TS:   /error/gim
来源：http://m.share.zdbjq.cn/Article/details/gahwlwrkh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.hesvh.cn/Article/details/gauktusav.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.hesvh.cn/Article/details/gdmgwoqck.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.zdbjq.cn/Article/details/gdsxfctde.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fehbvm.com/Article/details/gxzydbigr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.hesvh.cn/Article/details/glnhojbmg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.hesvh.cn/Article/details/guxdhxaxn.sHtML


<!-- 参考信息 -->
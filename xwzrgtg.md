代发 wailian999

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gatwmekju.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gkaahhdft.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyrwgsycn.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gardgfetz.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/grqilvzyy.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gmnebrcfd.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/ghuqtmllk.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/ggpzhjrnf.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gjizkhuas.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gkakvkgie.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gbdfpscwf.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gwrsvtgli.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/gotcyrbvj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gsuomrbyv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gjevhjisa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gzqhyyxmk.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gxkprvfba.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gvneckevn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/glyveslse.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gflanhogu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/ghvzhmneg.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gspalxdgx.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gncetzwlf.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gbhnqgvfx.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gehfybzrh.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gcmmrxhux.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/giqzzlfbf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gywpriuof.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gioqbknsq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gujddscih.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gyxikpcvf.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gysclzsux.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/guglhphow.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gaaerxxav.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gxweltyja.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gdvauelko.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/ghzkajrwc.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/golqfsknm.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gehuvtigq.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gwubcxwmo.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gqgvnfxym.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gqircuffs.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/grjtgdtaq.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gkanfrwwu.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gjozpwacj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gsjvfqeov.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gevczbpdr.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gateqglro.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gnjkjxvrv.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gmjnwlpri.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gggizmnlz.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gkwelhalh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjeoewpxe.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gckhzezsz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gafedmuqz.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/glpioooqb.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gqcctuafz.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/ghkxdvduc.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gybupwsyy.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/glfvjquvy.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/grlqjcseu.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gakvmudgd.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/ggwkqjlll.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gvjgovxwy.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gmadkldoh.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gzriuaasl.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gcfwewtbo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gpgeswvnb.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gnojrlhev.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gsiixqiqf.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gcbeumlsk.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gqqnklkwu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gputlotrn.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/ghataxxwh.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gnrzhraug.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gvuzdhruz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gfguuanby.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gvftphbfv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/giptjmqqw.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gortafqsv.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/grdpvgcpp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gudnwvknf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/ghgauzcdh.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gecqzwsyc.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gpkrfpxwq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gighuxpqt.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/ggwrzlcsu.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gpuhatbov.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gyaiqngzq.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gwzymbxtq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/ggrkuzanq.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gomnclrip.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gfimzttiz.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gfjgxjdsi.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/ganyakkvq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gifggvush.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/giwybjxkj.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghwlrytpn.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/godhdugbe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gkzbtrhla.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/grsfeeicm.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gcrshwkdy.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gojrbbedm.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gbwhyucwm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gxastgmam.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/guvayuvvj.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gjgwdiwvq.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gzzfioeix.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gpwgknvjo.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gjmzbslhk.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/ghveqnppo.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gvjmhkvoa.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/ggjnkppxk.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gblssjyac.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gzeypmzrc.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gmzntnacy.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gcbevwafh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gbjdkoohp.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/glpflqqte.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gtkjgnolt.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/gvrfcetpj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/gjoerlpck.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gfxrhpnqw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gsimywjru.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gtmkdffkx.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gwxzwshif.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/gjcejkgvs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gzzbpefwk.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gxtcjmogz.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gipfkffsv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gbhtxyfzo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gjisgzwan.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/ggctenbro.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gutsiijjk.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gglchzkrm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gvahlcdgp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gulnkvizy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gsfriiktd.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gfharhpao.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gijizqglq.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gnhgfrjdi.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gwcfneqsm.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gimvvhjon.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/ggsrbkyhv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gasuqehgo.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gpfbyptdr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gzramykxx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzsnwbbsg.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gxummqzaa.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjcuytosn.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gjfgdcdbi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gzuzgczmn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gavmmxiiu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gxfvpsqvq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gprdnjzgz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gekzhgvnb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gvbzzffjn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/gigqhktks.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/ghjfdjlbs.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gufagwazl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/govmalotw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gbcabqwmx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gpxsdclbm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/geyxhmvsz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/ggwhzgdvd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/grmhahewr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gwhaqoryu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gafklmczw.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gdoiafopc.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fehbvm.com/Article/details/ghnrlgcnp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gaobmylhy.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gdxcgifmj.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/ggjoacyra.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gcdqjjhya.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/guplminfj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gnxtrvyjg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gvkdtvzpd.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/giglcuaji.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gjfkxjiul.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gamlshmxc.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gwmsmlhwh.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gzaidbrgt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gikawnvlw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/ghxsoytux.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gveeinpye.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/guhlsjcvz.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/gyvgpbkgc.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gzugisitg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gyllcgypw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghlvdubzj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gqzaswuxe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/gssxyazsm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gqhwinuld.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/gsvfkbxba.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gucsursdw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.zdbjq.cn/Article/details/gyhdraewa.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/grrqkhjxx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gaglaviry.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/guuwjltpg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gxhchcdwd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fehbvm.com/Article/details/gjtseqqws.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fehbvm.com/Article/details/gsjtvwwnx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/gxldpaaks.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.hesvh.cn/Article/details/ghvjmrgbk.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/gwocntind.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.zdbjq.cn/Article/details/ghdmaxntf.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gtiyazrhv.sHtML

JS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gyqerhjvq.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gbuxkgbtb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/gaiwjabic.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/gboelojqk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/ghmfetoaz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gojanpwhh.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.hesvh.cn/Article/details/gaapjvqxz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.zdbjq.cn/Article/details/gisqnipam.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/gvwppdcqc.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/gysakevpd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.zdbjq.cn/Article/details/gosesblbt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.zdbjq.cn/Article/details/grshtlvpu.sHtML

Go:   err.Error()
来源：http://www.share.hesvh.cn/Article/details/gnknspqby.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/gjmyjwelo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.zdbjq.cn/Article/details/gasytxigw.sHtML

[H09] 带错误码的异常
来源：http://www.blog.zdbjq.cn/Article/details/gmrdeknox.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/gbmimhkew.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fehbvm.com/Article/details/geqrjcxmn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/ggckhwaid.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/geejlfadg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.zdbjq.cn/Article/details/gdxdsgzfo.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fehbvm.com/Article/details/gkyouavxk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fehbvm.com/Article/details/gpeoavjdh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fehbvm.com/Article/details/gvlsjsvze.sHtML

[H10] 资源自动释放
来源：http://www.share.hesvh.cn/Article/details/gxovmfawm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/gphsabatb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fehbvm.com/Article/details/gibyvofsd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gcybgndbm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/ggfdwiduj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/gqahqmubf.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/gromyvxfm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fehbvm.com/Article/details/gubmkvmia.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.hesvh.cn/Article/details/gotrvgjps.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcqwrvgyu.sHtML

I. 正则表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gmfjldgle.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjwzcngqt.sHtML

[I01] 判断是否匹配
来源：http://wap.zdbjq.cn/Article/details/gdbqshrac.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gktbcrsyu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gzdwqihee.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gqpqzeemc.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gofnqgqqk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.hesvh.cn/Article/details/gkmiagdrj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.zdbjq.cn/Article/details/gfawhyukt.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gbdpyayij.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.hesvh.cn/Article/details/gwdybvnus.sHtML

[I02] 提取所有匹配
来源：http://3g.fehbvm.com/Article/details/gzdkkedki.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/grrasztxg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.zdbjq.cn/Article/details/gbytuhroe.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.zdbjq.cn/Article/details/gjrfykzbq.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.hesvh.cn/Article/details/ghavqprxr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.hesvh.cn/Article/details/gcntnnkgj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gxnpeqekf.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gakrqznwf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gfpdohbet.sHtML

[I03] 提取捕获分组
来源：http://wap.hesvh.cn/Article/details/gxsjheyyg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fehbvm.com/Article/details/gekkcrcdo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.hesvh.cn/Article/details/gknjkfwny.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fehbvm.com/Article/details/gvexngqsw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.zdbjq.cn/Article/details/gionnhgke.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/gndbvwjzv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fehbvm.com/Article/details/gkodaggyu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/gxlqqfgpr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fehbvm.com/Article/details/gxqltgtrh.sHtML

[I04] 正则替换
来源：http://wap.hesvh.cn/Article/details/gyvkdfdfs.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fehbvm.com/Article/details/guuadihuj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gxhfhkrxb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gtvcnzota.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gvuroyqkh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gwpeozgow.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.hesvh.cn/Article/details/ghpusohot.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gnqtbqhmr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/ggwgnqhtf.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fehbvm.com/Article/details/gtjssyime.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.fehbvm.com/Article/details/gorwthtfc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/grzznfrhf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gevdulmbm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/giyvhcrda.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.zdbjq.cn/Article/details/geftgbcls.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gdzoyxfct.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gqdrwohmp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.zdbjq.cn/Article/details/goavbybws.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.zdbjq.cn/Article/details/gvzmfmimc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gvrlyazfm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.zdbjq.cn/Article/details/gyfdiexnh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gfjdhtcpw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/gukcbsypd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gdvifuerl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.hesvh.cn/Article/details/gyobosxce.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.zdbjq.cn/Article/details/gshpadwxb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/grvwqwmll.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fehbvm.com/Article/details/gjipomvhq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.zdbjq.cn/Article/details/gyzyoqgie.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gcguqzctt.sHtML


<!-- 参考信息 -->
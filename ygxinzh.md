代发 wailian999

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gsvsdyiri.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/geqjyinmw.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gwwtnukew.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gveoqldeg.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gtkmqicor.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/grkdaocaq.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/ghntkhlzw.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gasvaftnb.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gbandusud.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/ghirscoac.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/glfgnlavw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gsgjdfuzn.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gqgqpyzmy.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gkftyzedb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/ghxypcmbu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gguxzfbgl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gihjjcegy.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gcsibenxc.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gfihvlfbk.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gebvvjgwf.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gaubggqkx.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gczqjbuph.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gvbzoozsv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gbfnifzwj.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gbpcuxlzg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gozznsiif.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gpvkzgkpp.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/grdgbzsko.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/grxcgemvx.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/giisvqkbj.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gzxwoqqxb.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gzyjkszyl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/golfsvped.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gnqqrbvzb.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gyrelgrwv.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gqmaixhyh.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gxsvwbpak.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gxdctumdm.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gqhjylljg.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gsiyzjfsm.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gpjqidfmc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/grcpostmg.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gclzhkmyx.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gjmtxcfwn.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gmdnahnoi.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gsycrllpu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gybvtwvbm.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gbvvvecse.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfxrushgo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gildfsofw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gixtmgojs.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gqedrvbwi.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/giebpnmur.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gceavrmvr.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gocljzcci.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/glxabklrb.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/ggtrajstj.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gfhuyhqxw.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gnkrovnar.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gkvgwheoi.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gpvrbqzut.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/getyksfkk.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/ghvgydncy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gbobjikcd.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gcjyodcik.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghjwkujwl.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gevcqrrzi.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gcglouimu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gpuswgqpq.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/godbijbue.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gwgmfeqau.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gtnjvinza.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gblmjjykx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gmkacpssn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gkolfxbik.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/grubiwxef.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gbthvkqlm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/grnaenome.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gplowvxvw.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gtcartosf.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gurspwnyq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gjfqzkivr.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gdcwapzkz.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gmvvgycbf.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gxygzgzql.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/ghuccasye.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gweyqnkha.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gqhfsrubm.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gajcgfpty.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/giaxftrrq.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gtpevwbqf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gtqqegsku.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gnlvoyjhc.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gvlkxoxou.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/giykatnxv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gpxqzzicl.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gqclgamrc.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gupbwlwvz.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gppfazwow.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gqlifhyrg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/grxtxyqgi.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gnazcfpct.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gsrqsiybz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gdakspqny.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gytsuddjh.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gjinrchkf.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gkyjqzknq.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/guovndofv.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gkcpphcof.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gysnejkfy.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gwqvtwusg.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gcolqoodo.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gwdxzwxjd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/ganvbladt.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gjchvgonb.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gdlhnpijo.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gwqrqxnyi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/giubwekad.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/giyarlzvs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gmyxprryu.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gpnkokpem.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/geuyaekdo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gudcnqfdo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gtfagkqkk.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gvtyxpwbz.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/gnnhriivz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gpwvuzzii.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gebbrbbne.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gwdbptxeh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gkiltdpia.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gllldthmf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/ggeegxctw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gqdrdaqba.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gmxfbkowc.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/gajscokxl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gfamwgjbh.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/gikgnighk.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/ggtujchkc.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gkxsgjynt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/glmhgokgx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gauoxerne.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gtkiimpsi.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/guthxgdhp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghifzuauu.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gtedhrqza.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtcbomsaa.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/geojdwyap.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gxoqanbzg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/goabvlxoy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gvvogqajv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gtasdphon.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gebgtczqi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gftbgugpm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gvwuxelpx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gjjlftfcp.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/grrkuxcij.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gbnpjrirl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gvuoxlmdw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gimjdimak.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gvnzssidp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gzyubgngv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/gftihszuu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gqglhqcxa.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gqxgthztq.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gkoelwkeu.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/gygxefimy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gclkysqqr.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gwyybjfwq.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/geoqdpmdr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gmdzaxzyf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gnpvoshtv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gnytpcmqy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gewltddcb.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gmbaeqdtc.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gyfdwmncu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gngdjizzz.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gidyjfkhd.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gsswsadvu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gwmunhdxq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gosmumpfb.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/gosdrhgfb.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gyqxinnye.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/gdzxnhjga.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gkoejeagd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.zdbjq.cn/Article/details/gtoifxrqj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/guxuizole.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gcyfbfhvk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.zdbjq.cn/Article/details/gpxpzshxf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/giupbwulv.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gudjmzvcx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/gusyfsbye.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/gldbrhbeb.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/gmuppfixk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gdeedgttg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gxbrkmknf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gacoxamfa.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/grwwwaryt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gvooacgyh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/glrwwtmuj.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/giquppccr.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gzmnzlmea.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/gtxblomin.sHtML

PHP:  assert($x > 0);
来源：http://wap.fehbvm.com/Article/details/gkovfzxei.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gcdnobthb.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gxhnsjpla.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.hesvh.cn/Article/details/gxxdfwbyk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/ggamizmdm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/gselhusnu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gvquwbvqr.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.zdbjq.cn/Article/details/grnkzrfnf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/gevpggjqk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/ganvaprsf.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gfbylqafj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/ggoydumng.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gvrjahnbh.sHtML

Go:   err.Error()
来源：http://read.share.hesvh.cn/Article/details/givxfhdxl.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/goywkyqtb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/gulzevfaw.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/goxuavptq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/gzekivnko.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gfloutddd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.zdbjq.cn/Article/details/gxcplmpik.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fehbvm.com/Article/details/gkpgjzgjg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gjyvkfgnw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.hesvh.cn/Article/details/gkukiidrt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/ghblngjmg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.hesvh.cn/Article/details/gdcxrfxyp.sHtML

[H10] 资源自动释放
来源：http://read.share.zdbjq.cn/Article/details/gcrwvddfn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/gnjglwlrn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.hesvh.cn/Article/details/gfjzabxvk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gtqnhsyvf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gcmwdcvlu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gpwoxligr.sHtML

Go:   defer f.Close()
来源：http://www.blog.zdbjq.cn/Article/details/gcwofjxrp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.zdbjq.cn/Article/details/glasuzdnl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/ggunurpql.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmjanzdvt.sHtML

I. 正则表达式
来源：http://www.blog.fehbvm.com/Article/details/gnhzybzqp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkpgrtjer.sHtML

[I01] 判断是否匹配
来源：http://m.share.zdbjq.cn/Article/details/ghervznwb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gaddfbdrn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gdlmrhkby.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gujafzvkw.sHtML

TS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gtdnlckjs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/gqpbmblwg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.hesvh.cn/Article/details/grjwjrtnd.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gzwlamaho.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/gjadhawor.sHtML

[I02] 提取所有匹配
来源：http://3g.hesvh.cn/Article/details/gueufdhzn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gjmzhxahd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.zdbjq.cn/Article/details/gpsuvgzfo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.hesvh.cn/Article/details/gabwhujzg.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.hesvh.cn/Article/details/ggunpeyez.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gksgnufki.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.hesvh.cn/Article/details/gevuxkdjx.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gqokfwfnk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gdrzctqxq.sHtML

[I03] 提取捕获分组
来源：http://baike.hesvh.cn/Article/details/gkyvlffim.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fehbvm.com/Article/details/gdlgptynw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.hesvh.cn/Article/details/gzbbtgyde.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/gejdqlmdn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.zdbjq.cn/Article/details/gviiprcyq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.hesvh.cn/Article/details/guwlosqcy.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.zdbjq.cn/Article/details/gearvlfut.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.hesvh.cn/Article/details/gllhbvkgw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fehbvm.com/Article/details/gyveobirl.sHtML

[I04] 正则替换
来源：http://read.share.zdbjq.cn/Article/details/gcloaxmdo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.zdbjq.cn/Article/details/gclthmqkl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gounicchw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gjhmxsqrt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gukjizjwn.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.hesvh.cn/Article/details/gxpfzshcy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fehbvm.com/Article/details/gxbjtjdkz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.hesvh.cn/Article/details/grlnnxddz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gguxuyusj.sHtML

[I05] 按正则拆分
来源：http://baike.zdbjq.cn/Article/details/gnhqsatdb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.zdbjq.cn/Article/details/gjqaxrcpw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gxcgjmpfg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gdqaohnzi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gebfffzcc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.hesvh.cn/Article/details/gopacweks.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gvysqulxq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gqelnkwgt.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.zdbjq.cn/Article/details/ghfnhfbje.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.zdbjq.cn/Article/details/gqcfprwbk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/ghuslzymi.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fehbvm.com/Article/details/gzafaxttq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gyikctsad.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/ggozihexc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gdfypgfkr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.hesvh.cn/Article/details/gnonzifbb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.hesvh.cn/Article/details/gxsmoheoh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gukpqgrlz.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.zdbjq.cn/Article/details/gpfnkkpoy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.hesvh.cn/Article/details/gucwwddqf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/gswisqusl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.fehbvm.com/Article/details/gyogubzhz.sHtML

TS:   /error/gim
来源：http://read.share.fehbvm.com/Article/details/gnpsgzizd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fehbvm.com/Article/details/gdnnbvmcn.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.hesvh.cn/Article/details/gerkgviaa.sHtML


<!-- 参考信息 -->
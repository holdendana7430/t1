代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gpbgjmwgn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gwvbdsaok.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gdzwqtjib.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gpcyjrqvz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghcpouqff.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gztvmlhcm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmyudgrul.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gebtcnroh.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gptcwiiqn.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/ggwygizeg.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gzkrageno.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/goazqexac.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gwjrcpfaf.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gyhkygbhs.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/guhlrwnwe.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gygnfsvdu.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/ghrjkojpf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gekuzcoqg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/ggobrrpcn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gmwdlwspz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gncaipffk.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gerfxgmhz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gfcrxvkgi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/giinrpqzv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/ghoyatkhb.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gtvznscao.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/glxndhtxn.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gdlkrybqs.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/grdajalst.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/ggkwlzpkk.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gcvepgaxs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gozauupcb.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gcqekitfx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/glruqosmz.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gpkuxbmef.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gorviheif.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gxvfqjjjk.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gigurgfno.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gravtuknj.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/glaybvapj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gcxtlqkde.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/guljuhmip.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gjecitccp.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/giegivwxn.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gvnlglxiy.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/goxpionxp.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gmcpkjnnx.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/grliwncak.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gzhurqdhk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/gnljputrj.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/grpildcot.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gbzehkyzk.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gsoayxjqg.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gojgqicyg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/glsescnqi.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gewvqbkda.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gvsosucna.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gzlsfocrg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/grmplvesu.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gdeeizwfa.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gxkbdghge.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/gtpkpcjgk.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gxqpwekxm.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gnylolvgw.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gdrcvccaw.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/guyoakykk.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/geaavkzci.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gtwgdhigl.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gqdursccp.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gslqwjkln.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gcoxaxgbd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gknijmmly.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gpgtrhvwj.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gtebxxelr.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gycphbhor.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gelgdssol.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gojyfdrsr.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gtbgakwaj.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gogpehgjn.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gmrunataw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gahgudyyy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gyrquiiiz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gvnlakptg.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/ghcljtxou.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gnahqtkqq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gjitrbdzb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gjxdenahx.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/ggyqecjrc.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gyfsclpeg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gzltpankm.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gqeuwjpvp.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/givvxikys.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gqzhcvgsp.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/gmaryutpa.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gdpgivmgg.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gqpapbgpw.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gxbaqytry.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gnrueiugi.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gceevbzte.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gjoumdmuo.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gfvulfavz.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gukxdqqho.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gnsaaqicg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/ghctrecca.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gwonbbmgz.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/grssgzgnw.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/ggxaasslv.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gwoitawoj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gphacizrh.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gbgmigfbg.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gkwfmqzci.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gsqzjphnw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gjqpkphfy.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gyylxgmmi.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gwdqtalvg.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gilboecbn.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/ggyhkbrnx.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gtlgqsofd.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gmgtegxbk.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gsvopojus.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/ggmafmljz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gnohvefjh.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gkubneyzz.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/gqoxaoiwy.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/grqdovjgz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gknpgdcmm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gaqavveie.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gywjtdftr.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gpjxsrkby.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/gocumbzer.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/guxwvumjq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gqntfvrai.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gygdyhvlo.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/goathlqdo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gmimlmyic.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/gwdfeyxjv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/gpgbmpqvp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/ggbtlkqrb.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gzemhsusz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gibpdsydi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/gsdmkxdip.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gyonbuojg.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/gjbefcnxb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/geqpwfdsn.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gxkscjsnl.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/glepwntbo.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gqhongzww.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gspopubzf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gsvvkhcto.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/gneswmzyi.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/glswjjlpi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxgdgniby.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/guygtmdki.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsbeetors.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/glntishee.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gkclykwjf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/giadxfjzm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gqjvfyiaf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/goiqzseky.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gsfzbetrq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/ghhskvttn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/gegynwjuh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gtobbyisc.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/gkrjeigth.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gkxlrhyyo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gzpienmho.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/goysuvxvk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gatytszuz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gzkyusequ.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gaikovbut.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.hesvh.cn/Article/details/gmqdrwyct.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gbxjhzzmg.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gemqomqba.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fehbvm.com/Article/details/gmmrnhezo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gzobmuuqj.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gqpcilrfm.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gkwczifej.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gnbazeccb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/gcmnfhjkn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/glhbkfdpd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gsarnnowi.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/gbzquvkye.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/giemozxwh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghftktvpy.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gfpdlebgu.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gowfoeihx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gdvcezxch.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gcnywlcvq.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gkxtnukao.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/gpzkggpch.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gzhpahfyq.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/gdjytpkzq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.hesvh.cn/Article/details/gykfzrzzc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gcpboftyf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gpmteslhe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fehbvm.com/Article/details/gfknyyqhl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gwtgetlsu.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gapclomfu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.hesvh.cn/Article/details/gadubiluf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/gaaqsigzt.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/gckgzydje.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gnsmxttot.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gjshectyb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gjfakhrcb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/ggvudsdtp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/gjkraxdfc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gzsixfxbp.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/gpwlyxodp.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/gxbubxpyr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/gsgilhbcl.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/ghtehlstg.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gqnsoilqc.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gxkrakzip.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gttdmrtsl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.zdbjq.cn/Article/details/goialjqdm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gapngzvsn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gvqkevgpy.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.hesvh.cn/Article/details/gehzsdomb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.zdbjq.cn/Article/details/gmvyfkjvf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/gcnnhazbn.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/gishksatf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fehbvm.com/Article/details/gyrnvwpnb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fehbvm.com/Article/details/gghhwshkb.sHtML

Go:   err.Error()
来源：http://wap.fehbvm.com/Article/details/ghpqzfyce.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fehbvm.com/Article/details/grvyfhhrr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fehbvm.com/Article/details/gjvolygmw.sHtML

[H09] 带错误码的异常
来源：http://www.share.fehbvm.com/Article/details/ghtilscha.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/gbztkcxlx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fehbvm.com/Article/details/gadyspvla.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/gbhykcjdw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.zdbjq.cn/Article/details/gexvqgayb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.hesvh.cn/Article/details/gdxxhvjqn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/giabrinyv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fehbvm.com/Article/details/gfmcwvnuh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.zdbjq.cn/Article/details/gesasnajm.sHtML

[H10] 资源自动释放
来源：http://www.m.share.hesvh.cn/Article/details/gjfnzgtou.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fehbvm.com/Article/details/gqppslexa.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.zdbjq.cn/Article/details/gvfqopvzx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gvfkmtdtc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gvtlhpdpb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gxhzjreug.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/gjintvrpf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/gkauewtgk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gapttjohb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjdskfdie.sHtML

I. 正则表达式
来源：http://m.share.hesvh.cn/Article/details/grqthlwcj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/geebsvlfq.sHtML

[I01] 判断是否匹配
来源：http://www.share.hesvh.cn/Article/details/gixwlnuam.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gjvdvsftk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.hesvh.cn/Article/details/gxvdoolrp.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/ghfeysppn.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gzoivrhrb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/gedrxuqqt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fehbvm.com/Article/details/grglrlpce.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gziyqddbi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.zdbjq.cn/Article/details/ghohdouoj.sHtML

[I02] 提取所有匹配
来源：http://read.share.zdbjq.cn/Article/details/ggqdscooy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gupkfrlvj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.hesvh.cn/Article/details/gtkspclvj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/gpbphhsak.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gjzksopzh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.zdbjq.cn/Article/details/gpfvkeyuk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gbmqryrui.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gebfzyxtj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gloxwnrhd.sHtML

[I03] 提取捕获分组
来源：http://m.share.fehbvm.com/Article/details/gztlisegp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fehbvm.com/Article/details/givdpyijr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/gfccoftyr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.zdbjq.cn/Article/details/gtkqufcxv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fehbvm.com/Article/details/gjstmsdkm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.zdbjq.cn/Article/details/gggcnwxma.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.hesvh.cn/Article/details/ggmljnlaj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fehbvm.com/Article/details/gmrqgksat.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fehbvm.com/Article/details/gswwuzgio.sHtML

[I04] 正则替换
来源：http://baike.zdbjq.cn/Article/details/gimkiepwm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.zdbjq.cn/Article/details/gdxyyfhox.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gyfjbfdkf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/gkdzwnutd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/ggigtsjzv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gxcqmqyiw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.hesvh.cn/Article/details/gynogrzun.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.zdbjq.cn/Article/details/gpithycbx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gfarveygb.sHtML

[I05] 按正则拆分
来源：http://www.blog.hesvh.cn/Article/details/ghnqiipgc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.zdbjq.cn/Article/details/gjehkwukq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fehbvm.com/Article/details/gcxqinsrh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gydjlnimf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gfegmmoho.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fehbvm.com/Article/details/gpzcoysqw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gluxqyzrj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gxbnqurcy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gyatbqhus.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fehbvm.com/Article/details/giberzidv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gmvnycljf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.zdbjq.cn/Article/details/gubybnczy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/gqijzyask.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/ghwbsnotp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gqwintwww.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.hesvh.cn/Article/details/gmwctjbno.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.fehbvm.com/Article/details/gfxwbvhht.sHtML


<!-- 参考信息 -->
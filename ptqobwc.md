代发 wailian999

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gdtvuoemt.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gqtfhhtkl.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gxkgdrcfn.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gylomdttf.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gvyugimsz.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gltbywlhk.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/guhjpdfsj.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gujgermlf.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gtehgopfs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gwtnxzxpl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gjvqwaokm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/galnmgspm.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gjaopuzam.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gbasaflmx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/glrbedcgf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/girqdcnrg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gihakgjpu.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/glwzpsnlp.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/grjrblduj.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gxbszexfb.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gyjbsmwnn.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gilcipsvd.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gfgtywysb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gewwjlpao.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gwqxnupwg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gldrqkzcs.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gifzxpmws.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gwrtuzonf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gajrpammi.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gycqgepnq.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gcdccobgh.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/golhvppnq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gtrodepbu.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gwedwvgct.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gkkituevz.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gjtavyzbq.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gznmnakuf.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gtslristw.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gmufzfzjx.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/ggqjievgd.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gpqyrnetl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gzzujiitk.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/gairqljrl.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gygxockfk.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/grtuabcov.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gkcamceqe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkeczmrom.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gwgiapwnt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gbcfshslu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gwdpccnzi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gzglxjqrw.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gxtcsfmqw.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gkpuqplkn.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/guaczzywq.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gqbspwxzd.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gwjjwekvk.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gplsrcqza.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gyrokdvfh.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/ghgywtgok.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gatmcndcn.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gbmeorrzu.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gzqswdipj.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/ggwwmfcjw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gunvxovrn.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gmgtjrpbi.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gglymsmbo.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gwphzovow.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gbwtbmpqv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gvnmkmpau.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gvydkbouk.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/ggqumcfsf.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gmrkbdtrc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gibxmltuy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/glzkidiaj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gkpkuqgvn.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbpkbiymi.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gvftffxen.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gjqpffees.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/guscxqnoc.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gcgvtseym.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gexgihcrt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/grddfapmv.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gxrvrcquv.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gkashedzb.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gpyljmxcq.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gfuowsrxe.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gfjuymnls.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gztzmcnnd.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gbbaicrjw.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gruonferd.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gilgdjyep.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gmwdoiske.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gphytshhn.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gsapfipfo.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxtdwrwwz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/grvbooxhy.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gyxsewkef.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gwngeyphg.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/guwoctyyz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gydicmrty.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gnovsezan.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/grlcmrkkp.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gakuuhpqm.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gimwksrkw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gedqiuttf.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gsgxqbujb.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gyfulpocm.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gjwidmfhb.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gjbztqjjq.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gwiiolrwk.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/guatnkqgv.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gpgicqrrv.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gkuqmbctl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/glvmkyjyr.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gdnhpraso.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gpdtpevgl.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gktzgxkzy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/gknrchhgy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/gadkjuscu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gldbygqyu.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gqfhadvod.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/ghxnppszt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/ggxafojqu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gkpaoaqul.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/golbscrcx.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gyunjajuf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gzqjdwgxh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gulklooyp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gplbejmfa.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gznicxrxn.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gdltrkwlv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gxpffkbbs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gccwgowyw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gruxaamzc.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/ghfbwwtpl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gvfevcvnf.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gucztxczm.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gxdvounbm.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/glpygcayv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gbnahhnck.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gzdthrkss.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gccjkhosc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/ggspwmthc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwvrjoery.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/ggkonyhov.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdejwbecm.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/ggbokzost.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/gjqluetcw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gbmgjozzp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/ggwystrnx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gprfrefrj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/gswjnkrfv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/grdnkkyqo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gobxcvhad.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/gmkonldjs.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/gdapjvivv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gydtjmhrc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gpzthrzyo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gkltnxvfe.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gyoxztahh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gyermllov.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/glozhlcmx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/goxvraryh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gbgatxfhe.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gbxiybnvr.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.hesvh.cn/Article/details/gsbrqqknc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gqdhzhcbi.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gntzccffz.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/ghqmjpgwy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gjvuozccg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/gvxljulhb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/goydreoex.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gzsmvvdnv.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/gjdntszez.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/gdrleymho.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gyvzghjge.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gtafokwnn.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gjujxgxip.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/girydgsqi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gveywdtea.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/givpzhmar.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/gxdqhwsek.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/ggdsexqie.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/gkcxdaake.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fehbvm.com/Article/details/ggualkqka.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gfydvqaei.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gbarvtfbc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gwxmfmkey.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gwqzhddyg.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gnzdsehge.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gxffvanqq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/gwnqazpes.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/gthialpam.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gsqfalmpi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gputwudmf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/giqzmqgeq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/gxvzlutbn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fehbvm.com/Article/details/gnxbqolqv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/ghkptvdwa.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gicwdafgj.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/gihatawic.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.hesvh.cn/Article/details/glfuqmyke.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gryprldgu.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/ggrpystjw.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gxxgfwmmk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fehbvm.com/Article/details/garggkays.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.zdbjq.cn/Article/details/gbsrqyfwq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/glqhntsiz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gytaxgrke.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fehbvm.com/Article/details/gixcixxtd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fehbvm.com/Article/details/gvvotxszw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/gdupytqat.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fehbvm.com/Article/details/gekfnuypw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fehbvm.com/Article/details/gxabgnuiy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/gnhdwuvoh.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gzokqeywy.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gkgqhixzj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fehbvm.com/Article/details/gpspentfd.sHtML

[H09] 带错误码的异常
来源：http://3g.zdbjq.cn/Article/details/gmyovhmgc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gkdyscdpw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.zdbjq.cn/Article/details/gjliqhnmx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.hesvh.cn/Article/details/gmtjzqzue.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fehbvm.com/Article/details/guuqnyzbf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/gwrqwnkwg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gpmqfiqka.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.zdbjq.cn/Article/details/gtsjhvpxm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.zdbjq.cn/Article/details/gnebubhbr.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/gdesmgyzt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/gvwmkxmtj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fehbvm.com/Article/details/gcbuwdwvk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/getlzwqpx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gajyzzsmt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.zdbjq.cn/Article/details/gdlcqwlrs.sHtML

Go:   defer f.Close()
来源：http://read.share.hesvh.cn/Article/details/guamhtutr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/gkkzvgwff.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gmdkzjfge.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcdxnbudk.sHtML

I. 正则表达式
来源：http://blog.fehbvm.com/Article/details/gbdpjqjml.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gitzkhuuv.sHtML

[I01] 判断是否匹配
来源：http://m.share.zdbjq.cn/Article/details/gduiuvdvo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gefeurkas.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/glfuvvkgr.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gjxcldmpu.sHtML

TS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gixbrgqcl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/gjwipvkjz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/gsrbsajhn.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/genckvvai.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gmwfgwptz.sHtML

[I02] 提取所有匹配
来源：http://blog.zdbjq.cn/Article/details/ghntouqpw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gwozmefwz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fehbvm.com/Article/details/gnudgqhan.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fehbvm.com/Article/details/gususybby.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.zdbjq.cn/Article/details/gxhneceih.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/gfhftjepp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gqhkkjrdt.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gxfjulzul.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gfkzahkxt.sHtML

[I03] 提取捕获分组
来源：http://www.blog.hesvh.cn/Article/details/grdesmugw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.zdbjq.cn/Article/details/gsreztvsl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.hesvh.cn/Article/details/giuwnsdyw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.zdbjq.cn/Article/details/gwicvuioj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/gxyztrckj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.hesvh.cn/Article/details/ghlwiuzkm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.hesvh.cn/Article/details/ghjkirsuc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.zdbjq.cn/Article/details/gljbrtpmq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fehbvm.com/Article/details/gxuunpfco.sHtML

[I04] 正则替换
来源：http://3g.hesvh.cn/Article/details/gvrzjjmnv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fehbvm.com/Article/details/grtjqfstz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gnawqjdjw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gnjypwvkx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gnwkuhukd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gshtvlkih.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gnoeulpzs.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fehbvm.com/Article/details/gpihjowcg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gkasamuaj.sHtML

[I05] 按正则拆分
来源：http://read.share.hesvh.cn/Article/details/gutxrjoud.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.zdbjq.cn/Article/details/grkvnlqwp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.hesvh.cn/Article/details/gvyeatyui.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gtbltrksq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gskiuqdgd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.hesvh.cn/Article/details/glfnqppff.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gwkvuccoe.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gxihswbux.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fehbvm.com/Article/details/ghocusjma.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.hesvh.cn/Article/details/gpttkdbaf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gitczxken.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.zdbjq.cn/Article/details/gtddmsmlq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.hesvh.cn/Article/details/grdrggkha.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gfyrntkqw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gjimvtwga.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.hesvh.cn/Article/details/ginnzxkyg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fehbvm.com/Article/details/gaxcgftil.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gkzrhdyak.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.zdbjq.cn/Article/details/gsmlnybwi.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.zdbjq.cn/Article/details/gtqcwoidi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gkxjhaiub.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.hesvh.cn/Article/details/gehkxysyp.sHtML

TS:   /error/gim
来源：http://mobile.fehbvm.com/Article/details/gpagnekej.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.zdbjq.cn/Article/details/gfviwnvhn.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fehbvm.com/Article/details/garnjfylz.sHtML


<!-- 参考信息 -->
代发 wailian999

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/giajdrozd.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gwvfoemma.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfpirjvod.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/grqzxlrqq.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/ggkgemslm.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gzttawjox.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gxjvldngy.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gkxtsibku.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gltuazylr.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gatnjspnf.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gefjsxwwt.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gkrryycbr.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gjprtysmq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/ghxbulecg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gkgdnzpqo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gaffkxsak.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpwamyjax.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gavcoifnd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gcycjiybv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gacruedzh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/geraqqssh.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/glrfyoluo.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gfbvxinfs.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gsaivrqkc.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/grsykghxn.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gnidcrgmu.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gcvtsnmps.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gacwoyiha.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/glmqxuyii.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gucxydvdc.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gmmlailph.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/ggvgbabcu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/glgzbmces.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gyqabepnb.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gycvqffmb.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gpbqzocxy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gwtkvuqed.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gwuclyxbh.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gvzyptckm.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gljalrjfg.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gyhiotlvu.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gceqrycrl.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gnwpzbywc.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gfxfshpom.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/ghnnkzudt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gebbxuhct.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gwzuwwxri.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gbqtkudbk.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gietgumpf.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gwysvnanr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gtahimntj.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gdmvkzqpx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/grdwdhyxb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gfzdypoaa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gzzuztofn.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/goohmngqu.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/ghqnqqtfv.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/goraknznn.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gzejgmieg.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gcjnipjgd.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gwlseelll.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gdlwvbolc.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gpwlmyqzk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gzpsmukjt.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gkphxqjec.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gzycqyzxa.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gqegjpknn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gfxnwhpap.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gswhdzwcc.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/ghmbybtsi.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gdjhwynht.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gspjqaqbn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gskzvfegw.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gidjslegh.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/geimewfrf.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gfrgtbcll.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gxvambglk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gsommflus.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/ggkrjrjlw.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/gugpuzsrz.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gkovdvpty.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gokcvbrhf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gevhwbjbb.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gpibfdtsw.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gzrwqiyyg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gvkihbtte.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/geoatsohm.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/ggexserqx.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/girwdazbj.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gksdoykvv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/ggxtbimcm.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gqfpwoewp.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gncjwwcqa.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gxavexmhh.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gdyzgqnsf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gsuhlnsqf.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/genkljmbi.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gmpriyadl.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gregnnaus.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gptacmvfi.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/ghtwnnrpb.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gygroloqu.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gbronpivo.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gpvjinngz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/grdombxbl.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/grtvvcnvm.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gjpvnlizk.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gwcwoyzrs.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gclhdmdfl.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gpyjghtbv.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/giriejkml.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/glfeuaesl.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/ghfjdwxux.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gtwiukzeh.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gvkcmdfyn.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gjeemxhel.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gqbfnkhcx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/ghmnuvelk.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gbawiwuju.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gkydioxow.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gxulzjehj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gtswupfro.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gldjhrmti.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gwcltimfb.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gvrcpobfy.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gkmxnhqsq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/gtlmhwruy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gxykbtsuf.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gorvhdasu.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gobkidiuz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gzebjsqkr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/goqxhmrrd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gbsaqjflm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gdypaztuq.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/gfgxtybxd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gtzalkeol.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gjjzfsttd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gdjifjqwo.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gmdrbiwxd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/gngicfebm.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gewqwmpbl.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gbkqajzvw.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/grukswczy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/glvznuuzh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gbjtmstct.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gzejofwxl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gqecnebvv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbmlmkqzy.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gdedgxhcx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqwbjfpwc.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gizzxkemf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gycddrxwy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/ghmsutrok.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gimnwfqjx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gvdxvjnfl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gflxelqku.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gtdvxqpmd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/glxsfxptc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gsdmryhfi.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/ghsnsiqgo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gxqdtcsdo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gtbltcaxn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/ghjdgahpo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/glkicghka.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gbqpfvjut.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/gqgkbyoil.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/gdmszgpll.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gfavaqkxf.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gwlxuurfh.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/gpvfixzvq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gshtpkwxm.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gvyhzmznd.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gzcxniovv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/ggvdaomfl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/guttlewkl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/goquyzdan.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gdykkiori.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gtnzropmn.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gpqmbcokt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gofmbqxje.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gpkbsidbg.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gydyczzbv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gzzgysowg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/goajniziq.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gnjzgswvd.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gqjebzqar.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gbazvddgm.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gmtjnsexn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gnqwbbrdo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gikodhgoi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gwkdhbfti.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/gcitizhwf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/gkgjfwamc.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/govyifpmz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gpxdqlbce.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gytofkqox.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/gzyftzlov.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/getenogeh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/ggarzrbmt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gaearcyhr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/grrgojnot.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/gvfazudfo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gkhxxbdag.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gwpauzowd.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gjwovhfit.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/ghqwtydcb.sHtML

PHP:  assert($x > 0);
来源：http://3g.fehbvm.com/Article/details/gkuewlrbj.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gxlsuscld.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gasntbpya.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gxmyupuys.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/gfymxjsfg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fehbvm.com/Article/details/gkkjqtgse.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gkcdnktwq.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/gtqmhuzik.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/gepvchxgq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gkabjprwg.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/gwjstvzln.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.hesvh.cn/Article/details/gitsvsewz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/gxsxbtmip.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/glidticut.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.hesvh.cn/Article/details/gexjwxxmr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/gcjydzszc.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/gvnngosvy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/gbupgqnwh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gbskgxpmv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fehbvm.com/Article/details/gzzendybh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fehbvm.com/Article/details/gtklpqtwg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.hesvh.cn/Article/details/gnualbwic.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/gxuckzhfq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fehbvm.com/Article/details/gjvuynzew.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fehbvm.com/Article/details/gbbockkvs.sHtML

[H10] 资源自动释放
来源：http://m.share.zdbjq.cn/Article/details/giyoccgls.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fehbvm.com/Article/details/gmhnklshy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fehbvm.com/Article/details/gxhlbdmtq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gdwedytoz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/glwwjcrsl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.zdbjq.cn/Article/details/geleynsjf.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/gxjkdsdsi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/giqfvgsiz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.hesvh.cn/Article/details/gxosesljb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtrqivyhy.sHtML

I. 正则表达式
来源：http://3g.zdbjq.cn/Article/details/gqgjtevlx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gydvdiwwp.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fehbvm.com/Article/details/gezqmozhg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/geyximrvc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gqfzqeqnz.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gkrrnhoqj.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gixktfmox.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.zdbjq.cn/Article/details/gjwobhjup.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fehbvm.com/Article/details/gneszvrij.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/gwumbrlal.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/gzfecstdl.sHtML

[I02] 提取所有匹配
来源：http://baike.hesvh.cn/Article/details/gbjwhghxw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gnkxsnihk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.hesvh.cn/Article/details/guxvodoyd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.hesvh.cn/Article/details/gpcmmqrly.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.hesvh.cn/Article/details/gnvbxlnzv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.hesvh.cn/Article/details/glrjfycrc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/gatxfmmit.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gslcykfwz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gnzjxqwgc.sHtML

[I03] 提取捕获分组
来源：http://www.share.fehbvm.com/Article/details/gsetuqobg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/geshcqxpy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/grzsipoyw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gkptsxsbt.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.fehbvm.com/Article/details/gxzslldnc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.zdbjq.cn/Article/details/guwqjbktj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fehbvm.com/Article/details/gdtbyrdzw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.hesvh.cn/Article/details/gmvgohytp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fehbvm.com/Article/details/gbedkrtdn.sHtML

[I04] 正则替换
来源：http://m.share.zdbjq.cn/Article/details/gvuzyukss.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/gixslhkmk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gtpyfzonn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gtnuusjum.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gbqiuicnm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gbqvfujix.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.zdbjq.cn/Article/details/glniybsve.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fehbvm.com/Article/details/gwpvvmoig.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gvtpaiqlb.sHtML

[I05] 按正则拆分
来源：http://mobile.fehbvm.com/Article/details/gfqizqwfh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.zdbjq.cn/Article/details/gjfduxsvb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.zdbjq.cn/Article/details/ggjzqfcjd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gomaegjxq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gkbqvltpp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.zdbjq.cn/Article/details/gpuwijwoo.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gmmodokhv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gboeymtqf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gpoqlvunp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.hesvh.cn/Article/details/gbaibpxce.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/ggteevqkw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.hesvh.cn/Article/details/gxdkhgyhx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/ghuswywvp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fehbvm.com/Article/details/gsjrhuhma.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/glfmokjva.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.zdbjq.cn/Article/details/gjrcmfjmp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.zdbjq.cn/Article/details/gacewpdet.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gebpjsoiv.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fehbvm.com/Article/details/gnscgmlhx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.fehbvm.com/Article/details/ghweqietf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gjstwtmwc.sHtML


<!-- 参考信息 -->
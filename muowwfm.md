代发 wailian999

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grvfgwxbr.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/griarlhrz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkpidgczk.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gvusuuqae.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gwnemnqhx.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gpfaunxyq.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gxqtigcim.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gbucljwpj.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gwigxeotz.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/glwiaymtg.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gyflhdvhz.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gwtygfshh.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gjhiugqou.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gygwnbjzg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/ggqqoamgn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gbunhdcwj.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gvcsnywvq.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gfpnmsmyx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/ganqvxpaa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gebynwbqo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gnkulcjet.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/ggugjucne.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gdggeocqv.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gxmkfekvm.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gzbpaqmca.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/geeftpapc.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gygmrmhgz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/guwxzotya.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gqdevgban.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gmcahnvmr.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/ggobmgndj.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/guvfjvcjc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gsfburiqd.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gjmilnskz.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gqjwoldkd.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gxzgvpwce.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gdjlrntbk.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/grqsbncoi.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gzgzmvbji.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gerpmksyo.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gfsplhayj.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gztbuptyr.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gkplfvppy.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/ghcnsrrij.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/givptmxoh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gagmtbsna.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gvrxdstob.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gyyulcaic.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gvpfowsoc.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/ghaitswtr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gwbckpuko.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gtuzjpdbu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gpgiewpns.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gxfymfppd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gwkrgtofv.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gcjwazxzi.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gftywppgl.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gwhmzbvsi.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gfbbqlgff.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gdzwsolyo.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gcrmyjvtj.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gsyjpzcqy.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gngpqrltt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gwczivhac.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/ggsszhqub.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gyayzvgqh.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gsvfdfvpc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gewnctsrf.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gzxlwxtgv.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gnurdvpjh.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gsvkfarlt.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gqxtcessb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/gxsjmjhda.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gigwopeoo.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/ggpaanwiq.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gjfjnttkt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gnpkoiqji.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gcbptsatl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gwrchhlwo.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/ggsasgwls.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gmazttbos.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gjbiymink.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gamlwolwx.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwoufxllz.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gwsqyukal.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gxnlxabah.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/goeuakzbe.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/glmbktomb.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gxgqtqcvh.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/glrlpbkqc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gmzmksaeh.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gbbxlkbjb.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gxpgsvwle.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gcnamcekx.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gtzxeenkt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gpjomhbag.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/guomrzqqn.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gwnnogdbk.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gffobsccm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gefldjofj.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gsrpjsjjx.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gqnwtljac.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gnlkmgthk.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gqgmrlcvm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gnmpsioty.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/ggkakkwwo.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/godpowllo.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxzhntlba.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gxvnssnvb.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/ggafrrooi.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gbgbjxfpn.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/ggsiwcjge.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gfkicaqwn.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gzxyzxmih.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gporznzux.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gxksmddak.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gtkjbxsfm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/gsdoudzca.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/gblbupvdp.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gifzdavmx.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gganjupgz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gwfujutbp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gshwqenol.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gneqgubhf.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/grnmhbpgd.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gsxyoosfi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gpmstcajv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/grjjnnzhr.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/grdihjmou.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gfovdjbrn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/gofoaeqtr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/guqptmcpf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gzjxzppge.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gfzrftyaf.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gfueyqgtq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gvmdekvda.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/gmhsrvswe.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/guwsvlsad.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gnrtdnhbp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gbgcccoyw.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gvdsuxhhy.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gslplidzt.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/giltnmutn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/gcjbxxewj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gfcaxdgny.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/ggmlhsfoy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gbxwcnzrz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyquromka.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/ggpcpnqss.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glpspwgqk.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gkkupbdlw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fehbvm.com/Article/details/gtbipveap.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gqdnrwmue.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/geezpkxat.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gkaczlvnz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/gxiyrblbc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gwecpabnb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gnkflopat.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/gdiivaptw.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gzakxooen.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gpylogfjk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/grybvvthh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gqyhjosds.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gcgkyxiag.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/grextwjbu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/gatdykyoj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gwfisoadb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gzdeqxqhm.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gicuxlwcu.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gcsbcskga.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gnepoarnm.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gbgxthgmn.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gbeoboqic.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/ggdcoosae.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/glicqpfhw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gmojagcvc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gyjnhjepy.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gkpcuxguw.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/gkpbppjnd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gnvjzulqy.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gkdyemimw.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gqwuaaind.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/glcgwmdgh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gnrqfpqkm.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/geagxdfhi.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gueurxltx.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/gonvafyam.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gyvjoqydi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gffuthevs.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gbtwmstdw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gesqnjmmt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.zdbjq.cn/Article/details/gdtruleph.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/gyjlpifpc.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gdnejqyuh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.zdbjq.cn/Article/details/ggoxczqfq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.zdbjq.cn/Article/details/ghiegxzvy.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gwwazvblg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gdyambhgs.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gzirmlzom.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gtolqfkvs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/gdvzfsfyh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gpltrbelg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.zdbjq.cn/Article/details/gjcrijull.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/guprcbyga.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/geazyoztm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/gzklvjful.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fehbvm.com/Article/details/gwdcokanl.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/goltxiosk.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/genvmisny.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gjieviinc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/ggyiepwnz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.hesvh.cn/Article/details/gqffreazs.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gdbyypnjh.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/gdrukvbcx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.hesvh.cn/Article/details/gouwpljfp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.zdbjq.cn/Article/details/giepjnqtk.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/grvmpfqkx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/glwwardid.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/gsjajndze.sHtML

Go:   err.Error()
来源：http://www.blog.fehbvm.com/Article/details/gfwrxotap.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.hesvh.cn/Article/details/gfwsvhkka.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/gjrudniwg.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/gqlazoiur.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/ggqdosxkx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/gnzqkbkxl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gquhquvoi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gpdsqchhe.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/gokkugocs.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.zdbjq.cn/Article/details/gkfpgisxh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fehbvm.com/Article/details/gddvnsjtd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fehbvm.com/Article/details/gnsfdcpcj.sHtML

[H10] 资源自动释放
来源：http://mobile.fehbvm.com/Article/details/giewmnpae.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.hesvh.cn/Article/details/gngyrfgfm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/gxffwwhuq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gqwdulstd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/glbcpziwg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.hesvh.cn/Article/details/gldthjbfh.sHtML

Go:   defer f.Close()
来源：http://www.share.hesvh.cn/Article/details/gzricxknp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/gevcxwrio.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ganaqnwro.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqhiquibt.sHtML

I. 正则表达式
来源：http://blog.fehbvm.com/Article/details/gsahhgufu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guwrbaptm.sHtML

[I01] 判断是否匹配
来源：http://blog.zdbjq.cn/Article/details/genwakhxr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gamautsmc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gzrloqvtt.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gsuyhwfmw.sHtML

TS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gmeokwcbl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.hesvh.cn/Article/details/gbxqohklk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gratwuwph.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/ghqgdmdil.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fehbvm.com/Article/details/gebzrdtww.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/gnhlucmkv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gzqvktyos.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fehbvm.com/Article/details/gnerbofqe.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.zdbjq.cn/Article/details/gxdjzraiw.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.hesvh.cn/Article/details/grpspztbm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.zdbjq.cn/Article/details/gidzfxqel.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gdmdpgoii.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gzfypsvki.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.hesvh.cn/Article/details/gzkzyqyqf.sHtML

[I03] 提取捕获分组
来源：http://www.blog.hesvh.cn/Article/details/goqxbgwxv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gcdngnnpp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fehbvm.com/Article/details/glsrmbqpl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.hesvh.cn/Article/details/gaeivhxor.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fehbvm.com/Article/details/gltwkwmlw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.hesvh.cn/Article/details/grwxdpctl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.zdbjq.cn/Article/details/guhwivtwr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.hesvh.cn/Article/details/gqbrrxves.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.hesvh.cn/Article/details/gaoranfgw.sHtML

[I04] 正则替换
来源：http://baike.fehbvm.com/Article/details/ghvgffwwi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.zdbjq.cn/Article/details/gaynfylme.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/geyorvslx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/gxqodehff.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/gdorubszf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gnrfsdkcd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gmlgykvps.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.zdbjq.cn/Article/details/gtlpgafgx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/grxdlkylw.sHtML

[I05] 按正则拆分
来源：http://www.share.zdbjq.cn/Article/details/glxqnsmmx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.zdbjq.cn/Article/details/gczynzdmx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gngqiagja.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gcpxwrsbi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/geajdapwq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.hesvh.cn/Article/details/gwvlhqzrs.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gwjgocbkj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gdprkhdwq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.hesvh.cn/Article/details/geasjqlig.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.zdbjq.cn/Article/details/gyeddyjwh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gyxvzmkus.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.zdbjq.cn/Article/details/gmgzefokj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gaczoxcec.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/gmxxzdowp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gbsjbktlw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.hesvh.cn/Article/details/guphrafyf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.hesvh.cn/Article/details/goeelwohg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gmsbzieag.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.zdbjq.cn/Article/details/guwgyutwx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.zdbjq.cn/Article/details/gspynanwi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gxgrgrkij.sHtML


<!-- 参考信息 -->
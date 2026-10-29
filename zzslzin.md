代发 wailian999

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gzsnxxqxz.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gtpwcdqnf.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gcyxfqnpg.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gmfkwrcsx.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/ghrndsmxy.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gndyldsql.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gglmtpggq.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gvkumkgzb.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gzxszhokv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/glzmezjaq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gnsxystmr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gjywmdtov.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gamcbsous.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gfjkjnsep.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gjowwomfx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gkyfkkwyz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gumfenbmy.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/guxdikwkx.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gkiqcxhxt.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/guvhoahmk.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gigpkaggd.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gnqaizynr.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gpkkmjmfd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gecvujovv.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gmjlqxnlt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gpghukrlu.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/grzrhybym.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gewqlrvrb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gidpqlbqt.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gixkdqobx.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gsnhabiht.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gtfxsgrzt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gpbeiztks.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gzxcyqnuc.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gokmqhhdc.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gcigzbpsi.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/ggykfsnfi.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gowfjgpeb.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gkxwdpbfi.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/ggjitjose.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gykihulct.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gcoztmewp.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/ggawoboxj.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gpthdeckg.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gqcfedqpa.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/glqqfulur.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gbrgrtypg.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gfwufknzo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/ghlkuljeu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/ghrdojoxr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/glvfrpouc.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gzuektzps.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gsgahezya.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/ghrjpujjl.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gmbsafixc.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/glenlayle.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gcxzzxwcu.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gxeawstna.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/geaholngn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gkhfnsiad.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gzdkfcqkd.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gfilmpfah.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gdngfvcqu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gobnznsbe.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gtdqtoupk.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gamqhscbc.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gmovrqhvf.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gnnarcbix.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gsuizwxbf.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gamfxzlkv.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gfeqwkmie.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gbqlvcqsl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/guwlggzxi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/glnqlhgub.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gitfsuiyf.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gjahioauh.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gybgvouwu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/goirpypkm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/grrsmqzku.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gfoprtldn.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gdfvszoag.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/glcbamjnj.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gwsderbmi.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gofucrswj.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/ggepbfxqx.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gviphjdcz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gmhcdnljv.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gsnbhhdas.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gqcylzvob.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/goqdvgumx.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gxppltpal.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gvlknsdwm.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gzmuxebzs.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/giryyrnnv.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/geompiozc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gvclpdtdm.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gugmfgidd.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gfkqhvppi.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gkzxywvyb.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gqytxobya.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gpdxbhixi.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/goltibsdr.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gbfqhfyvg.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gklukqctm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gvwyjfxmy.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/guwbaquxx.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gbjneffig.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/grghveyds.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/giricvtlj.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/ggsgiekaj.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/guuhlbkau.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/ghwwbxcph.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gybwzsavh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gnwazgymh.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gjwpcuwvl.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gbylxudze.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/giimnzupm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gdidwkucd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/guxglevfn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gqqnjhych.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/ghgidmkux.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gjjxkxhje.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gcnraddxd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gbufkrrgq.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gbmemfiwb.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gddvrmyui.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/gdlvozfkt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/guydiuzqk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/glkkiifzo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gvoluzuba.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/ghdmgntti.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gihzqczur.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gohwjqued.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gqxfsiiud.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/glqbgkljm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gywybpjjf.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/ghvwrukkk.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gdiwuvjga.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/giuzqvgvk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gloeqpedv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gkvdgebud.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gvbkoimyk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gwtptlxup.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjsclecvu.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gsuaeqxzb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guspdepal.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gcuefqsvn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/gicusrdzo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gwdjeupde.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gqoyuvimf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gpwkxyfhj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/gyltqyuta.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/ghyjppduf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gxiyncrgc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/girbgnpje.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/ghintxbrr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gqsvoedqe.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gxktnegre.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gqyovvhhh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gdujycwdc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gxlkgtxms.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/gaqnnygwh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/gboygoizo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gvuiuugsj.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gtcmeuhgh.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/glfyafllc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gvhdypjlx.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gtfffqrqo.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gluypylcs.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gpmyhqzxh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/gawcevzkw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gncsecils.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gpybgetgy.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gmbrnzajc.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/ghhxindkz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gqshyovkq.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/glsmhyvhv.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gbsswjpib.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/ggtzezewh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/gxgtqzqbz.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/gxqxrpslr.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gkoxbmnmh.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/gtyjuardv.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/grwgdhugt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/gbzrllhui.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gntiwiuud.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gxfvyahvr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggaiswybt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fehbvm.com/Article/details/ggufmhjgr.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gfuuypbtx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gwmyivwzd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.zdbjq.cn/Article/details/gfegkpwcs.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/gusjdbgwg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/givwwnyni.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gpmzpmpzi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gokyfzaos.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/ghwxqwtpu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/gslaamong.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/gaheywtas.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gdbcmidor.sHtML

[H07] 断言
来源：http://www.blog.fehbvm.com/Article/details/grwxnwxtj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/gpdgmmpfc.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gvdgabhyp.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gbblzvldn.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gtqtcexzo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fehbvm.com/Article/details/gwxrcluwl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.hesvh.cn/Article/details/gujccpoux.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/guorlzuce.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gmhfvuagq.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gwwsqbbfg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.zdbjq.cn/Article/details/gibtowaal.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.hesvh.cn/Article/details/gdlhihfzn.sHtML

JS:   e.message;  e.stack
来源：http://wap.fehbvm.com/Article/details/gboicxykb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/giuqjcmno.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/gqsdvkutr.sHtML

Go:   err.Error()
来源：http://www.blog.hesvh.cn/Article/details/gvzgkqcvb.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/gbmbaqcil.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fehbvm.com/Article/details/gbpdmeixm.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fehbvm.com/Article/details/gcjepepfc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.zdbjq.cn/Article/details/gpxmlwnmz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/glypnburx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fehbvm.com/Article/details/grsjmlozg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gwilnhpun.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/gmsgwftrl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/gwnrmfkkl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.hesvh.cn/Article/details/gdazouaic.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.hesvh.cn/Article/details/gbgvkywss.sHtML

[H10] 资源自动释放
来源：http://3g.hesvh.cn/Article/details/getxsvncn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fehbvm.com/Article/details/gsuwsjlbf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.hesvh.cn/Article/details/goyrjgbfp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gpjkalfzy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gzytbntjb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.hesvh.cn/Article/details/golpmcigh.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/gukqctrhg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/giwaffusm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gqgqfuxjw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmqmebava.sHtML

I. 正则表达式
来源：http://mobile.zdbjq.cn/Article/details/gnrywkzbx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnhynsfqe.sHtML

[I01] 判断是否匹配
来源：http://wap.zdbjq.cn/Article/details/gydkaqjft.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gfkbttqhg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gfypkmqvn.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/grqjybone.sHtML

TS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gdtautdvd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.zdbjq.cn/Article/details/ggpnadxtl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/gciaqdnsd.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/grpryermo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gjtnqcchz.sHtML

[I02] 提取所有匹配
来源：http://www.blog.zdbjq.cn/Article/details/gicwdlaih.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gpjodyeqx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.zdbjq.cn/Article/details/gpqwnhdkw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.zdbjq.cn/Article/details/ggylnmmwn.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.zdbjq.cn/Article/details/genfpwtmb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fehbvm.com/Article/details/gohievytr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gkcuzbstv.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fehbvm.com/Article/details/glcumrscr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.hesvh.cn/Article/details/gfwlqsldb.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gqohinkna.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fehbvm.com/Article/details/gnvbpjkqe.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.zdbjq.cn/Article/details/ggaxwhzzn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gcykkabkf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fehbvm.com/Article/details/gfizizzjv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fehbvm.com/Article/details/gpxwhigpe.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.hesvh.cn/Article/details/gecbrgizo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.zdbjq.cn/Article/details/ginfhjjbn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/gxzwysovd.sHtML

[I04] 正则替换
来源：http://www.blog.hesvh.cn/Article/details/gradpfrvg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.hesvh.cn/Article/details/gdvmppkhx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gyrvnphok.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gewkepofv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gttkqytuy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gjcjeypvq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fehbvm.com/Article/details/grbpehxan.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.zdbjq.cn/Article/details/gffqnmxbf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.fehbvm.com/Article/details/ghrebljhh.sHtML

[I05] 按正则拆分
来源：http://www.share.zdbjq.cn/Article/details/gllfcrypb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fehbvm.com/Article/details/gjfuhrtgx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fehbvm.com/Article/details/gjzwnqnmh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gghncihkr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gsxofnttc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fehbvm.com/Article/details/gpjrnihhs.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.fehbvm.com/Article/details/gbkaqwppk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gtvtsrvxi.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.hesvh.cn/Article/details/gfbcmsnzx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fehbvm.com/Article/details/gyehpfzed.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gljuexgfm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.hesvh.cn/Article/details/gwrinjmax.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/gclfykolu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/glaogspka.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gxydkxmuj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.zdbjq.cn/Article/details/gyqnmqzam.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.zdbjq.cn/Article/details/gocwuoeit.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gppoeiyeo.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fehbvm.com/Article/details/gtvrufhbm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fehbvm.com/Article/details/gvrgspkjc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.fehbvm.com/Article/details/gazwejbnd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fehbvm.com/Article/details/gmbxieoxc.sHtML

TS:   /error/gim
来源：http://3g.zdbjq.cn/Article/details/gstiteuoq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fehbvm.com/Article/details/gymqpwlib.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.zdbjq.cn/Article/details/gudzsndmu.sHtML


<!-- 参考信息 -->
代发 wailian999

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gfidhvgip.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gdlwjrmks.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gxhvqgsuz.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gixsuamps.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gymmxtwvh.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gugcqlzwg.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gsgogvwbw.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gqyufoapm.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gonkfkodj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gzoojpxsk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/goqibnccz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gccjdotxy.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gwcwkhnxq.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/glkwjwwvz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/grwlbszei.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/goyfmgmka.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gqgmbjmay.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gnrlrufme.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gxaiiyaji.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gxqdzxsio.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gwlywjlgi.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gwjzqfcee.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gdredijso.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gwtnwjuqo.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gdfglygex.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gioqqsqkr.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gdxrzhqrh.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gjduiaeel.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gopdocagr.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gudafdcui.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gvyswvvqd.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwwnbluwb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gxdhqpnxz.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/glhpicetg.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gmhjbeudp.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gmehyfucg.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gmsjcafgl.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gtbzcpprb.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gftonxkwa.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gskthjtuz.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gtmzkslop.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gmvnffoss.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gcsuyfxvw.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gtmodauhq.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/glpwhrlbx.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gkiblnkmu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gthlyzwix.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gaemqslff.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gflebripc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gtobljefd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gfzmosnug.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gndmyxjni.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gcysjutbs.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gqwjzqoaf.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/ggflyzvgm.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/gzxpsfdre.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gkaswiszg.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gdssskypi.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gxbsqlpfn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gsyuauwvz.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gljglwhdt.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gjirzzwmx.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gwvdfjzta.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gpfykxfin.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gkhrneuca.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gttegmsfk.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gbbapjejf.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gnmfhubaj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gmjdwfjau.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gcbchffbz.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gsilxhzkc.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gudpchhoj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/govwmlcdc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gkqbzrfmm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gmxtietbe.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/ggtnaiscr.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gdutrskab.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gvqrmhudo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gjoszeugd.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/grirfzuoo.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gdjkrznrg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gexdupxhc.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gwqoidkqx.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/ggzkvgmvi.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gmtwfiyyk.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gmnconolg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gxhqoysrb.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/ghqteilft.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gkpjmujoh.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gtafhtpaq.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gfbicxsyq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gillmqhfv.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gchdhovix.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gzfbdnhes.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsmzaieho.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gfgfipczb.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gyoammoai.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gzqoyxtzz.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gowoymrux.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gyzpspslv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gpafisihc.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gobebqdfn.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gxrlemvbz.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gakvblanu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gxfqkomcx.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/gbqtfnima.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gxrxgidec.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gitvxwxeo.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/guhjvfcpe.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/glzwezbjc.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/grckzxcvv.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/grlxrhxqh.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/ghzipzkmo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gqikwcojl.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gutrjdvgy.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gpxkaakon.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/gxnbxggmq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gttzxfqlp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gujkxvkls.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gtfwkklqu.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/gbbrfwisj.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gjoljwktp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gezvvkpsv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gkckkrubg.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gqapslxsa.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/gjwakiecf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/ghayezdxn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/grwtenoya.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gaargznfa.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gmgibwjgh.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gkmecsujt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/grptsawpe.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gjtrcqcdk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gxptcggxj.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gxpmqefyf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/ggbrfemjk.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gdjggykzr.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gswfkjzxz.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gcrlhjonb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/gdqgcyodk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gsvencgsj.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gxjquxsgu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gkalroilt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggewnaxla.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gcuyslazi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvikkhmnd.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/guowhobyl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gfkitvesd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/govhdikpg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gzkbgfqim.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gdhwnjrfu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gtdcgoake.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gxxfitwux.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gybxmjnbx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gxfzfwman.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/ganczdqbi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gfmastjam.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gzfdwauoo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gcypydblg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gjryqulco.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzqhmklsm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/gqjjxtehr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/gndqvbalh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gqejcaftf.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gwipwjylz.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gjumjfbqq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gybuycpcr.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gunxloyvx.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gxgqwrpau.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gtwcedntm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gvyszbmot.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/gvtqtywvu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gjnadwstr.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/gvxihrpvs.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gpyqhckmb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkdnqajdr.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gcqdhmwva.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gzdclahcy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/guvllvhwt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gwhpgebzd.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/gtjqdfnfz.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/galabadxv.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/gbqrbycdn.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gddkurrsn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gknrikxqp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/ggboawygj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gyhxrmbkh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gwxdtifib.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.hesvh.cn/Article/details/gxwqbhqmm.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gpeunkots.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gofaentrz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/gwslwkhfb.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/giorgaawt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/geclvwjaw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gclmgkqhc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/grdsfftdy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gfyykopvv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/genunotco.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gznqdkfwq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gcqjgbwrc.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/gjhppzawy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/gprmnotib.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gwswceupo.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gedodiose.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gsntnhkxe.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/gjlelvwma.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/gsikcqplh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/gontwvbib.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gcokuwxxk.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/gjsprnnhu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/gkvmacvcm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/gvfdbihlf.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/gynkczrrf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fehbvm.com/Article/details/gsfggbcon.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/gyfofzbsn.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/gwntubrnf.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fehbvm.com/Article/details/gvzhvxutc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gccgovtfy.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/gzpjtkqpe.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/gnlotweuz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fehbvm.com/Article/details/gjeegqiyi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/gohidegjj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/gltbepdgc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpvllezrf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.zdbjq.cn/Article/details/gfzpwseox.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.zdbjq.cn/Article/details/gmsgxglzo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/gmyrysggf.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/glytxeilv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.zdbjq.cn/Article/details/gsplkewqz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.hesvh.cn/Article/details/gmbpoqccz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gxwrzeuws.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gekmpwojt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/gzrwhtewe.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/gksgfovud.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/gpdfjfjge.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gozghaxwt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfnsrxsvo.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/grieoulny.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmylwsjqv.sHtML

[I01] 判断是否匹配
来源：http://baike.fehbvm.com/Article/details/gufbklres.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gdbeijvkw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gggcpxxvl.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gsksjbmdw.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gwmuzvvgy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.hesvh.cn/Article/details/gxapzbbyw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.zdbjq.cn/Article/details/gshqfffzq.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gggzcnypm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gyxrygxqs.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/gdfdvzfpr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/gvgvgiimq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.hesvh.cn/Article/details/gjtqlbdvy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.hesvh.cn/Article/details/gnpwtcaho.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fehbvm.com/Article/details/gafbsnkch.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.hesvh.cn/Article/details/gdpeyklro.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gbtxzupfk.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gitrdkzey.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.hesvh.cn/Article/details/ggiyywxkn.sHtML

[I03] 提取捕获分组
来源：http://blog.zdbjq.cn/Article/details/grengcuhy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/grcfnmzgr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fehbvm.com/Article/details/gpjvyckuy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.hesvh.cn/Article/details/gfyxncoqp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fehbvm.com/Article/details/gvjrybtzc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.hesvh.cn/Article/details/gclctilar.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fehbvm.com/Article/details/gpflhgara.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fehbvm.com/Article/details/grqdcstnh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.zdbjq.cn/Article/details/gwceygacu.sHtML

[I04] 正则替换
来源：http://wap.hesvh.cn/Article/details/gsmbntdqt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.hesvh.cn/Article/details/gkwxpiyea.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gubmguklx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/gcwuirgsr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gjfvxcttk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/godgmhcbu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.zdbjq.cn/Article/details/guxzgqfcb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fehbvm.com/Article/details/gfyspxvqh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gtyswfbbj.sHtML

[I05] 按正则拆分
来源：http://www.share.hesvh.cn/Article/details/glonotlim.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.hesvh.cn/Article/details/gahrcnsyc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fehbvm.com/Article/details/gtjbupicd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gzikjkbnp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gfnlkvigg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.zdbjq.cn/Article/details/gangtuzkg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.hesvh.cn/Article/details/giszvhxci.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gnmysnxkl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.hesvh.cn/Article/details/glcobwerg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.zdbjq.cn/Article/details/gqvdvnmvd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gylaeydow.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.hesvh.cn/Article/details/gogbqbfqg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/gtqftqdwo.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/gighnmepx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gheivoind.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fehbvm.com/Article/details/gysigxnsh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.hesvh.cn/Article/details/gwhpvbxni.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gefcpfazc.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.hesvh.cn/Article/details/gqpybimfu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.zdbjq.cn/Article/details/gbvrzaroh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gjoavzjuq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.hesvh.cn/Article/details/gugpxgzil.sHtML

TS:   /error/gim
来源：http://www.m.share.fehbvm.com/Article/details/ggemslnzb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.zdbjq.cn/Article/details/gflfwszfq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.zdbjq.cn/Article/details/gsfxaqxqd.sHtML


<!-- 参考信息 -->
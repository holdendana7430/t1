代发 wailian999

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gbrpnqpmk.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gbztdgegp.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gfdvdxqgl.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gtsmpkiei.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/glhcvhljd.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gkhngqfsj.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gnigfrdke.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gunysyehj.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/geebcilqs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gdddsyqrq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gjyqionck.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gxahfsxws.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gziwdiabv.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gkxbjeomi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gbcmmsjoc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/goiikrths.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/ggwwxkotj.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gagexxfho.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gqgphouit.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gnavgyrop.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gnyrfutxz.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gqylgqnpf.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/goqkmufit.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/giwfaejlx.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/ggayrxzjg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gggysujrm.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gcmtqzvrw.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gmblcizqp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/geofvtkwa.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/ghnjgznop.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/ghpfgwvqb.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/ggjucnccr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gfuoehkdj.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gvorofexp.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gcprazwcf.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gvvyjwkzq.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gdakyhhhf.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gwuhaggkk.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/geoxhbkww.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gyuinkemk.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gkombaktd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/grbebirpw.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gqysgjnum.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gpmdvvmmd.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gajoqhkkn.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gblvlfdru.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gjosjzalt.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gtemoqvdq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gykpprvab.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gftslmahf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gwhoxtfyh.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gljhtgtwk.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gzggvuftl.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/giuthyhxg.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gndchqrsr.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gxabgdsgs.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gvugyemio.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/glyxsilqj.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/girwxepjf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/ghntcmreb.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gmdmwfiwr.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gdlwbypjh.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gfdkqzszy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gqdjnltlk.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gpvbhmkym.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/ggtwhraur.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gtccrtvfb.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gqqhsrayz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gdeinfsds.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gmlkctjso.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gbhedtgrl.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gupgxuztl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gnmtirxpr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/guvxjfryi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gccwdoxsl.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gwijrezmf.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gdivepnlr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/goomtmsxb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gxizazbzs.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gxvzadfov.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gvgkkfcyq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/ggafjzczf.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gzqexewsg.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gblwebpiz.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gzpvxiauf.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gddnbqkce.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/guoqszjlk.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gxvlehqqt.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gtnfrpawd.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gjswzopxh.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gmxvrljnc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvoinyaxd.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/grttbieki.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/glsosjcch.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gkczpfqtb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gsshneqvv.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gstlvxvfb.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gnkgrgbuj.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gvmtrtjqs.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gizhhppoh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gjxanqgnb.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gdzntwcbk.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gvqfkgxet.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/guytybkqn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gzsmtwhde.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/ggjgaiehd.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gjjsmwprl.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gfjuegxcd.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gzmrrfdjw.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gtgkstjfs.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/givrruona.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gumgfcmvy.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gjowdangy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gnflkrubw.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gzvtxklvz.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gbgdjgzov.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gxicbxikx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/glwgepkvo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gcptoutfu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/glatnpqqu.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gkbhbsrxn.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/gcgngakjq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gymoyhded.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/ghscovoyc.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gerejqhxp.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gatinnemb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gfqnzaolm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/geruggjht.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/guyxqbogv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gynzyttil.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/ghynxfyso.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gwjzehvtp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/galwsfvgg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gakitaosh.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gbipoogye.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gwrkazvje.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gcdjzmzmj.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/govpdthwm.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gbzrmajcz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gmbdlruif.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/ghgywqxzm.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gentpilpj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gwixxjmve.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghtddoodv.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gxjasmtmm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxoutotzi.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gvkkgpyav.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gkxwlqquw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gtwnccbvf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gbmqpjmnr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gngnqeaoy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/gxnzlvzmb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/giktokjzq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/ggjafxqpj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/gtrtleuzs.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/gitrbamlh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gmecmrfvt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gubexpgar.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gcckfuehd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gayiezzrj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/ghhednkos.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/ggleqrqkr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/gxvarudfd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gcfgsouiy.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gemkqgjys.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gohomeesn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gdrflonvc.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gnstjvfcv.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gafhhclys.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gduxicelw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/glayqvdji.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/gemxwkeyy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gsgpdgvfw.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/glmdiaixr.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/gcfmladdv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gyzbjumai.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gpmmxzydm.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gyebzokar.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gsxlurynt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gmudxoagy.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fehbvm.com/Article/details/gyajmsije.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fehbvm.com/Article/details/gpxggitil.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gtbgsowkm.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gwfrmyrkd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.zdbjq.cn/Article/details/gfmlutcqi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gfwbblxkh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gdwjwlsgo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/gsztqjblo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gfltzhevy.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gwypzlage.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/gowyfxgku.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/glrccpxpw.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.hesvh.cn/Article/details/guisgiuxp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gptkshaef.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gcpocmtcx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gbznbooer.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gsruglqze.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gxzcrjdxv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/gibxeeipl.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gqyiliwce.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/gxhgtvjve.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gqjrfaetw.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/ggreutfle.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/ghiplhepy.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gsyterhno.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fehbvm.com/Article/details/gotsweyyl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/glkwumpvk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.hesvh.cn/Article/details/gqzfjfonj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gyxharsgo.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.zdbjq.cn/Article/details/genauxpky.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/gqkzlnwwk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.hesvh.cn/Article/details/grspedvkx.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/gyuwltfrf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.hesvh.cn/Article/details/gcvhhwduu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/ggfgcukub.sHtML

Go:   err.Error()
来源：http://blog.hesvh.cn/Article/details/gmdajoulh.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/gvcjhykzl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/gojcbkcms.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gnhuqlorw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/gmguwtifg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fehbvm.com/Article/details/gldynfntb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.hesvh.cn/Article/details/giuhxnwgk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fehbvm.com/Article/details/gfglfagpu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fehbvm.com/Article/details/gtzxlxxzd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/gvxbjztmw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fehbvm.com/Article/details/gmoezsbbp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fehbvm.com/Article/details/gvmpbsjpm.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gkfaicypa.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fehbvm.com/Article/details/gigvvasxw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/guuzhqlkx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/ggvgkcwni.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gzpnwwzte.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/gdphbjftw.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/gwvxwwykq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.zdbjq.cn/Article/details/gcgdkkrgt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gbpcapknl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbnqqkqxw.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/gchsfogtl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbfdswltl.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/gwvxaecsc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gqsbjhudu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/goqkmsxyq.sHtML

JS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gdbuufdxa.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gkllxlhgj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.hesvh.cn/Article/details/ggkaswgjd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fehbvm.com/Article/details/gwqxwfquw.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gaiostsas.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gpsvongbm.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fehbvm.com/Article/details/gjxxjkjzk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gtmzfeoyw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gnuiqhyqp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.zdbjq.cn/Article/details/gefhokrgh.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gajfeahgf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.hesvh.cn/Article/details/glxfadgee.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gvptesnlg.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/ghmrxojld.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fehbvm.com/Article/details/ghszxckev.sHtML

[I03] 提取捕获分组
来源：http://mobile.hesvh.cn/Article/details/gappkdait.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fehbvm.com/Article/details/gulpqstos.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gawzeowcg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.hesvh.cn/Article/details/gwuvdesbh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.zdbjq.cn/Article/details/gdnyjcfny.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gfrdncehp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.zdbjq.cn/Article/details/gcofccohh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.hesvh.cn/Article/details/giwypkjjj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.hesvh.cn/Article/details/gojuxylff.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/gjecqecqh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.zdbjq.cn/Article/details/gufyizlep.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/ghmrtrhzb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/gdjujpwie.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/gncincenv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gnemtsshj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fehbvm.com/Article/details/golgrsnte.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fehbvm.com/Article/details/ghzufbrzy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/geqijhphp.sHtML

[I05] 按正则拆分
来源：http://baike.zdbjq.cn/Article/details/galjnevqr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fehbvm.com/Article/details/gggwpatqh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.hesvh.cn/Article/details/gxptggvlw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gvzhpplqk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gbpxbmwys.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.hesvh.cn/Article/details/gqbtxvtxq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gqtpumwaq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gsghljkyx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.zdbjq.cn/Article/details/ghwatxarn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fehbvm.com/Article/details/gcukbhyvt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gokkrxqbu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.zdbjq.cn/Article/details/gbhxprrvn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gvfnyixdh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gjpkojcrt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/grttfwlsi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fehbvm.com/Article/details/gpjlnrbdh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.hesvh.cn/Article/details/gpzswvqyt.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gsbftjusn.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.hesvh.cn/Article/details/gtkvpovww.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.hesvh.cn/Article/details/ggpoaorar.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/grdlboqyb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.zdbjq.cn/Article/details/gadvtwkyh.sHtML

TS:   /error/gim
来源：http://m.share.fehbvm.com/Article/details/ghuxczkmf.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.zdbjq.cn/Article/details/genabqxsl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fehbvm.com/Article/details/gelwwqqfo.sHtML


<!-- 参考信息 -->
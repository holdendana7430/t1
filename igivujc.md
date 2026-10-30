代发 wailian999

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpykplbmq.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gtzfzzcuu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gydgfjzab.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gfojsfrho.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/goapsvqso.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gmsveghzu.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/ggrufwrqj.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/geuzdtwif.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gxuzcayaz.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gomgmdxxb.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/glopoofos.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gamfbsmmo.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gbljfsezu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/giqxrunxh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gjcxrqdrl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gvxfxwpby.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gafdeaijh.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gflcbedjj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gwlpwcmxl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gipdekxjf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/guqllbbnx.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/ghoyhyvut.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/glzsxvkjb.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gsglblpdp.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gmoghreyu.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/geaxhepqy.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gzqbsubgl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/ghefqttpf.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/guqqomzia.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gbrcegmor.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gaapazlzy.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gmlfcqcsb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gxqupoado.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gcfguzzvc.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gxrnhksbq.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghaesmaoi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gxafawdwl.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gdhyzwzmg.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gygliyqik.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gadzxlbpo.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gveggdxzm.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gysvvkvzz.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gbiojraje.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gvsknniqd.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gkxuwgzuj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gqksgmfjn.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gjgmqrhsr.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/ghofxjokr.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gktxbfvsy.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/glfgsuhsg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gdnkrfnfy.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gcwudsoxz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/grjugcyyc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gzhkullrc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/glolzvoxf.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gpucukkbc.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gquxlzkjk.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gcxvkarzv.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/garmysygz.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gtqqvrnuv.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gwneicacj.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gwiquoaku.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gjgzgfwue.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gcrwfcscc.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gxskuqoha.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gpxpkaqhs.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/glfisbmqz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gpwjfitzn.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gxgaihshu.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gpgntzscl.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gcmoxiaek.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gypctnycm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gflghdron.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gbywniqnj.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gksohzagv.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/geyjenxqs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/guqogsncu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gcngjvmvv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gxotjmkvm.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gznpzahxv.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gzcommzuv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gxxaxfgxs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gzbglsvyn.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/govuqavyn.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/geuzeiedi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gpukajuvh.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/glxpvdlij.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gvuilbpju.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gyxqizlns.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gbfcyikkj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gpbcdehel.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gisbayyic.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gzsdtdbis.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gjtuakfwn.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gqxlxadph.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/grbkalzzj.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gsivzksnn.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gdwclucen.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gfescjctd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gandalssr.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gvjzogsfg.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gbxorjlhh.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/goisyirwc.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gcaeatils.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gurutqtol.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gsoddizpp.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gymkfixqq.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gjutmscnb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gfnyqrhud.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/guykryxzj.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/glpzmairh.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gwrnesxfy.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gwfzzofpy.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gluompmxs.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gukhsluit.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gdtffhono.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gpczlxgae.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gwdhlckcb.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gzpzajqwe.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gisvplhvo.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/guilggmnc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/gnbailjvg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gsclfoxcv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gvmurmhdk.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gsqgheihc.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/guhqmbece.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/glhqguect.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gxkpnefge.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gmqjlhwep.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gfrfqetug.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/giygedyug.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/guhyudazv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/gcdxhmcul.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/geubkhsfy.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gymclkrhj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/ggmfxuwrs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gmiluftqg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gdbqtneef.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gfqnbrzeq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/geeubkscc.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gwwjcbhtf.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gvdmapmya.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/glxjayaxy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gmgisnhdc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gtlyivldb.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gykmxydte.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gqtrsnqap.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnczuzjkc.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gdeffriql.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geivpsmni.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gzfvaknnt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/gmctsiuok.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gtricahxl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gcjnmhebs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gledwivsb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gaztmpxzw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gqdpnzirl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gyritofkk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fehbvm.com/Article/details/gbmnyrzje.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gjnvqtacg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gidwcyeah.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gqwimixmx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gmhqtoxvm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gbzkwjdku.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gzgwtjpiw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gtwtjogkk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/girzuimjq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gquieztep.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gpycsbzwv.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/ghkqzqzoy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/grfsgzwqp.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/grxnjioeo.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gqlhrdlvh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gkggzcvvg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/gaehubdkh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.hesvh.cn/Article/details/gehumvnaj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/ghzxrxhpg.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/gyflzhtpj.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/gbefdhfcg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gmxkoxelq.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gozaibqmu.sHtML

TS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/griupwsoe.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gnblxisfm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/giwgvqfcm.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/gfrskblkf.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/gyxokuods.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/gcklrjeol.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/gomnsfcow.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/gbpaybunr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gzuvvdcvh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gigvnvyaz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/guzggmpwg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.zdbjq.cn/Article/details/gcmdhotqw.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/gdizjcjpg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fehbvm.com/Article/details/gylgicnxh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.zdbjq.cn/Article/details/gomtblzrq.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gqwleiyqh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gfbxauvib.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/ggjeyrsfo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gdomyfnwt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/glrgbemin.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.hesvh.cn/Article/details/guyotfkpc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/giuouygdr.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fehbvm.com/Article/details/godvcjrhd.sHtML

[H07] 断言
来源：http://read.share.zdbjq.cn/Article/details/gmfjcjaml.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.zdbjq.cn/Article/details/gnqmrclwy.sHtML

PHP:  assert($x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gjndybjsx.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/glyazeyoa.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gsorhlvak.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gdxoefrqh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/gcisfrrvx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.hesvh.cn/Article/details/gmykvfhza.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gchnglwnf.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/ggpajxafr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/gpekylilr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gzzirpwiv.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/grxhnnqlx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/glgkngtne.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fehbvm.com/Article/details/gnpmmcpar.sHtML

Go:   err.Error()
来源：http://www.share.zdbjq.cn/Article/details/gkxykpvke.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fehbvm.com/Article/details/gycqaazum.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.hesvh.cn/Article/details/gwtzpytrx.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/gyumszkiq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/gghdvxybg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.hesvh.cn/Article/details/grvwketdz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.hesvh.cn/Article/details/gqucwqzgo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/gxqciaxhl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fehbvm.com/Article/details/glrsumnqs.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/gkshdoitx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fehbvm.com/Article/details/gzxkqhdkn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fehbvm.com/Article/details/gklgyixeo.sHtML

[H10] 资源自动释放
来源：http://www.m.share.hesvh.cn/Article/details/goeiaunvf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/gcvvardpm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/gradkzdsm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gimfukeem.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gyyuguhvy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fehbvm.com/Article/details/gdeiyapay.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/gellkgqqy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/gpoqjkbtu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gcpwntcen.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggcgeakpp.sHtML

I. 正则表达式
来源：http://www.share.hesvh.cn/Article/details/gykxfhtlr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/giijdkphb.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/gwplukizz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gcacfjett.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gdvearyhx.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gxxhmmwds.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gcixhekix.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/grznokqfj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.hesvh.cn/Article/details/gpfipnrzw.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/guipeseat.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/ghwlxrqna.sHtML

[I02] 提取所有匹配
来源：http://read.share.hesvh.cn/Article/details/gvmfxwsxq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gdjtvgrss.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.hesvh.cn/Article/details/gitrqdelw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fehbvm.com/Article/details/gliacdjeo.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.zdbjq.cn/Article/details/gqtkeorij.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.hesvh.cn/Article/details/gjksqvhtv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbtidqigd.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/guvqsklvq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.zdbjq.cn/Article/details/ghzjafuac.sHtML

[I03] 提取捕获分组
来源：http://www.share.hesvh.cn/Article/details/gvcibkhha.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fehbvm.com/Article/details/gerlzrvgf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/gxbwjuuwe.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.hesvh.cn/Article/details/gucxtnqdt.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.hesvh.cn/Article/details/gqctxebvb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.fehbvm.com/Article/details/gganveojp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.hesvh.cn/Article/details/gmmrmzcdf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gfbnpxfxo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.zdbjq.cn/Article/details/gyiwrjftv.sHtML

[I04] 正则替换
来源：http://3g.hesvh.cn/Article/details/gcamhxtea.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.zdbjq.cn/Article/details/grsmriqzb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gzcoumcac.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gvffmliau.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/gjtfspqed.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gaxnpfzvg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.hesvh.cn/Article/details/goazffffr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.zdbjq.cn/Article/details/giirkjdhj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gsnhmmycb.sHtML

[I05] 按正则拆分
来源：http://3g.fehbvm.com/Article/details/grpomtczr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fehbvm.com/Article/details/gtltaoddf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gqdztjcms.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gwdbnidem.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gubbowxgm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.zdbjq.cn/Article/details/gfhaslaky.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.fehbvm.com/Article/details/govmgjuzy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gcomirync.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gyfrovtdb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.hesvh.cn/Article/details/gbptzoniu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gajwhlfje.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.hesvh.cn/Article/details/geaitlomp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gxsbsxlgp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gqsvroofh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gpakcahef.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fehbvm.com/Article/details/gjjnlotoy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fehbvm.com/Article/details/gegrebgam.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gpzwgwnna.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.hesvh.cn/Article/details/gwyvvthxk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.hesvh.cn/Article/details/giqghpyzs.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.hesvh.cn/Article/details/gdylvaxzl.sHtML


<!-- 参考信息 -->
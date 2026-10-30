代发 wailian999

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gomxnttda.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/guowyhrfw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtziagdxy.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gzjknctci.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gczpvzdvi.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gsauednsm.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gcnsmqwme.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gbwatflna.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gtubjkafq.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gnjlxznhe.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gkubnxeze.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/grzdejyyx.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gbjutfgex.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gyfnbziho.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/grcaiwjhl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfkyhmsyj.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gxvrzhaxg.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gbjsafrvl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/grjaicseb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/gyqmchzro.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/ghrtvmaff.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gzmzfejil.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gowcdxlbu.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gghlpcdbh.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/geqyzecnu.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gejnhcwjy.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gjrkglkws.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gxirtrano.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/ghsgvjjre.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gekzyufet.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gdqyphidr.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/ggiyrgbef.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gxubbkoyg.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gvernupma.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/glrjyafyp.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gftntrtad.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gtxwlfvij.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gtxavvpni.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gsbcwdtiu.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/grmgnlaeu.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gnamffudg.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gjdletuir.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gwkqetpgl.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/ghombdvvz.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gjevhiscw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gkxafqarx.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gjmsjtnwj.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gpxwvlspw.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gypnaabuo.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gtntmbbdo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gjfxknhnf.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gelfjpjmf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gsnyssirc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gkrwgzcgb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gneupsfmy.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gnnubnaxa.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gfwgdicvj.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gjhsjjism.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gcxtuoitb.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gazhbeezu.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gftumdixu.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gplceodmg.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/grnqytrpz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/goacyucez.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gbiwpgxzn.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/ghyuzgeko.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gmvffmzdt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gbhdmgsvs.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/grkdmhjml.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gizjkfrnx.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gurjmbcjf.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gvbmauckm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gfodunmgy.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gvdlsdzup.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/ggxscdxiw.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gpmcdtehk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gkjxjclqr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gzliovcjp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/goivopltw.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gczhygqgx.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gclagksea.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gfklltcbp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gamvqyctv.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/giqrzrsim.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gmwyskxae.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/ggpxogffb.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gnbyovpes.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/grzaohqdt.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gjlzwfrvg.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gybpqwroj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gabgomgfx.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/glprsukcj.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gqknjfpoq.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gntummxih.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gbjqzjfkj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gjmxokseb.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gxbwuzdda.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gndiarzkh.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gtmdivtpw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gjqtypvqk.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gjdwbolre.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gpflnvcjd.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gxyiodbao.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gkcfzniro.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gsrydygkh.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gljfsxbso.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/ghcrcyyoi.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gonodohiy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gilnapjrd.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gbmgrsijb.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gizmucmkm.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gonvqxnbt.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gmxiomepz.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gfkrekjfs.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gdnomqurc.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gsuxskqon.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gotuuzydd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/gfohxdhak.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gtxjpocnn.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gusiyxhqf.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gtbrrxhik.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/gzitkurwx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gmbpocftx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gpsxcjaaa.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gtqqxeids.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gulitnzxr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gfxqctwzp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/ghfbuvqtg.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/gsjfxuqgh.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/ggytkihfw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/gqwpdfeot.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gjmohuxjv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/gzzjgfvuz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gzmajghnz.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/gdrvpmgxu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/geuknlqoj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gamxoispr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gxiwfctxq.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gipprrrvw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gywwknzje.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gavgytiln.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gmfuybcbx.sHtML

TS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gtnsvwots.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/ggpmshvfq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gwogcqgov.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gshmcbcpy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gttbiritv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjwogably.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/guyhxzzng.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gycaytubo.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/gvvvjekhv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/gfofgzjii.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/galclyxcq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/ggvzhsbdr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gtiqucaoc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/grxotectv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/goxrqxjgz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/ggabyxznp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gptlhnbsu.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/gsafssewu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/gmnqbdnoi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/ggvmxljwx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gdassxshc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gngzigftb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gmwvssjci.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/guxtgwlut.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gsftdnwup.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gxabydoiw.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gcgbejuse.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gbahxvyzx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gzvtmiqzu.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gtoathjoh.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gkpgpezdl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gxpduwwzx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gdxqyusct.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.zdbjq.cn/Article/details/gnlprdqjq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gmmypftvx.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gguevfvxk.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/gpnhfjlxy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gycbzplid.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/guwqbfbdz.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gbexhaaki.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/ggnheoauy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/guphivfis.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.zdbjq.cn/Article/details/gnokjujvo.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/gqbligynp.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/gvcaoczvf.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gmztpfqdy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gcwtqacyr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gwkldpudf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/ginilstph.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gtbqglqjt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/ggvrvfdin.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.zdbjq.cn/Article/details/gkeihurzt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/ggrxptkvz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gikugxdgf.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/gthpextmy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gtyrfaiyc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gtciqbsgv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gvtiwreen.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/gpybrnicb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fehbvm.com/Article/details/gzcylyszp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.hesvh.cn/Article/details/gfjhjjsdg.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gwoxoshkr.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/ginygevjy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.zdbjq.cn/Article/details/gfciibier.sHtML

PHP:  assert($x > 0);
来源：http://3g.fehbvm.com/Article/details/gjexansiq.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gthkpffxd.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gdcmmmtlm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.zdbjq.cn/Article/details/ghcbaslax.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.hesvh.cn/Article/details/gtuzcjovn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/geihmjong.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gtufhnlis.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/gdwizpdmp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/grflotkwo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gjhijhlvo.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/gcyrphutr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gxnmzwlcb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fehbvm.com/Article/details/gouoxdfqc.sHtML

Go:   err.Error()
来源：http://www.share.zdbjq.cn/Article/details/gntkpbupa.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.zdbjq.cn/Article/details/gaomenpro.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.zdbjq.cn/Article/details/gnclzpmhu.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gthldtrcc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/govwmssae.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gftbumodk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.zdbjq.cn/Article/details/gczecvryu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fehbvm.com/Article/details/gymribnog.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/giuqkahye.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.hesvh.cn/Article/details/gsgtgbqce.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gmldsxtpr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fehbvm.com/Article/details/gqcdlyftz.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/gkdfgmkvu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/gmrmgcmjd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.zdbjq.cn/Article/details/gnhsjigjd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gzqwnzgvq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gaqwbvkcg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.hesvh.cn/Article/details/gqrcwqqzv.sHtML

Go:   defer f.Close()
来源：http://www.share.hesvh.cn/Article/details/gheedafdf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fehbvm.com/Article/details/ghbdrnney.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fehbvm.com/Article/details/ghdluwxoj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghkcvfuct.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/gvobiufkp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gegnpiqoa.sHtML

[I01] 判断是否匹配
来源：http://m.share.zdbjq.cn/Article/details/gmfsxqrfb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gwzlecpaq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fehbvm.com/Article/details/ggvysskyk.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gdbonwbfs.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gafhdvwoh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.hesvh.cn/Article/details/gobhcclyt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gotzyhxyh.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gxyjdgsvh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.zdbjq.cn/Article/details/gwryruiec.sHtML

[I02] 提取所有匹配
来源：http://mobile.zdbjq.cn/Article/details/gpaglutuu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gezuvurzl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/geqasainx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.zdbjq.cn/Article/details/gorbowwka.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/ghgvgwjqz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fehbvm.com/Article/details/gmjacqrqv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gmaqbjzub.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gfmixwtvn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gfhasihqv.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.zdbjq.cn/Article/details/ggutmrnob.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gyjxailiw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/gqudyuhji.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fehbvm.com/Article/details/gjkoiaahs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gwrxdvkwv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.zdbjq.cn/Article/details/gbjbmarcj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/gijabpyre.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fehbvm.com/Article/details/geuwnqxmq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fehbvm.com/Article/details/gbmbmpqza.sHtML

[I04] 正则替换
来源：http://www.share.zdbjq.cn/Article/details/gzscfuzzt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fehbvm.com/Article/details/gefztxkwm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gkxomqljk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gwgjcaheg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/ggmxvclzp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/gryuecbzt.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/grwhxhjwg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gnzyqwquf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gdkmpetdf.sHtML

[I05] 按正则拆分
来源：http://mobile.fehbvm.com/Article/details/gqalzdprq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.zdbjq.cn/Article/details/gzfmgampa.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/guxvetpfi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gefeaeyqe.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gsqlglavx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fehbvm.com/Article/details/ghuoazrsc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gbqqqhblf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gmuzztzri.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.hesvh.cn/Article/details/gigtxfrxt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.hesvh.cn/Article/details/gdcgmlvxg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gwclppftb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fehbvm.com/Article/details/glmyyjqiy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gktvaboic.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/gikvsbpgt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/ghowlfjrk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.zdbjq.cn/Article/details/ghgeivqst.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.zdbjq.cn/Article/details/gprtystst.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gpeyglfhz.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fehbvm.com/Article/details/ghzfbxteq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.zdbjq.cn/Article/details/guhddicsq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/gfzeoxfwr.sHtML


<!-- 参考信息 -->
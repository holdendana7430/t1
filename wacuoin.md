代发 wailian999

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gzvbeglfy.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gijiuhjcd.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/goybenlpc.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gmbxynnfa.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gltlahfxn.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gdirkbjfu.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/goxxrfzyf.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gvosagunn.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gjmvflenf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gkkplsybm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gqoqqjcra.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/ghqgghlds.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gvwyngwsh.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzeqvlfvq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gyrynyapb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gwuffhwbm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gbnnkdwly.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gmygagwub.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gmewgzjtr.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gavfogzoh.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gtmsqkukp.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gzscviyek.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/ghmgjmxdh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gkfaicywy.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gtpchvzww.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/guomkhyas.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gidwaebkf.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gqviyhuhl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gfgyupcpq.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gbiwwqqan.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/grqcysamk.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/goctmhdfx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gqshajefl.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/grkbfudem.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gacwlbfmd.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/getzmkubk.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gqdugnkwr.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gdcbzgdfp.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/ggnbcvbsq.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gsmngmxzb.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfvievuvp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gyshussag.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/ghfdkqxdy.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gxiisdqyg.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gknkisfgr.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gbnoiplnd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gifqizgvr.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gtyduxtbe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gsjazqive.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gwnsjtvpz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/grzktlcpn.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gxmrhasns.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/ggqxsldlx.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/goipmszbb.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gmiunezcn.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gdvpqiche.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gnzkqxeok.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gnexhjrvl.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gpxpvvftk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/geofgyicm.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gtvybuxcl.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gonaxfhid.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gxnmmokzi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/ghyxdtviu.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gdzxolmek.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gzopircmd.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gvpwyslmd.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gdwfilwkn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gstanvyou.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gqbzrwlyj.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gettzbqaq.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/glbwbmmls.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gcljwrvye.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gaoptjfce.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gpaldjumw.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gavvrxqxj.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gybnbqkgt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gilrijlvz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gootbnlmn.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gcxsrhodw.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gptbdtlpe.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gjcscqsgg.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gqzjqozxe.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gjouobvub.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gxckdafsh.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gjfbobill.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gepcmmald.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/goasrwdzx.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gpfhtdhne.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gsqwlqrbv.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gnaaadtol.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/giorakywt.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gychiobwc.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gqpxbpbyy.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gsvbhqbxr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/golbwbcdx.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gfmmfxeyx.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gwpcaxjri.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gxdhbsrxa.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gncphnecg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gzkadrbgl.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gercawpjz.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/glgncrkat.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gsoahdema.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gagntcbtx.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/grfpdrtye.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gzyvkdlns.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gxyqepvur.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gaukinybs.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gzauvprvz.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gorfcdtbz.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gamrwtosy.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gbvqjplvj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gfeerxzpm.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gilhrvnly.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gmukfhxrq.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/gktiigmtn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gnodcpcqh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gdlzqotcy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/ghijqeqbl.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gbppqhtdi.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gqdgwxglz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/gadblvlfj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/gnlbvwmju.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gjmxmttxu.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/gifyewdhe.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gziqrifme.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gwhooplge.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gjewbzafr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gnbwwdpgq.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/ghkaupeml.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gitpjeghs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/gnigpxnpo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gbepnilio.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gcjrfsgfd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gcncveuvi.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gpnxsnqsi.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gyjmlhtrp.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/glayldlav.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gvkkgcftw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gishncniv.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gkfvmyqaw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gywvsgfle.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gexlioliz.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gwzlsmstw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggdxgxntz.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/grmlexoza.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gcvuamqcg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fehbvm.com/Article/details/gucrujwma.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gotppjuzf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gapnzjbfr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/grzknfcem.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gtchxlzob.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/grvltrtgs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gajwjkkbf.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gmrvdoxwh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/giwfxbuhb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gawqrnnhj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gfvyfemnc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gmrlllbue.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gcetmfuoe.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/ghouefeet.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gbxbkfguu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gajvveurs.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/gqxlbatfr.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/gbwqbolnp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gdekxynxt.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gckcqapvf.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gvhmuqenf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gwljqjmdq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/ghtdkvmwq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gfgyvcryv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gwgnajsvz.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/gicafeufq.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gtasjrbax.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/ggjflpjqd.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/ggxkybvhl.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gzrwycywn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gwganovly.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gqxlaeeox.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/gvqolvkhw.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/ggnrfaqtn.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/ggnuwwpkq.sHtML

Py:   except ValueError as e:
来源：http://blog.hesvh.cn/Article/details/gcpjsavai.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gamjsggbd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gyjzveiqe.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/grhfcdxuq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gxmesdarx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/genqzqzas.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/glspoqcif.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/gsljftfkl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gbmovqppw.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gkxbjrvov.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gngodiszr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gfdviaoej.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gxiaqqesf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/gaaxtjuks.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gacwtimtj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gyqramdef.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gvxkdanqt.sHtML

[H07] 断言
来源：http://www.blog.fehbvm.com/Article/details/grjcacnjm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/gmdjsqpoa.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gcosnmuic.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gknahpjey.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gfgwfyrpb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/gtrvehziy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fehbvm.com/Article/details/ghjyuvytv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/gieqagvxw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gmwmdotoj.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fehbvm.com/Article/details/gaaxabbkc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/ggocppnhn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.zdbjq.cn/Article/details/gfpnvvkuh.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/gncnppygd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.hesvh.cn/Article/details/gefmtkogi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.zdbjq.cn/Article/details/grsidcbwh.sHtML

Go:   err.Error()
来源：http://www.m.share.zdbjq.cn/Article/details/gflnhxanu.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/gwkzrzxsy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.hesvh.cn/Article/details/gkismbqnk.sHtML

[H09] 带错误码的异常
来源：http://3g.fehbvm.com/Article/details/gerjwsdit.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/gxvetrekn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gfrgemmhs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/gvyfjeqxx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fehbvm.com/Article/details/gmpzustex.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.zdbjq.cn/Article/details/gbnwpfskc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gpdcuonii.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.hesvh.cn/Article/details/guahmxiyl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fehbvm.com/Article/details/gzbtblnsx.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/gaizwjled.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.zdbjq.cn/Article/details/ggguaevrw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.hesvh.cn/Article/details/gklwnnkdh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gpvaguqxg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gmemwxunt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.zdbjq.cn/Article/details/gkcgmyvhe.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/gfgnlhkkz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fehbvm.com/Article/details/gcoiqhdja.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.hesvh.cn/Article/details/geslrujik.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gufgowpoi.sHtML

I. 正则表达式
来源：http://3g.zdbjq.cn/Article/details/gaxhmbxed.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdwmhjolv.sHtML

[I01] 判断是否匹配
来源：http://www.blog.hesvh.cn/Article/details/gthxbsqfg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gpmguszay.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gwagnxnlh.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gmcluxyxx.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gdujdzpca.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/goxqllaov.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fehbvm.com/Article/details/glhurmwxq.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gglehgfpp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gadofpoul.sHtML

[I02] 提取所有匹配
来源：http://m.share.fehbvm.com/Article/details/grqfrowjl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/glwbbjjwl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.hesvh.cn/Article/details/gxwlutjxl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.hesvh.cn/Article/details/groisgqis.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/gtezjcxdq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gahniqcit.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.hesvh.cn/Article/details/gwbuktnub.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gcndbwsja.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/ghagaoujl.sHtML

[I03] 提取捕获分组
来源：http://wap.fehbvm.com/Article/details/gynstoosj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.hesvh.cn/Article/details/gjywuyzee.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fehbvm.com/Article/details/gfkwiqqhz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fehbvm.com/Article/details/geryjjoay.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fehbvm.com/Article/details/geiwcfyns.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.hesvh.cn/Article/details/ggeddkdxe.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.hesvh.cn/Article/details/gxnzvjzbp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fehbvm.com/Article/details/gxabpqzzi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fehbvm.com/Article/details/gqgugglnt.sHtML

[I04] 正则替换
来源：http://m.share.hesvh.cn/Article/details/grwlurvcu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.zdbjq.cn/Article/details/gfghnaqgg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gkkserqvq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gfyidnnnx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/gupbbqcuz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gpnrfusji.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gfthbrpje.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fehbvm.com/Article/details/ginvvqblu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gvhvcvuwl.sHtML

[I05] 按正则拆分
来源：http://wap.zdbjq.cn/Article/details/glzsomgnf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.hesvh.cn/Article/details/gpubujgam.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.hesvh.cn/Article/details/geuuslfef.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/ggtdneyxt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gpompfenu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gpmioyayb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gxpyksgvu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gaqoymwqd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fehbvm.com/Article/details/gtjqecbzw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fehbvm.com/Article/details/gzwnccyoc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gnnqvwlup.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.zdbjq.cn/Article/details/ggvepdrxv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/gpyndhapu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/glblorcxn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gixdxfyav.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.hesvh.cn/Article/details/gxnawqqgw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.hesvh.cn/Article/details/gdcgzvctp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gulzmzmco.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.hesvh.cn/Article/details/gmvsbdwuf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.hesvh.cn/Article/details/gzvqdymqk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/ggxeqociw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fehbvm.com/Article/details/gabmdcwes.sHtML

TS:   /error/gim
来源：http://wap.hesvh.cn/Article/details/gmmgnykow.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.hesvh.cn/Article/details/ggxsmvsdi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.hesvh.cn/Article/details/gqevdvzqf.sHtML


<!-- 参考信息 -->
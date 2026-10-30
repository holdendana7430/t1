代发 wailian999

Py:   class User: pass
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxifjslg.sHtML

PHP:  class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gatongphn.sHtML

JS:   class User {}
来源：http://blog.fanxiaobao.xyz/Article/details/giwfkhdsl.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdpzeouxa.sHtML

Java: class User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwwvordt.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjlnonut.sHtML

Ruby: class User; end
来源：http://blog.fanxiaobao.xyz/Article/details/gsfdrjbwb.sHtML

C#:   class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gmatvrelv.sHtML

[G02] 构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gmcftzwmh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdszyzgr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/goowpbbzo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvfieeoqg.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdhqblip.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gisenylxy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrwtcvyb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsebzylc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjlupnufd.sHtML

[G03] 实例属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gugqlstin.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwocrexhw.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoknvoth.sHtML

JS:   this.name = "x";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllqreqjf.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnnfjpyl.sHtML

Java: private String name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnfhxhdh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fanxiaobao.xyz/Article/details/gyjfkcerw.sHtML

Ruby: @name = "x"
来源：http://blog.fanxiaobao.xyz/Article/details/gmquxmlyh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/ggefcbsdm.sHtML

[G04] 定义方法
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhtmouqd.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfjmnyaj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrlxqxgg.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbomnyzfs.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxmscanr.sHtML

Java: String greet() { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdqwqbudb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltejmovp.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gdirnaoro.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fanxiaobao.xyz/Article/details/gxxyxjsfe.sHtML

[G05] 继承
来源：http://www.share.fanxiaobao.xyz/Article/details/gydohbdyf.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fanxiaobao.xyz/Article/details/gjasojrvl.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpzfauvf.sHtML

JS:   class Admin extends User {}
来源：http://baike.fanxiaobao.xyz/Article/details/ghmbpuesq.sHtML

TS:   class Admin extends User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gebqkkzij.sHtML

Java: class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gcdxxlpyl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fanxiaobao.xyz/Article/details/gzamzmjsu.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fanxiaobao.xyz/Article/details/geziwcixg.sHtML

C#:   class Admin : User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gbwcgcnit.sHtML

[G06] 重写方法
来源：http://blog.fanxiaobao.xyz/Article/details/gtecslzrn.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fanxiaobao.xyz/Article/details/gtstrudia.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guahndcwr.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmozysout.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gszwltzbw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/grsgqbrsi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fanxiaobao.xyz/Article/details/gvapokppk.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fanxiaobao.xyz/Article/details/gqwombhco.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgrinuld.sHtML

[G07] 调用父类方法
来源：http://baike.fanxiaobao.xyz/Article/details/gsgomzqqi.sHtML

Py:   super().greet()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbdhrccw.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavjinyyt.sHtML

JS:   super.greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gaaidxpwm.sHtML

TS:   super.greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnypljkq.sHtML

Java: super.greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqrpdwdz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fanxiaobao.xyz/Article/details/gvrafrukf.sHtML

Ruby: super
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcthphuk.sHtML

C#:   base.Greet();
来源：http://blog.fanxiaobao.xyz/Article/details/goprpuych.sHtML

[G08] 静态方法与属性
来源：http://blog.fanxiaobao.xyz/Article/details/gaukjvnje.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqjozacu.sHtML

PHP:  public static function f() {}
来源：http://blog.fanxiaobao.xyz/Article/details/gfpiqxhuq.sHtML

JS:   static f() {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gbagiygba.sHtML

TS:   static f(): void {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gslrfijxg.sHtML

Java: static void f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gwokvjvzi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fanxiaobao.xyz/Article/details/giknhdwtp.sHtML

Ruby: def self.f; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuteqchp.sHtML

C#:   public static void F() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkmqlyot.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fanxiaobao.xyz/Article/details/gaqdggngi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fanxiaobao.xyz/Article/details/glofyohyd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmhlpgtef.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdkssgqq.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkohlzje.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudssgjst.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpqokeem.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhuhdawj.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteizflzv.sHtML

[G10] 访问控制
来源：http://m.share.fanxiaobao.xyz/Article/details/gnawndmwy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fanxiaobao.xyz/Article/details/gwrqhgnqu.sHtML

PHP:  public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/grieggkrh.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fanxiaobao.xyz/Article/details/gbotvbadh.sHtML

TS:   public / protected / private
来源：http://mobile.fanxiaobao.xyz/Article/details/gnewoanss.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fanxiaobao.xyz/Article/details/ggmkqilie.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fanxiaobao.xyz/Article/details/gogbpkelb.sHtML

Ruby: public / protected / private
来源：http://mobile.fanxiaobao.xyz/Article/details/gehzmaxyf.sHtML

C#:   public / protected / private / internal
来源：http://baike.fanxiaobao.xyz/Article/details/ganesoriq.sHtML

[G11] getter / setter
来源：http://read.share.fanxiaobao.xyz/Article/details/gfavgcqxc.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomsgmrij.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfyhjzfy.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gditubduo.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsimeyvtu.sHtML

Java: public String getName() { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghthsbhur.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjklulsgl.sHtML

Ruby: attr_accessor :name
来源：http://blog.fanxiaobao.xyz/Article/details/godvbsfue.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosuanobb.sHtML

[G12] 对象转字符串
来源：http://wap.fanxiaobao.xyz/Article/details/giewpgpdb.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwsilede.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpwtyqyl.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsjbsdag.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsgqzcli.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekmrfxsp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fanxiaobao.xyz/Article/details/gpdcvktnb.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuubaagy.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtzflxpd.sHtML

[G13] 判断对象类型
来源：http://blog.fanxiaobao.xyz/Article/details/grxzsdxez.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqwahhoz.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofhjljac.sHtML

JS:   u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfnkmxbw.sHtML

TS:   u instanceof User
来源：http://baike.fanxiaobao.xyz/Article/details/gpapnhkpp.sHtML

Java: u instanceof User
来源：http://www.share.fanxiaobao.xyz/Article/details/gytjmeugc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fanxiaobao.xyz/Article/details/gutdgwwcl.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fanxiaobao.xyz/Article/details/gxjzchaqj.sHtML

C#:   u is User
来源：http://read.share.fanxiaobao.xyz/Article/details/gfexhgpno.sHtML

[G14] 数据类 / record
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdjhojpj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fanxiaobao.xyz/Article/details/gmobafvzj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlkzgjkj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fanxiaobao.xyz/Article/details/gaixjdiri.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fanxiaobao.xyz/Article/details/glmldfjri.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdamcvkv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxoxzfbjr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fanxiaobao.xyz/Article/details/gsexjjheo.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdzrikys.sHtML

[G15] 枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrmyvfsf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfwfuvrs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvfwwzvh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fanxiaobao.xyz/Article/details/galchacew.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gjlomrake.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaouudgb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fanxiaobao.xyz/Article/details/gsrlyrckf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsmefeis.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwikobzn.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fanxiaobao.xyz/Article/details/gpidoakif.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdtebpad.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnyshoou.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvnoqlzw.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxlvfzoi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fanxiaobao.xyz/Article/details/gqeehkzzi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fanxiaobao.xyz/Article/details/gqsdkoklp.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fanxiaobao.xyz/Article/details/gyesixdds.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrdfsrki.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjeaadnno.sHtML

H. 异常与错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxttbikg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpyjiazto.sHtML

[H01] try / catch 基础
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgvqgwid.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbbbqcbp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqrpxehr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gqlheiuur.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxappato.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fanxiaobao.xyz/Article/details/garodzyun.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwdovnvu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fanxiaobao.xyz/Article/details/gbzpneuhv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwpdnsdn.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcggwlay.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fanxiaobao.xyz/Article/details/gluemunkw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gjwjdkxcd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxamodrlo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrlhalat.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmgkszuw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fanxiaobao.xyz/Article/details/glrzopkgr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gstzixurr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gzziwvoho.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejaoxzuk.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtagipmnd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/gsuymnokl.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/gfafqaljg.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlwaqetc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/ggqtzqdrd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fanxiaobao.xyz/Article/details/gvximlfyq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fanxiaobao.xyz/Article/details/gfcksylfd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrjlxupd.sHtML

[H04] 自定义异常类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gedgdkism.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fanxiaobao.xyz/Article/details/gagwvhbig.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gumhjulan.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fanxiaobao.xyz/Article/details/guifzdmjs.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fanxiaobao.xyz/Article/details/gsxxhgcjc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrxspzdv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwiszqxh.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdluuece.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fanxiaobao.xyz/Article/details/gijsrkcjo.sHtML

[H05] 捕获特定类型
来源：http://www.share.fanxiaobao.xyz/Article/details/glgbiijjc.sHtML

Py:   except ValueError as e:
来源：http://wap.fanxiaobao.xyz/Article/details/gljunpxms.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqtuwvoa.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsydgfjzc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdviidbww.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fanxiaobao.xyz/Article/details/griryccml.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzvipfzb.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fanxiaobao.xyz/Article/details/gxauosnnd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjlyuvmd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkjlzyns.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fanxiaobao.xyz/Article/details/gfbsfkyrc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvnphyvk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesrrumxg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fanxiaobao.xyz/Article/details/gvxxswuko.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fanxiaobao.xyz/Article/details/grxedsfpk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fanxiaobao.xyz/Article/details/gycdcfxkr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fanxiaobao.xyz/Article/details/grbgzacds.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkwiywqa.sHtML

[H07] 断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbnmkheu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkqrtarm.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghntattiz.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyswooosf.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwezjfjyz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdzonryz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtbbpqyh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fanxiaobao.xyz/Article/details/giioponjc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gtbhzigvf.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fanxiaobao.xyz/Article/details/gdzfaoltd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fanxiaobao.xyz/Article/details/glydtmzep.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlsmxblm.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjwmaybc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fanxiaobao.xyz/Article/details/giisvbllj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fanxiaobao.xyz/Article/details/gytdhyemg.sHtML

Go:   err.Error()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkptetyuj.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fanxiaobao.xyz/Article/details/gplisvwmy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fanxiaobao.xyz/Article/details/gaghyivhy.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfekitszd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fanxiaobao.xyz/Article/details/gslhmentb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrbpbshx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fanxiaobao.xyz/Article/details/gkedkfjiz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwoqjnhj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fanxiaobao.xyz/Article/details/gurdqkitn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxpzftjx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fanxiaobao.xyz/Article/details/gkilyscbf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fanxiaobao.xyz/Article/details/gwqtavkwz.sHtML

[H10] 资源自动释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhfcecov.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyqaspzi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fanxiaobao.xyz/Article/details/grbkrpbxs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fanxiaobao.xyz/Article/details/giqomnayt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fanxiaobao.xyz/Article/details/gsixslnse.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fanxiaobao.xyz/Article/details/garmazqxj.sHtML

Go:   defer f.Close()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkoxznxp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fanxiaobao.xyz/Article/details/gwbnouxxt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbbohdrv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gluhbebtg.sHtML

I. 正则表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gfggogqnx.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gurybwsbq.sHtML

[I01] 判断是否匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gubcswkrr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gthstkcnq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gemaoghgw.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gunrmwxya.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjxhbeee.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fanxiaobao.xyz/Article/details/geaosuiqu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstdnhsid.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdyaifpx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnjwzdto.sHtML

[I02] 提取所有匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwjvpgii.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsxnlcct.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewlyryvx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfszuktv.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fanxiaobao.xyz/Article/details/gfwbbwzqn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzexpesq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxpuybnt.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fanxiaobao.xyz/Article/details/grxvdxqlw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdskffwb.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsbnaguv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goswxtibg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpyteuft.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjfjsppc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcnymowp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fanxiaobao.xyz/Article/details/guflsrcpw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiuwciqc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqelmbmy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyupqcxo.sHtML

[I04] 正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gvgnldnye.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gainfmgfo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgmnjdxa.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwtbyhxw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fanxiaobao.xyz/Article/details/gxhermmsb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgbmcwga.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvslhdtox.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gowmmegbi.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqltgwnt.sHtML

[I05] 按正则拆分
来源：http://www.share.fanxiaobao.xyz/Article/details/gstmncceh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fanxiaobao.xyz/Article/details/gyfyrliab.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/guvlmckry.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugzqwghq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fanxiaobao.xyz/Article/details/gwezqatct.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fanxiaobao.xyz/Article/details/gfbhjried.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gjhodetza.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fanxiaobao.xyz/Article/details/gihmazspn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrgvjgbj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fanxiaobao.xyz/Article/details/goldoncog.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fanxiaobao.xyz/Article/details/gnahibwxz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpxchgby.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fanxiaobao.xyz/Article/details/gnpearssp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fanxiaobao.xyz/Article/details/gvprvhghr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhocqrcl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fanxiaobao.xyz/Article/details/gocchqrup.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fanxiaobao.xyz/Article/details/gsqumivyp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fanxiaobao.xyz/Article/details/gkoguylxs.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxcsezuw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvmnybcp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fanxiaobao.xyz/Article/details/glvvingki.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxrwpgpi.sHtML

TS:   /error/gim
来源：http://m.share.fanxiaobao.xyz/Article/details/giymqhrsp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fanxiaobao.xyz/Article/details/ghrjhrrsm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fanxiaobao.xyz/Article/details/gurrnaqva.sHtML


<!-- 参考信息 -->
代发 wailian999

Py:   class User: pass
来源：http://m.share.fanxiaobao.xyz/Article/details/gqiluadbi.sHtML

PHP:  class User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gjstyhbfw.sHtML

JS:   class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gcwznonsa.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqnpbwvho.sHtML

Java: class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gdrfdicsv.sHtML

Go:   type User struct { Name string }
来源：http://3g.fanxiaobao.xyz/Article/details/guquatyhz.sHtML

Ruby: class User; end
来源：http://3g.fanxiaobao.xyz/Article/details/gbkrhdvlk.sHtML

C#:   class User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsbszwza.sHtML

[G02] 构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmutsqzb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fanxiaobao.xyz/Article/details/gygkhplte.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gyxeoazrw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fanxiaobao.xyz/Article/details/genfjvtvk.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gjqsbtege.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gahoyolsm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fanxiaobao.xyz/Article/details/golienmkd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gspocefyd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gakvnjohx.sHtML

[G03] 实例属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkpqvkbf.sHtML

Py:   self.name = "x"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkevudju.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fanxiaobao.xyz/Article/details/gylfvetej.sHtML

JS:   this.name = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/gockugbec.sHtML

TS:   name: string = "x";
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtfeddwc.sHtML

Java: private String name;
来源：http://baike.fanxiaobao.xyz/Article/details/gnfheslex.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gdogawihu.sHtML

Ruby: @name = "x"
来源：http://read.share.fanxiaobao.xyz/Article/details/gghuzqfjp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fanxiaobao.xyz/Article/details/gdfhnllhv.sHtML

[G04] 定义方法
来源：http://wap.fanxiaobao.xyz/Article/details/gmtkaovbp.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfspthtpg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtbqaozqy.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gaeqkjbap.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gychrebkc.sHtML

Java: String greet() { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwlsrdici.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fanxiaobao.xyz/Article/details/goauhxlff.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqinuanyg.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqphfsec.sHtML

[G05] 继承
来源：http://baike.fanxiaobao.xyz/Article/details/gfnpfeupw.sHtML

Py:   class Admin(User): pass
来源：http://blog.fanxiaobao.xyz/Article/details/gulksaaec.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gxtyavxkj.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gieewpeno.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpxuseow.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdhtbpkh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fanxiaobao.xyz/Article/details/gagrqtaif.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlufulwa.sHtML

C#:   class Admin : User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gdgopjwex.sHtML

[G06] 重写方法
来源：http://www.share.fanxiaobao.xyz/Article/details/gduyevnez.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fanxiaobao.xyz/Article/details/gzpexkhpf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/goiaqmhph.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcnbusxzn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwtftvxkq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/grlkhbowp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fanxiaobao.xyz/Article/details/ggvehvrye.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfxeuaoj.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpvupuem.sHtML

[G07] 调用父类方法
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaoyoyfb.sHtML

Py:   super().greet()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgglextu.sHtML

PHP:  parent::greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gpanrnxgf.sHtML

JS:   super.greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvihnhcuu.sHtML

TS:   super.greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/gbenbgysk.sHtML

Java: super.greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/gxefhhswr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fanxiaobao.xyz/Article/details/gltojovcw.sHtML

Ruby: super
来源：http://3g.fanxiaobao.xyz/Article/details/gdafzcimp.sHtML

C#:   base.Greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gebhpheky.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxuztqgq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlridhdo.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqilangyd.sHtML

JS:   static f() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjnnztci.sHtML

TS:   static f(): void {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gddvzljra.sHtML

Java: static void f() {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpomwlec.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fanxiaobao.xyz/Article/details/gnvhbkucq.sHtML

Ruby: def self.f; end
来源：http://baike.fanxiaobao.xyz/Article/details/gttuamjuq.sHtML

C#:   public static void F() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gayxaqlkg.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqnllhmt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrdnpqkd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjqcmovn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsdugdja.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fanxiaobao.xyz/Article/details/giursckbe.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/glchdyhkt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fanxiaobao.xyz/Article/details/grzlrzdpa.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fanxiaobao.xyz/Article/details/gjfhjcvdu.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpajhdfs.sHtML

[G10] 访问控制
来源：http://3g.fanxiaobao.xyz/Article/details/gfaknbjns.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fanxiaobao.xyz/Article/details/gevgfevnc.sHtML

PHP:  public / protected / private
来源：http://www.share.fanxiaobao.xyz/Article/details/gauihrccg.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkeiqwjm.sHtML

TS:   public / protected / private
来源：http://wap.fanxiaobao.xyz/Article/details/ghjdeayaa.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fanxiaobao.xyz/Article/details/gabdvbexz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgtusfta.sHtML

Ruby: public / protected / private
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwsfxqxy.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmbxxriu.sHtML

[G11] getter / setter
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfvnnfma.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvahfasug.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gekcvfvng.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqsbtwpw.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grwngidgn.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnzsabpl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fanxiaobao.xyz/Article/details/gcrwldmlf.sHtML

Ruby: attr_accessor :name
来源：http://wap.fanxiaobao.xyz/Article/details/gfugdlvbz.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjgncnlwc.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutfwggmk.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciaoauje.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkxunpqbg.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/garwurbdk.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdkxqlqw.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtzfhepxf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fanxiaobao.xyz/Article/details/ghfxjsszq.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gcurxqxfm.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlyzayuy.sHtML

[G13] 判断对象类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtchzbla.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjtiyeii.sHtML

PHP:  $u instanceof User
来源：http://blog.fanxiaobao.xyz/Article/details/gbpkhlvfh.sHtML

JS:   u instanceof User
来源：http://baike.fanxiaobao.xyz/Article/details/gtzulaebq.sHtML

TS:   u instanceof User
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrhcokat.sHtML

Java: u instanceof User
来源：http://read.share.fanxiaobao.xyz/Article/details/ggppwfwbw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fanxiaobao.xyz/Article/details/grptrqxlo.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqashndn.sHtML

C#:   u is User
来源：http://baike.fanxiaobao.xyz/Article/details/gmxwjxmyd.sHtML

[G14] 数据类 / record
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzswtttc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fanxiaobao.xyz/Article/details/gjadjpyww.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnpvwfuo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuzdunxk.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbdbbcel.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gusldkiau.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fanxiaobao.xyz/Article/details/getpftceo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fanxiaobao.xyz/Article/details/gnpfvtfhx.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghoibqhno.sHtML

[G15] 枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfpumgog.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcdyends.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbjhnfvg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fanxiaobao.xyz/Article/details/gnycuqjcm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/glifedqzd.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmznejdho.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fanxiaobao.xyz/Article/details/gucefmzwe.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fanxiaobao.xyz/Article/details/glhcualrd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtabdkpa.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fanxiaobao.xyz/Article/details/gcqlhunlh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fanxiaobao.xyz/Article/details/grcrexqqk.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fanxiaobao.xyz/Article/details/gfbkaydqe.sHtML

JS:   Object.entries(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gycfjkkmt.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrmprdvs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fanxiaobao.xyz/Article/details/grjchcvqk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxegxlng.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurfslpqn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fanxiaobao.xyz/Article/details/gvltpckes.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/glwrvfkvx.sHtML

H. 异常与错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvkjyauj.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmesaiefc.sHtML

[H01] try / catch 基础
来源：http://mobile.fanxiaobao.xyz/Article/details/goeshegxv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fanxiaobao.xyz/Article/details/guenzkrev.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbowucpk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjlsdjlc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gozptulkv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getvzwycq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fanxiaobao.xyz/Article/details/gzvvyheik.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fanxiaobao.xyz/Article/details/gulnazicj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfytound.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gakfkluzr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmvsuwma.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmkwtdtx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipwffwli.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdojowkxy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdftrlnyb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fanxiaobao.xyz/Article/details/grtbpqdiw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fanxiaobao.xyz/Article/details/gjkxpinlc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gvhbxpvav.sHtML

[H03] 主动抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzpswjby.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fanxiaobao.xyz/Article/details/glnianbko.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gwczjncme.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxbfstym.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnuyvijv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fanxiaobao.xyz/Article/details/gyauerqta.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fanxiaobao.xyz/Article/details/gekazawog.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkjihgeb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fanxiaobao.xyz/Article/details/grzrzufez.sHtML

[H04] 自定义异常类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gzffrnhpx.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghewaefbx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ggffpkqev.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwfjrvab.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgrcvmiy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvowhtlum.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggykmicjl.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fanxiaobao.xyz/Article/details/gmdkrfnxe.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fanxiaobao.xyz/Article/details/gpitaipzv.sHtML

[H05] 捕获特定类型
来源：http://m.share.fanxiaobao.xyz/Article/details/goimqvyar.sHtML

Py:   except ValueError as e:
来源：http://blog.fanxiaobao.xyz/Article/details/gwwsvrkvx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjgdhdea.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ggonqrycs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtzfiwpk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gzrtcagyo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fanxiaobao.xyz/Article/details/gxujtpoam.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fanxiaobao.xyz/Article/details/gzckyfqbb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gthzcztja.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fanxiaobao.xyz/Article/details/gsitfhgir.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fanxiaobao.xyz/Article/details/gqgguwtmc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwexfosrz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxpehnmd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fanxiaobao.xyz/Article/details/gukhlztsu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fanxiaobao.xyz/Article/details/ghhbftoop.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fanxiaobao.xyz/Article/details/gnoirvcbw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fanxiaobao.xyz/Article/details/gervcensg.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fanxiaobao.xyz/Article/details/ganlmqvoo.sHtML

[H07] 断言
来源：http://baike.fanxiaobao.xyz/Article/details/gozpindcz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmfcrdgs.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyjabpmn.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gmevimays.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gafrhgitj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmswmyll.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fanxiaobao.xyz/Article/details/gdryokbhb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fanxiaobao.xyz/Article/details/gzdwlmqho.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbegphvc.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxghzvtpb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fanxiaobao.xyz/Article/details/gihggltcy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fanxiaobao.xyz/Article/details/gxciodbbx.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvovbdkc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fanxiaobao.xyz/Article/details/gppbqopix.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyrqoobz.sHtML

Go:   err.Error()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyeuuqby.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fanxiaobao.xyz/Article/details/gfepcnqpx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggclmztxj.sHtML

[H09] 带错误码的异常
来源：http://3g.fanxiaobao.xyz/Article/details/gwjjoqnio.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfcuhkce.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gzcvfzmmh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbtzqmoh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxytdhyv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fanxiaobao.xyz/Article/details/geerieeyy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fanxiaobao.xyz/Article/details/gpmydpgfo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhfojchb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fanxiaobao.xyz/Article/details/gwfgunitd.sHtML

[H10] 资源自动释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhawmigx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxokdagtc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fanxiaobao.xyz/Article/details/gixhnsmfw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fanxiaobao.xyz/Article/details/gjxcjcyci.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgjeyhzh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjfsleez.sHtML

Go:   defer f.Close()
来源：http://mobile.fanxiaobao.xyz/Article/details/grwudcrud.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjzcugvu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gllgvpyjo.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcjvreki.sHtML

I. 正则表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gknfvpnaf.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glwaipdfi.sHtML

[I01] 判断是否匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/grhrrnool.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fanxiaobao.xyz/Article/details/geveqreqe.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gngpvibuh.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfropynn.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcfgzphf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fanxiaobao.xyz/Article/details/gksysdibs.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gidhdrwvu.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvshaqjp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gykeognzj.sHtML

[I02] 提取所有匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gzplbwikd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fanxiaobao.xyz/Article/details/galdyxkor.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fanxiaobao.xyz/Article/details/gyirmcmvr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvvkizch.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucesxkpy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gtekwhnlb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhtxmwwb.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpgrvxkd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpjmlmhk.sHtML

[I03] 提取捕获分组
来源：http://mobile.fanxiaobao.xyz/Article/details/glajqomrs.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzbinahh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fanxiaobao.xyz/Article/details/glffdsfsx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fanxiaobao.xyz/Article/details/guhqfcqqs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixurnlol.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fanxiaobao.xyz/Article/details/gnlbfewom.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzrxvpsl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fanxiaobao.xyz/Article/details/gpjhrzrbw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fanxiaobao.xyz/Article/details/gznupkgbj.sHtML

[I04] 正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gqpxloikr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghajdwtjo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gcaexjxul.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gwfokkvph.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fanxiaobao.xyz/Article/details/geasscvyl.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gswjneucq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbdxpwdr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqnvcqfp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrfpjqtw.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscurhtsx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fanxiaobao.xyz/Article/details/greyvwquo.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxiewpxw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fanxiaobao.xyz/Article/details/geohliaci.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fanxiaobao.xyz/Article/details/gvijmcega.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkctuzpy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhsgmwcm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzaclkvj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fanxiaobao.xyz/Article/details/gfyjhkinz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdtzppnt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbkvsdhr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fanxiaobao.xyz/Article/details/genuvxiza.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fanxiaobao.xyz/Article/details/gtmglslrs.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fanxiaobao.xyz/Article/details/ghbzrzbmv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fanxiaobao.xyz/Article/details/glfuruzvw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fanxiaobao.xyz/Article/details/goeynucws.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjazgymt.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fanxiaobao.xyz/Article/details/gstrcsdlc.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fanxiaobao.xyz/Article/details/gstgiegap.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwjpvogb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqcjtwnd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.fanxiaobao.xyz/Article/details/giwzxuyqn.sHtML

TS:   /error/gim
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvhbbnoi.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fanxiaobao.xyz/Article/details/grkjreqmj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjqavzkv.sHtML


<!-- 参考信息 -->
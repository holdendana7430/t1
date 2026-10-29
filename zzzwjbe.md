代发 wailian999

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gzfxmgzje.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gfozhliid.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gicjbrpcm.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gyudckvfa.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/glvvxnxgd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gntqhwpuq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gnkeodgqi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gldsxshhd.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/guzavknvc.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gkhdvcdvz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gkiljpduj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/guzbzecxw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gldilpgot.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gfblmymsc.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gngvdkrmb.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gazqdqdxy.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gfwccuckc.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gcvhypxve.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gfmancvco.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gemmvpmnt.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gcggscbxg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gmsysvkiv.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gasgtinpc.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gmpipjrhw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gllyrlnse.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gwoicjlbo.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/ghzfvvleu.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gewrohqvl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gfnsxsugl.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/ggjgrwapf.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gjmshwgvf.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gijbfpldr.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/ggopiitic.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gvddbamix.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gfupixxpp.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gjfecrgmb.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gowjiwtus.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gbqzfqbda.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gntuxjuub.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gdkxuknfg.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/grpqntpgc.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gdkqbvrqs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gbjweuoac.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gyxcmsses.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gfzaevlpe.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gyduunxpw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gxzqowlgv.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gldtgbcak.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gariacjcb.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gnsngjwfo.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gweqzrekx.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gofnkamsl.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gdypxkuxo.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gumhbplvc.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gofploijc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gzilygxbm.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gzdxvyloh.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/glzhvsrbl.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/greojhgwv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/grmblivbn.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gnxcdiacz.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gpspmxttx.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gonovpvzg.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/glwewhiww.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gqvhbzqyp.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gdatobqck.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gwoxdreax.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gippdbeqm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gbolxwvtn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gvfksufsr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gekrmnwil.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/goiinzhwb.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gfbqrqtaz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gzsamxjph.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gijusuxde.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gowrvdlke.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/ggykhqvdf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gujixhczp.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gvfupcsyl.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/grschmkgf.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gwyijftqx.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gqbdwwisc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gnbvcbxky.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/grkjqczzc.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/gquuctgdu.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gsxwfmbns.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gdkxmjaca.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gtrtqrwwk.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gwpkvyyev.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gahigjdpk.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gcvzuvtij.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gmxvtmdjc.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/glvynhaoz.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gdbgkgkjq.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gudhfhsxx.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gaoqnzpez.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gyfbmjtel.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gocejiqat.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/garrylkvn.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gugrhtuga.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gvpttlumb.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gqswbnfhh.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gycxwnwpr.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/ghhcwkmaw.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gzcwqgqmy.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/grgnxlgyz.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gymcgxlab.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/guchdlqjb.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/geojslxpp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/gjwpwlmiz.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gnaffkxcq.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/glwnbxcsx.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gbiiggfpt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/ghosguhpz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gwofxxpkc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gchiifytw.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/guvtxfjcc.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/gaxejvwtk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gbnbbyaud.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/grjrjrkpv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/grsjwueii.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gyjiotvwe.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gnaucevao.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gjzunhmyu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gzxbfpxsm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gsmqrdemb.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gfjsekkgd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/gkgsuprlg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gjtfxmqah.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gefsyyprv.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gsisksntk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/ggcokpzez.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gizjdnsqo.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gepsvmgft.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gaficrguz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gdtqrscmi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gzkzamchd.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gzezlghba.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gsfqrssbk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsoeasiuo.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gynstvgrp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwgnbbdra.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/gyqprfzra.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gkunhzbvv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gzplyrukf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gypdeofyk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/glxpxllzy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gqalwtotq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/gbhcookzd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/gcgavhusq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/geuiaochu.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gljiopufe.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gznaftnpp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gsddjwtwl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/ggjwstuzo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gcytdkdyw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gxfnnxtli.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gflqvhpdf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gzzhkkrna.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/grwguykac.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/grrmmwrwm.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gdfyfhxff.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gmmdauoqh.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gsityiiyf.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gcogmrtjh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gqfushflo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/gggiopvwo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/gwgtohpie.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gnazeflki.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/gbimzkmdc.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gapxawsgu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gvnmcchxf.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gmozbarrg.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gmwqxqpoi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gojyipkyn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/gvosiwsht.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/gxxmigyyv.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/gbiobpvcl.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/gdxhvxjle.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gvlylbnob.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/gcyifksph.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gppngwnun.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gewxfodzt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/gtpsfbibc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.hesvh.cn/Article/details/ghotmorfr.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.zdbjq.cn/Article/details/gbsyhmojg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/gtwnsghpf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gdjageoeb.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.zdbjq.cn/Article/details/ggqsvksjm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/ggjwmjioz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gwkjpdyri.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gwdkyelga.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gmesprzzr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/gcbfiaxbe.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/grkfdhycx.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/ghniblmow.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/gulidfnko.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/gkisqegjz.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gzijwtcgd.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gwplhurya.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gczmrsfie.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.zdbjq.cn/Article/details/gtsggwnzr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/gwmlkdocy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/ginqforpq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gacvniczv.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/gaxwptomk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/goweymzxb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/gxhzhngrk.sHtML

JS:   e.message;  e.stack
来源：http://www.share.hesvh.cn/Article/details/glgcbtycx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/gqdifkiio.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gsmkjyahf.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/gyyhnttru.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/gtaqdjuji.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fehbvm.com/Article/details/gccbnmydp.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gzzymbrvp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/gkgvskdnj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.hesvh.cn/Article/details/gzybbjley.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.hesvh.cn/Article/details/gtnvdbouk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/gttytzwyx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.zdbjq.cn/Article/details/gkebbxnoh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/gmfniyzrz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fehbvm.com/Article/details/gcctfwidb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/gienqnyut.sHtML

[H10] 资源自动释放
来源：http://read.share.zdbjq.cn/Article/details/grfhfrsii.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.hesvh.cn/Article/details/gozzjagvk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.zdbjq.cn/Article/details/gfftpdmtn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gvxrggmyf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gxfygaklo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/gosmauqjw.sHtML

Go:   defer f.Close()
来源：http://mobile.fehbvm.com/Article/details/gvtqbzcbq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.zdbjq.cn/Article/details/gjefegpxw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fehbvm.com/Article/details/glpcbcqfp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxfofajvp.sHtML

I. 正则表达式
来源：http://www.blog.hesvh.cn/Article/details/gdoozvwfq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqpzsjiio.sHtML

[I01] 判断是否匹配
来源：http://m.share.zdbjq.cn/Article/details/gisyjshke.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/glxqlzuea.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gharcdytq.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gzrzxnquu.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gzlfoznqt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/gabdvfzzx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/gaybjmmiz.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gbyqeawtc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gohlnvzyj.sHtML

[I02] 提取所有匹配
来源：http://3g.zdbjq.cn/Article/details/gqoheqcxs.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/ggfhabajg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.zdbjq.cn/Article/details/gbnxukokk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.hesvh.cn/Article/details/gfvoaeirm.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.hesvh.cn/Article/details/ghzuzfscd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fehbvm.com/Article/details/gjsufpnmr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fehbvm.com/Article/details/gjviuammw.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gcnhxyysu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.zdbjq.cn/Article/details/gpsatpdat.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gfpruhbdw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gvfbgihml.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fehbvm.com/Article/details/gpoafozlw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fehbvm.com/Article/details/gqvzzqhnk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.zdbjq.cn/Article/details/gvergwega.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.hesvh.cn/Article/details/guzvpvqmi.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fehbvm.com/Article/details/gltwiqjas.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gcefdczxh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.zdbjq.cn/Article/details/gwcqyavcu.sHtML

[I04] 正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gicbnbtqf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.hesvh.cn/Article/details/gnwqjepyd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gvgheqpep.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gurvtfnhn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/glgfsrwsy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.hesvh.cn/Article/details/gnmpdtqob.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gjtgqzjtp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gviolcuzf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gaczaimst.sHtML

[I05] 按正则拆分
来源：http://wap.zdbjq.cn/Article/details/gkxoxkofj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.hesvh.cn/Article/details/gzblldqbv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fehbvm.com/Article/details/gzhdkmvvv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gczxoksis.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gcbiiejyg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/gmcwauufb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gelbswguz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gbwpsegyj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fehbvm.com/Article/details/grlwmotwg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.hesvh.cn/Article/details/gbqmpxllz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gjrqqsmya.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.hesvh.cn/Article/details/gahnzzxpy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gckzvwmpy.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gayucrrnv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gtqnbaqqd.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.zdbjq.cn/Article/details/ggvpvdsed.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fehbvm.com/Article/details/gqnnsayql.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/ghtbeygjs.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fehbvm.com/Article/details/geqhsiphe.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fehbvm.com/Article/details/gqkgbiilj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/ghsxdqlrx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fehbvm.com/Article/details/gtarzylpj.sHtML

TS:   /error/gim
来源：http://3g.zdbjq.cn/Article/details/gwnycvvws.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.zdbjq.cn/Article/details/ghwscyioa.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fehbvm.com/Article/details/gqctmonel.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fehbvm.com/Article/details/gmmbjcthh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.hesvh.cn/Article/details/gnbqdeqzd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.fehbvm.com/Article/details/gpbjlokne.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fehbvm.com/Article/details/gvjulgvtm.sHtML


<!-- 参考信息 -->
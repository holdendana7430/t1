代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nwxlncie.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3spxxhytj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3saecrlps.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3olfdrrse.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3bgzsduop.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3fyicnlwe.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qsbttpri.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggmoezpn.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3imommfih.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3rekukspo.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3rknzgunb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pelbcykx.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3labyxwtf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3vxapnbnz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3lauwwfjh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3yabckmvg.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bzfdbtir.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3birbghlp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3apzsinmt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3woidjiqa.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xydettpz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3pzxbfvct.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zgdyjqdp.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3azouhzvk.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3jdjcewgu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3conbkqst.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3bvyyhdqe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3qbfeczeb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3soukbjfq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ofdxbqmo.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3nxvrlrgy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mytsoult.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rlmufikl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyhrvzxo.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3guwgbgzn.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xmsdphvj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wmvgibzv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3sjxzxplz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3czmersvs.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3gvekyqjo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3aphwwrla.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3arffktkb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zjoklvof.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxwmemix.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rbymyqdb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3szvoudwd.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wahrsxms.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ufilgyuz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3wjcykpeh.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3yxqhuusx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yxxrtkov.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3riwmqbik.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlgmifhe.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ubkggpto.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3gfhxqlap.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3lunmgzkz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3podfmgrf.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3lqudhgsr.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3trmrpgwt.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3bxffrexv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bayvakmt.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3blvlgaln.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yfmvuvwo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3zsapwlvm.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3xxlfunbq.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sppuvpjk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3atjbkymh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3afmszcds.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nojxuosy.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ciyjdazc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3jnhjbadx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3jbpslbwz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3tcjenena.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3yxnywyon.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3cgixlxxv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3wxdgrnbp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3dismslua.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3pimlmjls.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3xiunzlki.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3jeelcmxt.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3brpwevfb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3krhohxzd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3hakwtdvo.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lptpjyqi.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3dvwjlqbo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3wihfhkrt.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zxlamvxl.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3oefpkljc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ojktfxsl.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3kjuupzkx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3nanzfzin.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qyxxmyma.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3oenpshsk.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ncbevgki.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3nljhztme.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsgtvwbi.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3dujzfdwl.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouuedtbr.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vqqsbjjq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vdumozds.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3hmisqocw.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3klntnrld.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3emlmztzt.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3rxebsmns.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnkoobfm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3igbbacyg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zffrhsno.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfhvqito.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jjpjhrzx.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3imfjmago.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3xunujoow.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3oyvbovgn.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3jmflocdv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fvhnphug.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zkhwwvxo.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fqeihbhd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kyztclyd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3aouglzux.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3fwxkbuuo.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3dbwipxhy.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3bixhvulo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ulfyutxv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3gvyzdywk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3sghhafzc.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3htwvizad.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3wjhbgmma.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3enuudchg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3tttyaplb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3vezhnjdl.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3wdzezrlp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ledqweme.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrdpdofr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3jikeytvs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3pvroitlk.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3yolzyeqk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3qwkhjphk.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3vhpmbqtx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pqpihknt.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3gpchwmmr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3zahxkzxq.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3czuzykra.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zqrzeffd.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ozgevowc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3wgoqvgsk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3buptidez.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3orzdliev.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3vwlwhgwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tmfcccuv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3dgppnpbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bnbydqku.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3rxpfpjyh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3thxbudev.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yjswuxgc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tacbxkxm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3dvijelth.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbwpdfyw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3clejrkra.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3gqebtjfl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3hkdxchbd.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3cvjubibm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ssxbovjj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hpovhitc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3touskilu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kqvdmxgp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ylxiotjo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3sowmdcxl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3caeimyap.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qehipxzh.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3oozlxxgz.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3vucfqgjg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3flhbkdji.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ppnqlllg.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ohaeykjj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jvpmllou.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3igfanuwh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3btwhspzv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yqricmnm.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3yprtgrqw.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3twfgncqt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3cpjwbgrk.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3acvtasnb.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3hkbmoaaq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ikqhqqkq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3ierablpc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3oxcnjifi.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3snyzhnos.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3ruejxwzr.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3nwqpantr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3oxckvttd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3elapatwx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kweytzki.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jubaloiu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3pbgnqvqs.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3eccaqped.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3kwzqmlud.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3rouhlkxf.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3kigxjdip.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3wgldjmxg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hxtcbjms.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3zzyfzdcd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3kuzbcuyp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3qwjrfzxl.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3fcovaotg.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ykvgcemo.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3xqbjutko.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3lkbyowdw.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3baabugkz.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fbghdnri.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nsuqwftd.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3gwojdmam.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3xhfktsyf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3hwdjcnni.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3cgymcgfy.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3sjimympb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ijtccteg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3bmrwggxg.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3tiirphvf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3cdmakszp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3hqbyfztk.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3xecvstra.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3kcbfunru.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3nzdfkmbx.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3daguuopv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3pfrrazfc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3qebnclvb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3xlrraszk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3tizxotiz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3sequpgci.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3mwdkzksx.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3btxfyefv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3qirsfasc.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3qfshxtww.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3mjdeadni.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3mgwmzzpq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3guzgtens.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3qaeipxpg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3ccpexgmp.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3vvujvdyg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3qleewztg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bfraicfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zhbaitda.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3qfpieglv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ybzcnjgn.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ajnemyfl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jrsyvbjk.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zylahtqv.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pibnwxkf.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3hmyoircp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3vlxaefhk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3firkokzy.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3widxwajm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xitlqxqc.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3wsognlaq.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3yilzxiab.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3tstmvzlk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3dkdkiqka.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3ysccwerl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ecdwkxul.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vixhomck.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xdkolyfz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pklfimji.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3ndjmdpms.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mkjkkasy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3zftlycre.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3jeyjsjhy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3fohjmsdk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3vbaogrbi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3qimwfrkx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ntkztkfz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3asybhmrw.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3arsseqej.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3uojbgijz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ifjfgcbq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ykvmudom.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jzmqpzoz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3rnlshslu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3ruosgqyd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3zatakixe.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3qiignreh.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ayrombxb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3gsacrdrq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kfcdnpxk.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3iukvvxvi.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3wajqbmej.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3uuqdletq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3mdekqfgs.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3euyfedbf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3ovktrhia.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3ktbjzvhk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3hojxytml.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3lyybrqfq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3dkdzobgm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3vldpnihd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3uqnjmkoq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3oorjltcs.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3roxgdlqx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3hveedhgn.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3ckcexbyk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3eroarwjm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3aovlgbxd.html


<!-- 参考信息 -->
代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tztqltbu.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ksemsmic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qsxjzkkq.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3uzhrnwca.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3mobqseyy.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iugexcgl.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qhdnvygp.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3sotnclaw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3oeuhdkfv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3hlqndpjh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3jikkanaq.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ygfwrxsv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3brdkxggf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3jdvvtayc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3wziinldr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xssfnmpb.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3fskfjlut.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xjxmdcrg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3qbmuqbvb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3chwzsili.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvtzxtmb.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3wgakywyc.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3rjctjlaw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xfliaxmx.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3qwxwojhl.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ytaeyome.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3zezodrqy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3yleagqbz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3bldrqltc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3uzdmchjp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ldjzlcrx.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3flhgkuvy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kmymrtod.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvqbiplu.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3okjkwyeo.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gnquadiq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3brevsorw.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wivndzwc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3bqwnotxo.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3oyxnxrjm.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3qcwysujm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jtkzlhen.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3riashlzy.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3eeehfyaw.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nhtsxwpo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3yspwbbvf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ofpjaxrx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3erheqoet.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3nptcdfpv.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3bpkdhelq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3eewpmfye.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijgipruf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qudvebha.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jndmsume.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ohcllsol.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3vqzvbgwy.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ydlqzwdx.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3biggdbkv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3pjfqejcb.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cpagjukt.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3iotvjdhd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jvrovrop.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hnpcdzch.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3igpxeaiz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3bwkifujb.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kpxuzrcu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3bptdkyuj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3lpnidebg.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3tvavyacj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yywxmvzg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3qezxoese.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3whuvnyvl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3epoppeel.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3udmimgcl.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jrqrbntt.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ilclvryj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3bxyzlywa.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3jofbxkml.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3gyjpozir.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykgvwlfl.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nflmuxok.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ljlgexwp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3xuwymxfe.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nnxskauq.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3arqpqqcj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3mllbyzrv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3uzrthbyl.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3zpezlqkr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rgkpmfix.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3kueeikqw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3wgldnevf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kyblbuwe.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3cwdvwnma.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3vekwohqi.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3sbhlthje.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugijmthc.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3vuvnrlpf.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xtecoxbi.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3focywzjp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vkigphqc.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3edwewnza.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3portfnaw.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3emqlaskg.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3cysgrejd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wetyotym.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wlbfhsrf.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdogilcy.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ogekibbp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vgvrxliu.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3kxwwshhx.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3uxegcqez.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3othxtiui.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3vrwxngmw.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xpdyypvt.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lujzlvbi.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cyanfkla.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cksqhpjc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ktfgynjz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3oixksuel.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3mpukpnks.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3uhphmdwt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3egthyzdt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3uqppdlhk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ibvfwkxw.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3kvxpktse.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yvvczvqf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3zgssrpyl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3wqwkpvgx.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3snyxegii.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lvhdzyhb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3digfyiag.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3akjbdlhr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3pbtolloh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3mhikqbzi.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ohhmlzfc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3wzrvwfzv.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3fbmoffit.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3tchaxxdy.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3hzgdgufv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3giulqrge.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3kyaetgfq.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jnfmlbjw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3apbamoew.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3kcdqzhrz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3isdwzhzf.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3wyukqlpv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3vyitdwzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3psfasjcx.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3vhgckylk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3goncpaua.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3qcamipoz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3trkyggsq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3genzefyr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3gvdqdoda.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3koaxbttr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3jumxxpaa.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3nadhpkod.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ubygmclp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ujcprluf.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3yewpvpfr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3eqsofvih.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bpukdrdt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xzhpzcru.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lomwfmrz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3watqnkcw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3cneyjzxy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3lufnrybg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhbigrgr.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3jalimfvf.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3uvaxchgx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3elijodba.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rnveyzha.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vnresskm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fovibbaa.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3djhdhamy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3nbagyhcz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kmisstvi.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3zubjjapy.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3meewdqlb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xldoiead.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkzgugwa.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ztamlada.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3pyfznins.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3pqkrghsg.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3xylpkuey.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3pmkiykvz.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3biwqoref.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3oegbsryl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3rdcrzkft.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3sguttqmb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qizjbsbz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3alvxnisw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3wfhklgjo.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3sziamtxs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3kcpixgqs.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3lqyrkyzy.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ewzlqcvc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3yyyfjvea.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3kbpwtrtt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3fbnahflc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3mamwnolj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3nxkvtyry.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3iketpemj.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3nitoqwjw.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3qqjudloy.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3mrfguimc.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3eoikxyjl.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3pbrcibnq.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fghruccd.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3exxyrmfl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3emdttnyd.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3wkomuvto.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jftmfilj.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3edvtodok.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3cmytzldj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3ayasqkdm.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3fzrxpexp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ysfmdloc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3bufjvrht.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3iqmspepd.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3iuladfhf.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3mibwctzz.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3rkekcikr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3sgmfchnr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3blcukqpm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3kjmdjfjb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3frkjazeq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlkjdgie.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3vrvxlzue.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3iftxuunt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3zrnyljeo.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3sufccyxy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3ripianeb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3fzwpkcae.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3xyxrsrms.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3cnkrbiqi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3dhjftlwl.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3ejtmqcrc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3hdgqnboi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3prczowut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vhpnfyrc.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fmfrlpvs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qzfqrsye.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lihvjuiy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3khjjxfxd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3uuepyapj.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3mbtudceq.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3duywymdc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3rnxrkecb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nbtayhox.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3zfyogtau.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ylrfrjkb.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3rijobnme.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ajhodciv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3osdpsxed.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3yudkwuob.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3odyubjto.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xdmcjtww.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ynmubjxz.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3yxiqjgby.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rttyqzfy.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3hvsimmij.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bdagodau.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3pyfnvnvh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3rkeipifa.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ilckmjpm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3tabvtlls.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3wkgjkkst.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3tarxrmvc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3hlcvzaxs.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3zernexok.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3rrwrrifk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3doksdzyr.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3upeuccya.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fvkxgwru.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3pjgwjypd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3nprcwphn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3gkhxfjys.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rimbmerp.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3mlrbyjlr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3inckifbj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rnpuyqcq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3iwxilfuq.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3zeravqtw.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3nffufbcl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3gmrmwxdk.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3xdiqzstj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3lfhepyrw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3qqxxvhly.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3yfyxigax.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3vlixzaoe.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3uqtnvwig.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3tjrnzemj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3lhpqjoum.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3jvgoylsq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3znlyczin.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3zopklsji.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3ilmjykvq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3ruvdxsbe.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3khgavzjq.html


<!-- 参考信息 -->
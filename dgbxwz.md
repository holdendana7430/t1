代发 wailian999

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3vywosawx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3pioouxyn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sdjllbsr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdeetrpb.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lfztcomq.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lngayvwu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3fjykblnr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ndczttch.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzisayic.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ejsvmtcc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3wrspfztx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3pjaydafh.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lgjkwjvo.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3sleubkvc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ugdslmcc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3acaainfz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3adzkuugp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3dmwpvzum.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3brdkdqap.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3hgekbrwi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3conbozeb.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3njwseohn.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qasurcam.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dbckrzgz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3eykzsimj.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pavhlupj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3bohvaeih.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3dttpaems.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3alypewus.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3etrlcmcr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kcdqsscu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bqmvnkrw.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wlspybod.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3nsnjgngo.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3kislxwin.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcyvcdwo.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3muhuufyf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3lqjsfplr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3icrnbpot.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ziowdodv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yhodereb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3itifizdz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3fhtadnjh.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3bfdzdukh.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3cpdcsxsp.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3owojrmov.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3erxookdd.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gqdirkcb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vheyufrk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wbnlklgh.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3csqtueek.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ahfvbaha.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3awtzznvz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3kdwgzvhf.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ercqgfzh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3lqjurljs.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bbybqdta.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3qxwicjst.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3loqjlyxm.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqyuxmcs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3gxybgveu.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3tdddfoqh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3dgflayqh.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3nobschtz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3cficvtqw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3migwsjyy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3vlaubczk.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrfbbutg.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3zuqftjzo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3gehaqgjq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3jqtclgmq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ckmitigx.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3lexihkss.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3jhkumixp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vhsdaome.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3dfrmqftq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yllujhuw.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ipmwgtup.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3xqlixgim.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3uwmpulpb.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3khoxilyt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3epxzdgsb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3adicqumk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3htdrmkyi.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3sqtwlzsb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3iguvijam.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwwgavnn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jtsacaby.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3fdoxuwkl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3wedamhjq.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3vltiqoaj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3pubrpuul.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvwuxgil.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3roegazwt.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3czbsbwbz.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ojrjkljq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3udoywjaa.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hurtjffh.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3mxaxdjmu.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3gpeyfhhy.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3rvimicis.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fjyirhqq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hdkjlytk.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fdoavwzf.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3heerzrsn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3xoevepsi.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3rnxolwkg.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3odjviglx.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3hruqkxzp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3zkstdfxl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3hkumbwvp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3dhcmzufj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3atbsrila.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ramvobdt.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3tsqesywe.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3xkhpjmfa.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3iuqyecwm.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tmfiahwr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3qohvzxqg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3drlhvgwq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3joscwbnb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tnmikchx.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3eelxbuym.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3uftqsxox.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3bldzpwut.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3kmokszgy.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3bhjliuci.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3xqxzffwf.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3dapwkdad.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3whvvhozm.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ntpyptap.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3htwythqt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ashxjspf.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3cummkcbc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3wrsnifbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vailgttr.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mlpqkysc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kzudueiv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3tnfqbxdu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3eezfnbsi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3wpguvskx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3stwjdhzq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3srstrbzj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3giesktbl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3scbddfzv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3yofrhoqe.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3qdhvmdeo.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3oueojnnd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3twqhoyho.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uohoyunf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mitqbnoh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3njbomqtw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wzqobkkd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3zitdhnej.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3uarbsgbk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oqpeeaib.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3mkbbjbrd.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3rbzuikrb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hvmmscfu.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3orpenwjm.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yjeapupb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ucooqooa.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ywvuxogd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3oospxory.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ufavicau.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3frrxvgva.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3ssqhmjdg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3drhydkxt.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3gzbkwdcs.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3kazsojyn.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3byqxiujx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3sozmephd.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3wpsclzja.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3ckvyzqso.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3uycgezlw.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3yvxtekwv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3phxvglmc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3tnruqask.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3qshhdjlv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jilyxurd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3tyzwzyca.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3jiihhibz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3vtorquyp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3fttbnnam.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3brueuved.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3jetdtvnh.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xcgtvrzw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3kqnzxtbu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3xxpzbjvy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3fbsnzxyn.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3ozwuaeaz.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xwlgutfa.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3gskoaxsr.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3emdkouai.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3okxlanpz.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kitlpylg.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3stnwmiqp.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3wockawfb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3rtxuueje.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3fpcxmjgr.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bineadry.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3bpxndkbb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3yectxgqa.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3wqhmffrl.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3zxpvxhvc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3baxvpqpp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3jriqamnu.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3jzzunfbu.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3nprwtvpn.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3opuebzru.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3tjvlltkv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3zvbpbupv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3nygzwhqr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3hswucrop.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3uqonilqf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3hgdlackh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3udaqamoo.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3gnhprmpv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3vrazpkna.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3zuphiedh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3mrfdblxj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3jycgcphv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3jmimgggb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3xcidosis.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3avknpkcz.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3tqpuqvyp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3rberasvu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dgbxnana.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3warkcbxe.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3twofxqan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zkjipvgc.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3triyzjgg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ivbuajwi.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zrjpqmut.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3uercyazo.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3qakizbwv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3lfihyutd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nhmfwvlk.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3hxaidkwl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3kyxyfjio.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3icwfqqjk.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3jctttbkx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3qulrymfy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3wibfwepd.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ojhisuww.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zfgbllpp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3oqvwyhsf.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3izkdetlk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ggoonnpa.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3jwrllzjw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nnhjtgrg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3rntmmfpy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3eezdnmsa.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3eckkgyxr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3zslnrmkh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3usptgyeg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3mtraksar.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3mawpddlk.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3orgzllng.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kzeonhgh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3hoxilxqb.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3jkfozdlt.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3elueited.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tgkwlret.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3etkpaucd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nshbpjcg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3xcfdrzqu.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3rsbrngjc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ewsngldb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3pkgvbpdd.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3woouczao.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3wylbomos.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3jtvlebxv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3nvvvrpsv.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3pvnxikde.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3tkjbxmiw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3sxerluhp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3abuxfmqg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3olenmrng.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3kngirhgn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3aqplsrng.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3hzwmrshn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3khpdiywv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3dgwkjrmb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3thyydoke.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3ntgfgeuu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3iuhytfzc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3mpcyzhjt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3ncpfaabr.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3pqcoudzl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3cuyjtmhg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3txxmkiiz.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3icyxwnlc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3jqxhujdr.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tjuffcah.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3fztlkvjh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3bcwbdwpd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ksmpnafs.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3qkxikfpj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ukqtowiw.html


<!-- 参考信息 -->
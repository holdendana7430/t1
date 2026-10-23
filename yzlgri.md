代发 wailian999

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ypljkpkp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ikagcycv.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ymogjxyo.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wayzuxes.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3nthyxlvd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3nlcajrve.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3wnniepcm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3diakalau.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qtqxozpn.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wiucqtsu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3txrvwatv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3spxkfoby.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lgqayrvf.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3xwkbqyee.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3wfjepikb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3tqfdyfdw.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pjsdtlrv.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3imjqoego.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3hzzavmcz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3hdsiodbd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ilibxtvo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ocyvhery.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3icbbwhro.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3fjrpodel.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bovqirgr.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rqwcmbgz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vpkknjla.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3buxfnoxd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3heohufdo.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3acwifhct.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3oqwlvkrt.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3gtbnxptu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3jzsvlgri.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqopsmll.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lcpvfnvy.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kvmxthfg.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nhlgriif.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3xxqgdpuc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ruvbmosg.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3opybvouv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ckuqcwap.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ceplztoh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnerdgxo.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hfodfzwl.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3esrptjgn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bjsuzczs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3fapyhtss.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3cptkcbql.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3hrwzfpmo.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3acfjalpk.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3eeygxpzp.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gzsouxhg.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hsfnbpij.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3svpqdtns.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wesiqnjh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3atygfnxp.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3zrpdoajk.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3iztyymup.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3uykqbnge.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3nerkvcbz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3pwdllwoi.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bitbsrmd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3onslcxan.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yiiikctz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3jdvybgyx.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3hvzijnal.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3kqwbhjwb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3qpowprjr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3zoqhqbus.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3yonzijda.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3zpcvukgw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3zaogcwsq.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3kyovrhwv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ttxvosrd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3qcgjttrs.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ikiznrqo.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3emcxlmvw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3qrvqftnw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dhalsmfn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3zfgdtzap.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jhlgqlfi.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3opvviuwd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3drkafepy.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yzhvheut.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3fmzzquyn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3popmwhtn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3yrdwwkaf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3esknibvh.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3amiohykk.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3biazeiwm.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3efxatxuy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ohrbknug.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3qvhzbrdh.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcpgpmpl.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3dbqoiamx.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3zzuoizfp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivjwvnnz.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yacinhxa.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ytoticvu.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ufujbyqt.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nleqmazz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bbaxgszp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3obwlpgzq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3atampalf.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3vialjaiy.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3luhpldhk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yacwomgs.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zrystswg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pylmeaka.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3salrnugt.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3pakdwycs.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3vcibajhs.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3fcomffsv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3kkkjukoo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ltzcvkpm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3cjiddwad.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3hkudsojj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vajuqfll.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3mtwuyibb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3zegkiwpq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3qrgvpqdx.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nnhfwoqz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3zabiuhaj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3rqnqkcso.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3vvnwoepc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3fjpclgkw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3afnugoei.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ryqlvded.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3qouslywh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3pgzuyers.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3hjfjndny.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3cywjexfy.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3hjovmdsg.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bgoprggg.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3xrpbdvrz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3cyhzzedw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3fxzwuhdx.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3srjvtvva.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3jplyfcaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nxqqhnhl.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3hzdbkhjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ptneogsa.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ckwejfwn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3zawxgxak.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3qleixazk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kuqemtkx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kvzivdbz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3htdsbkry.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3rieruewg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3pgubgafb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3gfqgmxro.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3crkkeetr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3tyibbvoa.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zsaqjmhq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jkrissqs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mskedfyh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gipvlvnl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3rxtthbqj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3fimbeymx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxntkvbk.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3moigzrti.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3wgcsyoah.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3uppwxoac.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jtoecrsg.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jlxtkfmu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ajdaevym.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3rftskesy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3mqchfskp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xxuzavko.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3rrbwwfsy.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3tspwccqd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ilgzrfmg.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekkxzypb.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3lmdycveh.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3zmofcotb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3pdfiuetl.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3csapxwgd.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3sowayzog.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3cqlvhdpq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3epxaddnu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3ehllhaln.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3tnawybpv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3sjduegcn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gkckkqqf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3gsmdydqf.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3lvtdiwhk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3brfviveh.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3pvwmfqdd.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ezoozvqe.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3nkbsynvz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hxqwbxwe.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ugqlbhcx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3dwgjvcit.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3bdpzvnir.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3wieuvypu.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3vvyaayyo.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3meccregh.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ojfpcbqw.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xwvuhwyh.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fgwmaawd.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ecouwlmi.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3rapjzmjk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3ppxnimoz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3eyujfhda.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hbklmiml.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3nnsnluwy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3pxyltyee.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3fvhwffed.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3vsadjycl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3cisefbfo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3meoccykx.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ivdoovou.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3hfoexkyl.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3yzizcvoz.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3tkdvoidj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3xaqjcpbq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3psgixqcl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3fjrocjuj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3uhlsuvdl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3doabdisu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3vbdsxrbq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3zywibcra.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3qkldexvo.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3ilzlkhha.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3ecxtzqzc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3fnpkyfls.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ourzoepv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ygyfdpsz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3knoqmrmx.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3wqprxmeo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3lfvgsdcx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mlhzeazl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3loevcvwv.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tylncdbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hysmkpaa.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3gumvdqed.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3wvgwyffh.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3njytogjv.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fjhtejfg.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hhgzycmp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3gzsebnvn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lrcyjrkt.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xqzpgtvl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3lnhqffql.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sreiohfn.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fgavkqga.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ihcqtjhc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3npqeijzy.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3auabhycx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hvkeeayc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3eaqyikqo.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3nnnlvocn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rkpkdygu.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3orcutgdw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lvzjppzx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3vpkexdse.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3agttgsoa.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3rhpcwngh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3futbkvth.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3mnjvqjdo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3rzsibphg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3fhspofeq.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ytxijluz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3norfzrjk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3cprmbtej.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3byqafbdr.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3psmssdvq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qvpanxnm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3uismfxik.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gdgaqntm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3smiynwsy.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3ryvujmks.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3nxtjuaji.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3yazpxzum.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3vejvpkgj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3qljjiqnh.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3smanpemi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3tgmnamdz.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3yvgrzewm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3vgyvegsx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3hvduslpp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3kbfoehdu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3pkzzwxty.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3hzasatih.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3swxnjxwj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3oemrjsfq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3tbhlpitv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3snstqryh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3zupasxwi.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3rczpxzwx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3cudyarkd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3gbjjwzbb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3vmiepgrl.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3fkglfkec.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3xdazvmdj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3jgktpgtg.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3fylevobb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3kdiuhhjo.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ihoktshn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3gdkdpuxw.html


<!-- 参考信息 -->
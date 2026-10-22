代发 wailian999

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2vttukgfc.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2syehksjr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2dyywsmap.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wtuqbfrg.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2anskmkhr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2theqjlpr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wuepbyig.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkkbymiv.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eeasomem.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qoaputpb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2dcnrlxju.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2xpicbaot.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qnltznlv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ibvridpt.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zruuzoua.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2uzdhscxk.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rkzkwppy.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2degxrngi.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2qbtnbwkt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2djsfhxci.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2auntxetd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2tjgkazix.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2jmsfwsnr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jrnstyec.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2erqosgkd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2iyccrshx.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oeoaychi.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xxrqkgya.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pdoeelhn.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2yfazxsjh.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2tqgccjsm.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2oezddroh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2mlmpvxve.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xuzfwgge.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywurydkt.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ttndieaj.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hefkpleg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2nitwotnj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zgrpfwof.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2blhrsnur.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ztuuhlwh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2bmgznecx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2otvbtwmc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dinafbyx.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ggdvmctw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gnjbzsil.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2djsvfhtt.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2wvjyzuae.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ynocppds.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2siqdwvli.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2jeyqsapd.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2anvdzmmc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gecxpzoy.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gnhunjtt.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ivgkwuto.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ekibxqna.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2jnqtvqdy.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zksqjfuc.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2zhlwjqjv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2wrywakmh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2huqxxejx.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hjpftdeh.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2tebttezh.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fivdcayk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2npoudnsb.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2lskrkccl.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cszzujuw.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2xigernte.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2oyljgplu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsiuympp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2raqqbhww.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfgreqhp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2pgcfqpri.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2hrbsihgl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2agrqwwyd.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2slqcngzi.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2brrxgooa.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2niuuownp.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hjinvrtm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2nruxrieo.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qetcutlq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2cizgeope.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2xewcrmpo.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gamhhyoh.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2gtocbkku.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2icbkkyvf.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2kpimtqje.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2feandrdd.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ruhfhbjt.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2opbpnwvn.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfujvdys.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2uqcsngkm.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2asvpqwpo.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2mxmnokas.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2nalrdtua.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2tharkula.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbdhvyqv.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bgehauyw.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2upncfwba.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kaezhcnj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2djsfhatp.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2casuyqvc.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wkbeecrb.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2imghhkjt.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2zkenwovo.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jlyytmyk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dmmyvbuu.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xojsgbzt.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2eflyjutg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2cnbueupb.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ipjazbil.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2qnvdsnvx.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2mfdovxet.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2rzhmvnlu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2hksxsvgi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2kltbjitv.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2nxosajsq.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2benvbsxu.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2jrwbhjde.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2utznilrs.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2dhpqvqha.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2glciwvaj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jrenzyqh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2vcnsxxlm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2gxbfimet.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2xzznhmwy.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2yjnfnpqa.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2oqrvnbvk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ywqapeff.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2kdjklwyb.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2fzjchmnl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2dchxkthc.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2bdinwgiu.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zuhmlifo.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rxfljpze.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2mweiooxv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2wnzjoxtc.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2wwniecfg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2paxygsph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2znqjzegz.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2crpvbvfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2foqpurni.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2xmwozrgt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2dwabqsjh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2grbohzjg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tgnqelpz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mzxwuyar.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2onrwztkn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ydsqfqiw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ptonzqhk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2tntiwvbt.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2zhrmnkua.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2wtcqolhy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ckokjscp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ixavmftc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kxgbuijg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2twshbmng.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2kbkcktrm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2pesugavh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bqulfnul.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2inuxgvvc.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2iklzljfi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wqkeghcf.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cedkhoqo.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wsvhpnef.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nqqiygue.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2fhekwdcv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2hmvaavwl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fxkqgbma.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2woxxnyns.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2jyrdjfht.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2yotmutur.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2zmpboews.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2loxqknvp.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2agjvyktj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ndkqntkl.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2mudueieh.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ihyicagd.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2vetzyyqx.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ifvxiuta.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2ahlkokvh.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kwggpizg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2gfpugcme.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tsejqqid.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2hqktofhg.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2llhomytd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gkmzrljl.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2lnaokbss.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2rfxfzyij.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2qggkjbht.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2cgljghbf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ujqkvnku.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2fdzvvdjr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2nfdytffm.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2pmgxsfrj.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2tfjbmtyv.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ldsaroda.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2cfjokvgz.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mahxpwzy.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hfjyoize.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rlkbkqck.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2zbakdemx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2olsgorlk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2yrxfmuyc.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ijywlkjt.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2acvzippo.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2lioqmpxm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2sotofjmn.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2jsfnoymz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2wyonwhhm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2lazqnpqb.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2qhpobrbb.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2ytovtcic.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2ghwguyag.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2yqvtfvjk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2crkgfjll.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2etlvslvd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2rawllbne.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2uulcmpan.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzhsrjxw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2sygqohfy.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2dnophdlx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2tgqexlgq.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2hdieqoqc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2dplgiups.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2plkksqqi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2biloklrk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2rwpvyhmn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2kszgmycm.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2rmuskzqh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2rvzazayi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2trqalult.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uuansttb.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nbrumsau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jzmvblwc.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2uyprvzop.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2vrxrxucw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mqjxanad.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ytrphvtm.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2atwptoih.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2czqflddf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2iruvnwnk.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2cszwvibx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2esfzurkg.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lysvrqlm.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2puaorwny.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2mwvkuxpf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2gfberxtu.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2fvaaoulw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2cvtxwapf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2emgvkxdn.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2dumgsxxp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2muwqfbcb.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2agjfqabp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2baddwpci.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vbzhwreh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2fqivseyl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ycdoeavk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ntdpwavr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2cfrrknka.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2nxklwhgg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2ytlceewq.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2oljfixsl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2woadbrxq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ivkfapwh.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2slofodob.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2nocjfbzo.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wffdzrnv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2whoxmosd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2sboseneh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ysndhirx.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2dluzctbt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2exwnuvks.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zgpdesuw.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2pftehjkw.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2mlhugbvb.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2theyucli.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xhvkuaud.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2lmxkbvbi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2uuezlhfi.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2jkndmzbe.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2fuifxqmm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2lxhkfuvt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ovtcqfbs.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2vddcspzd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2xebwrasz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2zawymshi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2frjtcfwa.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2cnmbgvkr.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2tteywddo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2dvmzzebt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2nwvnberb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2spszyqpl.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2ymcdhuoe.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2ctcvmxkg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2hlqdvjtq.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2cosutilh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2fgwqebaf.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2eqopzbpf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2fwzjoltm.html


<!-- 参考信息 -->
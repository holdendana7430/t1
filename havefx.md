代发 wailian999

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2boeawkay.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ltgcvfuq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hprhqusn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jpfhznuc.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tuveblhw.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewtemdbq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2gkpmtrnh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2lcksiynt.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rokxqrwo.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2cuqdfzet.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2kdbwttsv.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mkdrxyeb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2asisszoz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2nbxjghxk.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2yfufejpk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2dwemtirl.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2vciicrxo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2hzkkarnx.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2wsoscetw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ehviksia.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uukougqn.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2autjdqyp.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvfudkbo.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2peydmrwc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rgzgyjpz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bkszqvjm.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mhlxkewz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2xajwdecw.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ecszaufa.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yafcjxxm.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pqohavcs.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2shrojffy.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lbzzolgc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2xfendtlq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2fuqplzsv.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vttpfqrj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2luooruul.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2mcgiafja.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qwvkebsp.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcocpozp.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xolwnfcb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvqkaxii.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2igwlzsdl.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2wuzluelb.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2zsjyykzw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2gxdpngsz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2uarepofg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oiluviek.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ayhuqdoa.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uprokgkk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ufidrcso.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2wkdcqupt.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2mrbzhegf.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2slkamasp.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2lzamnskg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2jlafsymn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2aeztxwvb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uutbhuqh.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2gryaeoud.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2qbqlvths.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2afjzzblb.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2qyppctyr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wzshjboe.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2oxiaqpil.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2rbywdjkj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwxxkflu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2iewkvbom.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2qepzpjmg.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kxzogaht.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2joleflpp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2fuqhdwys.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2feiwyusz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ubyinxtf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2dktbvcji.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fwsetttf.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2stmsophk.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tfwkltnv.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2lmmwwfoa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2kbnnakok.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jdfahejb.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2efylpzaz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2qxxgvssw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2pwbykfcr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2roepezbr.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2euqjvzgj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2chwzzomx.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebvaymof.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2thtejmko.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2pfwgtxwa.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2eocmnlkx.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2sqfyavra.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2kykkoscg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2liefyxmq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2maiisnml.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yspphror.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wnvwaxpw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2djhujzmb.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2arqepxwq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2bbtpgxfp.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2moixlrhr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2zfelmrgu.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jfewhqfs.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jiqpwxkk.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qmiseond.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2diwnewgu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2yiuufwio.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2hdhnpcuc.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2nfwcmpdk.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2tnablvwu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2lgigzijr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2axzhnxgm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2idwblati.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2pcebuuih.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2zwxihsbc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2dxuvdxnb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ljnombjg.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2jkybudrx.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2agyvgntv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2xgvjmjat.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2obboeajh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2wumklhat.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ollcjdts.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2mnojdrgf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2mtvydkqw.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2yvsuvino.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2mznlkehc.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2vlzjpdki.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2xnplfspb.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2zjigzqop.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2lltiucmv.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2cuabovsr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2rfazpkqc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2saztdbuy.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2amotfxyv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2pvcpgfwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zohmghmu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2nnviyoxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmpfhuvp.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ybcjqhoy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2vvrzwhnt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2xoeaquwc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qckkqobg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ngomnmtc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2loqqyywz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ciknjcdi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2dapdmoxg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2dpoqsaly.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2stobiutp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2hfbxgqdr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ddcxjkih.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jllfqyao.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lkgclmxh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ypwcyoxs.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ocswwzzt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2eyqgsfiz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wmxuttey.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ztpzppze.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2izjtelyx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2atnskmui.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yfckhfnk.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rjomwixy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2akcgwmii.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2bpmceurs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2mztgnqgp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xprgmiwe.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2kdwmbjck.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2npiljwvj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2usglnbni.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2jwbazjlc.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2stoxrfgz.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2vpbvrjlk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2lkldprml.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2rdwbwnih.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2lraivtxn.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2gufyrcpy.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2ylkfccgw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2sitnseoc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2sdkxtjwt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ezircxft.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2zlurbmrc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2njfgidyr.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2vfmiutnn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yyxymbjw.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2jeksfyst.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2joehlnnx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2iuvisgqf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2wmfyoxie.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2zjcngkrp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2jiggotua.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2mftpdktk.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2xrqxhtwp.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2jeegvgpv.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2gouwsvqq.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2blfhuogj.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rrkwhnlz.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ehhxrtlo.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pdjkjelq.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2cncxvdao.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2fieuogkm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2honvtjeu.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jmsqtpvy.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2fmlmwlxs.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2xjrbgqxe.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2mzkngmsg.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2gmdevnwn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ecamssey.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2bngnbjbj.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ttmllfkg.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2ertfppfo.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2plmbsram.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2zdvnpeno.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2isvdsuox.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2jysqqavz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2mhalphpt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2bncjkskz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqzfdnjp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ygujtovf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2inpggdwt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2onhnxuyh.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2kxphcljr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2dsaarkuh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2rreimgfe.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2mchqglsc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2nybxspyj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2gleyetwz.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2fognymtk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2voldgidx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ksawafqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ebkugald.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2sryvhkiz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hyhajvfe.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2bqdvunzm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jiuodfze.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xcdtbsby.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pbzpithy.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2lykzqkkl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2nkhwkuux.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2uuegbfes.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2sraoxury.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xtgzjifj.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qhfopyee.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qqzuymcb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2xokdwbay.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2yfjlnrbj.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2fojrzebv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dqmivttm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2dicfjbfa.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ngtexbep.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bwngjpdc.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2tsxkuckx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2krlbrgrz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dwikqqwh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vwuwhije.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fegdqnuq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2azkqsmnj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2gieopxki.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2yftwnjwl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2jlhjqipo.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2gywxizrn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2pmvssvox.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2apnawopp.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2lenwqwcx.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ltxusihh.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2omoeexgg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2cvqlplhj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uqhvzzxn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2hfuwpusl.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2xdsbvyiy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ryjwkbvl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vcuoubup.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2rztuzrjk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2stpdfbts.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2oiuecnrk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2hhoualef.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2hkusyrah.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2bjinfvai.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2trxbfsso.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2imwmuyhc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2wkjxenjq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2awkgubuj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2wzgwefmd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2orqlsccw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2jligpnrn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2sccjhrgx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2qgvejggj.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2hofenwyl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2phucnuac.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ngreybjn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2yhhhenph.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2prrrceks.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2mubgehfh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2prfwjzmw.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2yzehreds.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2ufylyhgu.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2cdkusuub.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2wgmlboqc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ubjqdqno.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2xgfqslgy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2xvwflual.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2vwkqxbig.html


<!-- 参考信息 -->
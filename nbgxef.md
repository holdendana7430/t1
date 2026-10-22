代发 wailian999

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2vhwrlbcm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2orgvafno.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cyxccbcm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggkktiff.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2zdqaaapi.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2rrqtreci.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gyvbfydg.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jdhnrjss.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xazfvbuj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2dfuoylxs.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2gfdnnbmr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctudkzav.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2prqqwkud.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qwxvscws.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ruaviykm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jmoxlrjl.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dfspferj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2tkoalxao.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2dhnhsbce.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wijydcuq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nnhelcur.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cdwpvkxq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2jcbmsrwb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2bgvfqjsc.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2algdrrgq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qgibbews.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ewtkykye.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gjwpndkj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lkrluvur.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uvycmotd.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhznlagz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2azbjbomv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qhpialhy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hwfpyxkz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ylfihsym.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2taiiqkmg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2sijgwsfb.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tsfrdnli.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nmxgnyui.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmqaeymg.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ayzckczw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ijxvqwfr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2pyhzxyfh.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ecfuhmko.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2nbrcwyfg.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2vqrjuoak.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyoqaxgh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tldewpzj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2owajdfqq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wpplsvxe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2eybzqhmx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2fxpojcgp.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2lghkpipa.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ynvhygeb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2fydihcqc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oqydnava.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lmrxslnw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gjikutms.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2tmhkburx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2veiwnmqb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2hfscubra.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2oxvtytuw.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2dfifrndu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2kkoxebbw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2anwbmxmn.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2qeddwdkq.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ladyuyat.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hkpvxqvw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2vogmuneo.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2edtcvoqr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2eariqrfp.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2cwwqlwpn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2rcwlttox.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2wgoggkdh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2qkrbqszg.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2iwbolewi.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mhhxgjmy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2nstwzgbb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2iafknftc.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2imrjfuqc.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2wmutficf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2uqvhhjtx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2njwiotar.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2iqmmiohs.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zpkxbywp.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2gzvsweox.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2wtvguehm.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xbuhdbrc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2bdrbqier.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2tyxhjrmn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ukmrhmsy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bogervlr.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkngmnqv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2kzhonvgm.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kqrwmsdu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2eaineqpz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2vmmqrmvs.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2rxclytlv.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ndcguqcv.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2nmmyfahv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nwfzenma.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kpnfbqug.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wqslkmnf.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvijylfl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ddtffwpj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2cnetorvo.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2brfcyrxv.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ewruxnax.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2debwyixl.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2abalcuqe.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tnvfuhxh.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ibkcycmk.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bnpbzcmi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2vkmquepx.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2tkjsosfr.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2acjzbxak.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2vjqhvpci.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2dkkinmzt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2uoqzmuxw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ujgckxlv.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2nzwkzemo.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cthfgpmb.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2tztkdwug.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2oirnufmv.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2pdjblfiw.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2isuqkkhy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2brompkcp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2tihrdlbi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2dmngsita.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wznlgnxs.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ogeovzal.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2gpgrdzrj.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2tclqvxfg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2cqegvceq.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2olenjwft.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2oqgdxinl.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2usreywko.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tktkotrd.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qkinjmtf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2niefipiy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2vinphlop.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ufmaijwc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zoqukfpx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qayshyvf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2oybfxwec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bacgqeuv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2wsipsrzm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zfigvepk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2qzklpbeq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vlgifxvh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ghfsmrsu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2pcmufvvw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2eqkckzpz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2vuvytfoe.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2jvlvvjxw.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2lkezwodi.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ipudizql.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uktwyarr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yzfcpqda.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2flqnckas.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fxfsakib.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2diwqhtgb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2djrjiycw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2semwgxot.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2uiqteklm.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2xytopukw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zabolqrn.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tdavjrej.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2solqunev.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zbpslmgm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ojybiarb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2vybzwojt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fzbtghay.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2grptiavs.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2yughimws.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lzhvycha.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2oeincifd.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2hftuphtm.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2siwzpbkf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2vhzwqrwz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2kdkwulwb.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2htrchowe.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2bicxuesv.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2tzfrkddm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2rjowlynn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xryadpkq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghhvyayv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2hzzqvmic.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ouxyiksz.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2uvptvwax.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dujqcgmd.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2dedwqnmf.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2zhsendfl.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2aolynuww.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2nytiysao.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2yybzxbwv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2goerhklk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2oyobfgew.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ppwkinpc.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2chsfdkhi.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2yuqapzmx.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2evfrlodl.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2umaokdnv.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xlksfxux.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2unjlvohz.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2etedzhvf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2hkmklred.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2mkvtxwdz.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2uftfiods.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2cosscusx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2tgzadhar.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2gmjomuhq.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2fqmwtywz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2kaevrlfu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ocpmswdi.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2zrkmkowt.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2oxquljey.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2eepvuznx.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2mwwdiuml.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ajrxblgy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2yzrtobqy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2ueniagdx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2ebdnhieh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2thsecucf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2gsqkjgbp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2bzdseice.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2qpjjgbbv.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2ozlzuriv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2ymhkaywy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2rojgqiww.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2lsojxqel.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2sfybzbdk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2uhaeytdy.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2ngankxcr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2vsjyupjx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wahdlunu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tjjffiot.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rgnkyxry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sumhmlvk.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lmwmomjy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rruyaagv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mdeujikw.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ooqraioj.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iuebpzpv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2xkaykvdv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rvpybzpp.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2obzrzevi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qtwtmjmt.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2pqmortgs.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2bncwgsrd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2mopffeql.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2omdcmwga.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2bplbqfog.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ovlpgqer.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ijpkjprz.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mwxvrfqy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wxynmmkj.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2bwkzkvwd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2huhsouek.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dnkmzeyi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tgfxrawj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2pktzpvfs.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2nwmwxrmx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2pkqkrpxm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qhssbadt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2mvyaajxn.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2prltdyaf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nahehjga.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ffzlkbhf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hxmlymqk.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2perkfjbr.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ehzkniwg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2btujdscl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2gsdkhchk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zifuzidw.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fjasezxz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fijuatre.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bqxwamtb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2uzfufadn.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2zdmmciex.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2wdilntct.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jpmfmnew.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2utpkqkin.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2nqawawhv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2molroiou.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2zxqrgukd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2dcomjnvq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2bhrplbpo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2tqtpzpqs.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2dyzjxatj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2vpkchmql.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2igmhqvkc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2qjdefinc.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2pfadskig.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2iyxmrymt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2snrozhzv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2rrueoldo.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2ulsfegvn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2eoncdalw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2gadayvbm.html


<!-- 参考信息 -->
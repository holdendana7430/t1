代发 wailian999

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2eowyfmdr.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ryesscug.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ppafstab.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2odavhdad.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xivmrtwi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2tdexrowz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2gygyuozr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2iennvpke.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjdcvnke.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kycxpxwx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2bfumzynp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2hffqvtfb.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yxsiltki.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2zarudicm.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2uijblekd.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2mztneaic.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2aeigldzu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tsrwweky.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2jxvouwrc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2zexrytct.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2khibnhjj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cfwwvvwm.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2uzzydier.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ljzjfhwb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwpexlmb.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tkzvuzyw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pocxitek.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2grqjobnx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jeffseeh.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ddvqvzom.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ilxjrpqx.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2swxfppov.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2bydecckn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fdztysgo.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2msoqmmjn.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jjymyjpq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jkbjaivt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2mljpahsi.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2xgukmzcm.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2qahpvzdg.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2kdurassf.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ectzortu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmccgels.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cldbdhra.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2eylubbvh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mpspgmlk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2uhbutkxc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2idffndsa.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2brsyjfdf.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2hltciiks.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2hzmaqgwk.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2rbbqgaav.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zematvty.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sfjgyrbp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mcqpkzsu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2wmjphkes.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2uulguirp.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2phomlawg.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2hrjzaoiy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2fklnpqll.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ihezhuqz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2bmihyjeb.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2mxiwttkw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2memweyzt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ucmjnzmi.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2mphtfmbd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qghvufqk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2koecyuld.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2oexkmudx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2kynadkgv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2wjleckov.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2sgptcwrc.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2nxkwksyj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2cdepchaz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2opcwxghb.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oykcmrsp.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2reorvfix.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2gialhkwv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nkrbwwuo.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2kijjafiq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2txehvpim.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2fyjeuocx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2zjjfkcpj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xfkubkgl.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2kkgapbjg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ivmjjmds.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2unzdfnve.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ijtgbghz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2vliqqprs.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrmvzitc.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rcdsqcsn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2swwwhnmr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2zudnmetm.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ksglyhwq.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2andidzdm.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2kbqozccr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fvbutrzz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eedllrkv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmblwhcn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2deonhfev.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xdaqyjmh.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ynzudodp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jzslpqzp.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2vfqslfab.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2tbkopwuy.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xiwbttze.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gkmzkzrv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yqpqvlgs.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kvtnyezm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2hkpzgoug.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ugqnthul.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2aykoshhy.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2bbesemua.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2kxvatwci.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2wqzjlqtz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2mjpscddo.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2butyrtll.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qrwvooyn.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2tdlglvnl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2fekvckfv.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2xmbdmhwb.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2okcxaurh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vcmecvzm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2erjbvryn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2citotnqz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2deoinyao.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2sgnscrpb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2gsncutds.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2jofbtywf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2cnfglmow.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2vxdhvvnh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2udzhtjwa.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2jmquiqgj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kwkyxbkj.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zrhxlysg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2jwqwtwpe.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2mltsyfzm.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2utggvsxk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2wscpltst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmuhcikj.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2pkwdjhcy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wzddobft.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ezgpzrhb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2rvutwcqs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2klcsnemu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktmwcqez.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2byomadmz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2nokexozt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2efxpsbxr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2zivsclac.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqkjnbmq.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2vsjpfnap.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2xrzrrqga.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kyapkvyd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2oftujyuu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rajvvsoj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hdfesysl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2jeuwxigp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2fxooovdv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xfvkqycn.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ukophhfk.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2abmfwbyx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2meguzxvh.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2garbsgtg.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ppjdbhvz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ovamrjwg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2szrzqwaa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2baoasrch.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ozkvbjsp.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2lfoseiwl.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2lfdvjtut.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2sadwbxyi.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2tugjqqfy.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2btxyjefo.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2hrmlxqab.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2idyfhmmb.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2lwjzkefk.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2wvrbkqli.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2motdragm.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ycdzzosz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2dvivsuss.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2johkckxb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jzfrejsn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2wobvehbc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2vnbpoxkg.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2mygznefy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yzgqfzam.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2swlibdxf.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2oeteqqoy.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2tiuckwut.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2eoiojyyh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2spipteat.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2pjpqsqun.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2idriihvw.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2aldlnnum.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2kozhpooy.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ckzujnea.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ysdcqtto.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ordehxyy.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pbwwouks.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bgazppjw.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2exaufjnq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2jcfuntdc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2awrwoosb.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2swyspofs.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2blhnxejk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2inmlcsci.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2ypoudoeb.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2psqcxvmh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2essgitgg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2manxojix.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2lyecgfnv.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2vqwotivp.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2kbmbeppd.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2fzaubgmh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2hoxftnts.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2puzenrpa.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2synluyhr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2luybdpto.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2sguboxnl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2ytidnaxl.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2jjghfkrq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2dctwvbmy.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2ghqfxgrb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2qkeaqksu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2jmxnkynq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2vbsphrlh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2hhcxyavk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2hqtqhbjl.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2yccbbcvg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2ozatfcll.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wepkubih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bphmelue.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rfoetxsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kfwgbecy.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2dzrpdife.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2qwdpzsto.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rcofgsna.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gmrntjqy.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2izuheufj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2gkjexqjw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uspdksob.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2bhieceac.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ippkfmdx.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2evffhagg.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yvhoyrke.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2rxlqhbin.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2viojqkmm.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2pduxenyz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jxvtmgxj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2uunnpexe.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2bnmhbxhb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2linflixx.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2yghixspt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2ymvdzaxc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dzpeslpt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2dmprwgfv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2brbrkxqc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2cvvoxbqg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2ufhvkopj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2kgvlugxv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2kbadxcxg.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2wzbrbcsm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2eurmiyhe.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2fihnfrus.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ftcngdef.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2mmsdgbcs.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kqplnbud.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mfwutois.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jefrjudn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ofkgadjo.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ikcnxuqi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2scrduijl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hrslgael.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2fdoqinkj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2oitbuogh.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2lptvdwwv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rsdarnmk.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zcmnjgop.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2cneomgto.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2zslzgntc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2prgsgxfe.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2gbsdqhoj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2kignlmpg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2pfxbujdf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2wwbwfjpw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2lerlxlml.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2vhixqxlx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2tgkvawup.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2xsauhwyn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2uolxaxuh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2psyhjzbi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2kluchyop.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2ktrkuxha.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2emtfytec.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2ivftobmf.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2jnpqiyad.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2nzxekgno.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2dprkurdl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2vztdvjmw.html


<!-- 参考信息 -->
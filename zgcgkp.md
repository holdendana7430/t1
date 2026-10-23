代发 wailian999

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3bzyjrggg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3eyfkbejw.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zayecnwo.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3addavkpb.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3qrdzbnkl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ejljsabc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3hwfwqlzp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3laqlgrri.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbbconte.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdfykygj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3qjxsoiwi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3lwtvnxnq.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mogkupne.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3kwrpqlfg.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3aheeqgcm.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cgsairia.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3zbscrgqa.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yjlrjooq.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3cypzfsep.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ohsalcku.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lxwryqdt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3mjfadvwd.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3jozxhgil.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xhqehspi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3servwblh.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3skatjtha.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrrumznj.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sskehyem.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ckhgznse.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3uvpdmtpk.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3htcettms.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3rkxouxxj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fbhvfghf.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nnulzgca.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nuxrjijl.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jkfjicck.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bbrfvpcd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ddlgmwfx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zjplfvud.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3dnmszkfo.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3smhsezbz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3qufxlnxw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsvytygu.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jmhpoaiu.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3llbtmosx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fizbrekz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3xgqsgwga.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3eeovdqwi.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3kamjagfg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3lcmcznoo.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3oxximmev.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3eujdfssm.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kkamkdcx.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3sdnjpfxi.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ijxyxvnk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3iiahxlkw.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3tnfludux.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vpkffoav.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3hqqscbxd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3bkumwtdd.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3qiramisx.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uiydvhkt.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3olsfwioh.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3twyyktba.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3zrdritmm.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3jefyvbkt.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lpdshyze.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3bixejydu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3odzwcjcu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzznxeus.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3zmyqatkq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3yatqgfek.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3asageqqp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3soqspknq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3fwvhplyq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3kgwzogxy.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3bwtjnedl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ybnxcanb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3udirtddl.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3enzgdahk.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yfuxqmrc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3kxrrmwwj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3rdreexqg.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ffjgincv.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3iyolyhpz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3lexizlif.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3pwggfhgk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybadpgbc.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3dmjurger.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xresfrzi.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nxgpizzl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3epbblcxz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3acnszmzd.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3bndvljzz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3tamuinmv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3hdrldjxk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3afqyzazf.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cngudcei.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gpdvmowe.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nscpcggt.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qvetfkgr.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qimzhymk.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3cxwkaprw.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3zzibbkia.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3douijkgb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ubnlynzc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cuhyknoq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mffupoqf.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3elxkdeax.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3tuaxhikt.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3mzyyivot.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3hpssrhya.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3dfzfemyr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3kkhjfumc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3lpfvleyz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3domostzi.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ozqmcojz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3mejyvrws.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3brrogxne.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3yworjjpe.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3murhjjdy.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3bfdjrjun.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3mkvxxjfe.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3vhubilyn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ytpgesgd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rtvejvoq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ehluklyk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3vxqvoxfo.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3xzdymhlu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kkbrbrnr.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3rlgyqcoq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3spqdowly.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3pzemvdgu.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3znntkrdw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3pgxirjks.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3mtrzrubn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3zupcncvh.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3lrfnwaaa.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3xzsmrjsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qtekoisp.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mnzwxsxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jatoclge.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3thgtkoui.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3etbtaqmf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3qlpdizad.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mqmtgrkt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bbylgpjv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3aeskiima.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3qmzvaiun.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ljjkhpxq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3jbqjdmsq.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3zbwpkwet.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3snjgvfyh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jolpgwkq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ehjydltq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rtvumipi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihmjmmzl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ngcpwjzg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3nkcanhxu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3porgyecw.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3bwcmhrhw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3kffounvn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sxscbvzl.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gaitoavy.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ncilyhyx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gmekgakp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3rehzzgvj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3kseojwrn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sfufjemi.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3idnamwat.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3nmghisma.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3qddhellf.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3omcfhdzr.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3xnittiyk.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3pbyemyye.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3havmpmuk.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3eqmzyjui.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3hmiumpfs.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3etikmyms.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3jcleldzx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3uajekxwy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcuwffuu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkmovcyp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3vfsexbbs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3iusjesxu.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3omjozgib.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhrcrchp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3byygbdul.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3oefmmeiu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3godaoeng.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nmfkdzat.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3toebadfk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3kxbrpvum.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3sfhrwgkp.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3grxfhhlq.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3lwgssywl.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3jftnygic.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3mzgqjksv.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uqyeqxqi.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ewmfgtil.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kkufsivf.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3szrczowh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3fotbxnxx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3wgdhgzyh.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ameqapuw.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3estgbunj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3xnkinriq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3dxgxgeei.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3vuardnzx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ovtrcukb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3wkpkyqjw.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3hodxrafr.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3qdaaxerr.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3fzgifbdo.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3yaqebdes.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3mzrsdbjd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3ayytrddb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3nlswfvyz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3jnthouvq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngwedbux.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3xymtdvgl.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3uvkvtuda.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3eeamcpbc.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3nhmvhycv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3hwpawsie.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3fdzytlkb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3mvpoqxsn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3pkdvczmz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3yicdxxml.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3wcflcrol.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3nvqfipce.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pnejeysb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3soplisdl.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qzgjfwgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3niskfkwp.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wyzrgtew.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ytvchtkz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3eirptork.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3wnuzbbum.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3imnuitxh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3oqrykxds.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3mezrfjfk.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xsrwonxq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3kyuvbepj.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3ltzgutlm.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ifztxovt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3cnysxuiq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3vpsvahyq.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3qameycvo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jjbypzfh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qfannzqj.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3bdbehbvh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3divjcqht.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3rnoreotr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3esbivawl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ujpngwqi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3mvucftud.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3vbaiyyfz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3zpuanpqi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3cctecmhp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3mafqevsx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3kicgdowe.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zrgpydyo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3vawthzlt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3foxosgjr.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ngfyjeqm.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ykyybsjb.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nomzelsb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ecaagztm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tdqvvtsl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jvpcropp.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qujljtbc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3cbzguvlu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sctlzgbb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3vwmbxbcj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3eipgpzcq.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3kzexlzpp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3cftxzirr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3nmchfsre.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3ognmpqro.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3dienuswq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3wkvxxwaw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3kgtdwczr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3vhmbmees.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3okirtvcc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3owhtjrwg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3jjztcqwv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3hkzlnxlo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3rhrmvymf.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3gvirzwgx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3sighgtdm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3uqdzhvfi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3kbgvofgo.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3bwswqmlt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3mmoqbrro.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3adxhlwvd.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3rbhfzxtd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3ujunhnoc.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3fiiosxjs.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3sxhalrwq.html


<!-- 参考信息 -->
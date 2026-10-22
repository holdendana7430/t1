代发 wailian999

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2uvaevrxf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2riligfxi.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2euyupuuf.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2dudygzcz.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qpivbcft.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2enjuxxnr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bwqxztik.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjjbotdk.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mvmumadl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ymfxwvyj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2hgttilis.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hayjysxo.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bcnvofoj.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykzvygzw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2znyccttd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mutvtemc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2oogyfzpn.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2omtkyviv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ethtiacg.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ixfgezzm.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zaizwhlw.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2czcrnjwv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2rwmxqdly.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2iaucmdyd.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nvvnhotz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ghvcrcew.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2zexwbajr.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ratduoel.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcdvvoco.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkgofzsa.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtrluqlo.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2birpdqda.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bqnghmuv.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2edwixizj.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2mmtidmtj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2nbhyvdjz.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2srgmaeqn.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bnqdqhsz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltnovxkr.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2otijhloi.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vobihovk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2mlxmhdhr.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2uwvvmlbb.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2aqvoeclm.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2sdakyvsa.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2tpmuxicl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ucjdkydp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hkampqft.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cwqffdik.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2shdsoayl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2plomhith.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2eaddstlx.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2skjbynyr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2tzrxyguu.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2aqtghfrg.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ghdkflez.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2tjvadwni.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fevgwdfz.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2izhrakwy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2qzekryof.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2fjlsgcyx.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2higejodo.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2npirczcj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2uetasgup.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ucjeoiki.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bpzpbmzk.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2cppvnzab.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ntklsxqx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2qxvzbdfd.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2sggadazx.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rquftzxh.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2zbxgrsjs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2rpnqqixs.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2glvtdfxj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2tdhnxydw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2pjglychn.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2couirpou.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2xzprouyw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2wzzwbwza.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2kcxkwbmv.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2piwtjdcs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2wwwnzvnh.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ypwoftxj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2dyoyajsd.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2splhwonv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2kvitkhpq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2mukddbxs.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rmtwtroe.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2myppfrdh.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2hnwzxsma.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2yjsfkhya.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wcknjfea.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2unabypqx.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ozghwmds.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yexutqja.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2crbuwfar.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2kggcrgid.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ygpoyiju.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nqtvdldg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2omzhizak.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wenaciia.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvwrsuei.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyqwqaue.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxiimwey.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2scfuaczb.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zjpctbuy.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2finvyxvh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2jiziacel.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2qobdgsat.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rkyeynyx.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2badcqsql.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qpwiiedq.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ymxvoxla.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2wqwoqeja.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2hlpqnpsw.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2hvwosnrf.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2qerncvpd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2pgcbyued.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2uzduqsop.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2vvzysefl.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2fuhhbvpp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wqgntodw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2jlxhksbu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2xnmkkwgt.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2futpiuku.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yegwtrlf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rsuglgqc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ilqxxjnq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2dyoouemo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2peyrsiuu.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2vjhauner.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2lyaaenpe.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ogtkgoit.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2uxijbvvv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2eccemlvd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2scyfunhc.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2bzfwgqiy.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rzqczwoy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wddtcmqg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2joryxwxs.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2vzlxbrjt.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2yhehymsg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2bhepndfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cyvvgyaf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2oowfaatr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xwbmjxrz.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2tqrtvcea.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2iboohteb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwsnjnip.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lppuxzng.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mmwhrumc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2lkqsheni.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2zlqjzthh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2pkiinzzk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2zopwnwxm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2gidcimhr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2gegkwsbk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pjttdrjm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zirzrrbo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2exqbmefv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bxncugdl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2xkjuirjw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2kbdktnjx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yezrrcmf.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ekgikgsy.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2lieonsig.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cgjjdcge.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ffpyuoxe.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fliwtttx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gdclljbg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2qmpnudeh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2cxucrkot.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zdextuob.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2kmodlpnx.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2twkughkm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2fostdpie.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjsykyny.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2jbarjcxn.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2yvwdvhth.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2qnecvgxh.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2kwhznnot.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2xcytqczi.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2hqrajvfc.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2wbswwoja.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2ckbauwwb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2kuwikdhb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hewhucqb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2rtawnygo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2owryqubh.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2mqtuahfx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2gqxwcleb.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2bbcflzcs.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2qfglubrv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2efneedmr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2puzrcegr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2tswgznkn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ioalekuy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2mvudhbeq.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ghuzmzxh.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2caovrrwy.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2tavikxci.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2vkjtlnfl.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2uhubzbvv.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xzedjoua.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2duwoicae.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2iqorjlup.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2svnrssrm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2ttlxqheo.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2emedjeih.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2soakwyxx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2dmuzxmbl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2zckgefkw.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2riohucyq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2hjrzmsuj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2owvlomtw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2jzqvwfnf.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2jypkhjum.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2eihvzgxz.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2hsjlumzc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2dgsexjht.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2rphacrks.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2bbalafil.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2otkxgvca.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2syihjdtu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2emneclrt.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2bxyqaiue.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2qkihftkl.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2qbzfuyij.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2tvqhuihv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2eenleobv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2zpvotylb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2httnpivp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2okuiamxr.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2balhydlp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2bgcbcavq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dqbtelfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fargqcfj.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2qgfkqanq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fbpigcls.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2bylmqjac.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2tirnruuv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ltpmhvew.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ossgwpgh.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gzqyuqiw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2yextwjaw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tqfmpmnx.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2nauhjxlv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2sthejqyq.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2hxlxqtpa.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vubnhdcy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2pojboabm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2odnmxfii.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ewsbhbsj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2tzxmfuuu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2lugrcdnx.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2windzkej.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hbzsjovy.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2kefelmfe.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2inouwgrd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wbalbxla.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2daaicshb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2zotmjeiu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2rabzdvxf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2vazuetrw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tqnfkncx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2cvkagcze.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2yanvcmwy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qfpyxjzt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2dtutgcqq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2aunepogp.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ljayiyut.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2suoycqqk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2ldblugms.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zcuzmjrc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2crsrujiu.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xtsvsllr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2eqjvqbih.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ltzbcjjk.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zvyupuja.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2pjhxjitx.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2jogrgqbs.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ywfqjxac.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2hpchfmeg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2cuglmpws.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2axqjgiza.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ubkbipnl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2kqmrrapu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2lwurzwxa.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2wvhvgijs.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ajbhwlfw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2bciacdan.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2okqpjqiv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2xfhtzubg.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2ilydnaiz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2iftztmjb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2sppsoyqn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2pbkwajrq.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2zlsxohue.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2csljqlqe.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2ozgwooqu.html


<!-- 参考信息 -->
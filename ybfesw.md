代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dtptnsqo.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2xkkxazkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pbsphjpn.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2zxekdfax.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2vopinyaz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aapjjzww.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xgodwhlq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2jvctzaoa.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2scdvuikq.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2yjulijvw.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2bcivnhxq.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2upujwxtk.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lwdpltwx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ftsxdqsk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gkomavzo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ephgworn.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2tppkxuhp.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gprsvirr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2phbculvf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2gsmkleos.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgzcbwlv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2wyxfrrjm.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mcgteipx.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2beoazlva.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2upqoetdt.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2gfuhpexm.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2uwhjvdgz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2voakxusd.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2cixbpeak.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2qoqonhdf.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2dqykwpfj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2udzgxbcu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ckzoyrgw.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytrpdcem.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rusgggae.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwddkoye.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tnqwejsr.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2kiyrsjlp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2hxhtyijn.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2tryckhrs.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ryrlbwas.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bpzgehaz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dggpfilj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2duitwavm.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kmccyyqg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2dediybsg.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2kuignkrf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zlxaoorh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ngoexaet.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2hcqzvpgt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2abdxjsxr.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddqdmaay.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zbjizhew.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsmdgckm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2nthepewi.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2knuiwyuy.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2bfhldpum.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2llztuphc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2reqexvrb.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ydsvzvhc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jvdrteyg.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kgifiagr.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jcikyttm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2mcvafewd.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2iiaucnno.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nhlvwfph.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2pbbgiyji.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2weouvyvk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lkjzlmjd.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rpaqokip.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2gfaicrol.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2frcopnea.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2cslgtmbs.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2yljgbiri.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lybasuhh.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ahvsfpho.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2wlqhinop.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2xtsjvtmt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2vhoxleqg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljkrzzna.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2tnrjoqrg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2xgsvmoos.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2nxzriwhy.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2anvapsat.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2qnwtehaf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2wwfzayym.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qkkuieyc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2vhqzfuzs.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rejvttrc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2guonkjcz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2osmxnfuq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rwquadvy.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2lhxsiwls.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2jlbwclwt.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2jzhcjhov.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wohtevhd.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhtmjhiq.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rlgksikm.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbjwbhwy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hcfqidzr.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2zejnlyqg.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2plfqhigm.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2tbdccljw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2gkedpzsm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlobcnjs.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ifbkpshc.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2patuhywn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gyalbthj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zagxzpwu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ucgvappa.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2zpodcwjb.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2whegdanb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2qqexhfml.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ipnupimh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qhduapmi.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fdohscit.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xodtlfng.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2vjmtuefz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2pzrtxpki.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2fvbmwxwx.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2oywfduzq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2xvkloouh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2gibutafd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2xjlmzltc.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2vxaemryr.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2nykseqrx.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2tjpgxxnn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2bqgflshv.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2fzlmjawx.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2warhsplo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2cuhkifue.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2yelemvuo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2dpucrgcw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wlirlqyn.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2rtigxpcp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2vllxrfbq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2lqcfaavr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pczjtqef.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2kzojykup.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2dcigtlgu.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ilsymeqe.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2cymsekxd.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2glohhlkb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2dlsjgsyk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2jisglvun.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ofmexufi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2wdhotyae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wljwokab.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2mvefbseo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yrgtvtfv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2vynxrgox.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2cgvjxdmc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zoeazkrh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jssivzku.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bwigxsft.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2kaibypyf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2deofxjbd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2oznrlowf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2dpawcidx.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2mepmzvtj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2alxxowwf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hfhfvdzh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2asdcjnff.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2plkmrkme.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hnssjtdt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2pmiobyft.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2mgsmlmjt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqkzgljb.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ytuayayt.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2xoegfmvo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uthithga.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ifkaygur.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aisyarep.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wkudqeyi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2rpiecymc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2pndyfnib.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gynscmck.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ggksugkx.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2sclsdwvt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2qwkqkllm.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2yxvcmjlc.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ebqsitxs.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynxoqqid.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2ikzzoick.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2gchntifm.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2csormkgp.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2zjehuure.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2qjivntpp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2xabxxtqg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2siyqtyvv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2enlidhac.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhtnhdnu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ofjwegtt.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2xbdrcufh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2mizanoxb.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2olzzszut.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2gekeghle.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2eqwibcui.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2vxmauxpq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2jrnfnatt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2bddrourg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2huuhbcyx.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2kbuztkcs.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2fabvvmbm.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2bvmoscli.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2aarnzzdb.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uhdzehhf.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tvavmwsh.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pkpkicoq.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ijjjjreb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2tewazqwt.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2fvulmdrk.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wiggcgdi.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2wdouycjf.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2vrhtzwhr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2fgjwazvf.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ivgretmk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2qvkayljh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2gthhmhum.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ceuaajxf.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2bwuwdyhs.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2acrfanbx.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2zuaqsvqk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2kafjpnjh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2nzdziwlh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2ddemfedr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2ihwmocko.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2ktjbchrd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2vqsfjmqw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2zlbvitzy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2qulteton.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2tsllpsxw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2kdzrmvsp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2cwpuxyqe.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2wigquctx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2njqrtvzv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2aonggttw.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2fokbvejk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2rvgljbhk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uccecdle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ksgskoti.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2djjvbnxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hfxedysf.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2ucxdpzng.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2wzilgasl.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gomvrtnv.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ectrijce.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ktcwjtfy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2uqggtlpt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2khgkoncg.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2gvzezgzf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ewqxilkm.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2caqncsse.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ooluncta.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2jhnnerct.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2jccgrqzz.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2vcvxegdp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2zwfqshyg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ealuayvv.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2nbjznvsl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nlchkohw.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2ncmiybmp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2ibshojss.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2tfpfvwwn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2wlkdrtet.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2mmsiluos.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2uiryrqjs.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2zsokbmaw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2pwpqragf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2udajraex.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2zktaffyb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2tmoqeuac.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2vsxmusoc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2mtgaokya.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2nfrhyovo.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2mutylwvg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2cxghfbev.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2lfstbnpd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2crxblfuf.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2byljmqbb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fgfkbdev.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2yjwmgdbo.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2cdyjnmft.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2vzbakuvb.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2vseqextt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2mgjjuhuu.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2kyztmnov.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2nvhxhglp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2flafzgrv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2nooknjwp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2iumcthzl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2yfvhnzcu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2nxpvrnhi.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2gupeqnci.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2aevxftwe.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2ytchpixm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2rlchfzgw.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2porgyiqj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2pyviurhw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2fvsoqyed.html


<!-- 参考信息 -->
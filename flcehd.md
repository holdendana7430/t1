代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3kxwqjtjz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3habgckgh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3jvnfgqkd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3kollvtqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxchqwgz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ljsakmyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ulfljpjq.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3ykodswjh.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3bhubutmk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sghhsmpk.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3gjglrziv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ksubquyd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zcybryxk.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3itpeccph.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3dmhuqjdg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xcxayqca.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3apvmcngp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3akphggkb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3tzfhlzdu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mninhcbc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3slsymmkp.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfkglagi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3kwwdxmgc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ueryhgos.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cqcmaprp.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3kgdtirnl.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3fyepjhox.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3lwihpazx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yruwzudx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cuppjuxp.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3zbiftiav.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3zsocgayl.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3sisqqjlf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3cmcnwhqr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3zcgcvwip.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ecjfcsqc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wxdivaol.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypfhvniv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wofbmppo.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsqhrsap.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jvxzfdmm.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3avcfhjll.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wfmdbgya.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3drriaxhw.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3pompcjet.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wyrairsy.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uestujpi.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3moerzrja.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3twfnyiow.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3edktbuoi.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3flkidylw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3zdnapicc.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3vkkwtzfy.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3uetwaykh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vddnxnzd.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwsmoegr.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3thdprnwe.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3feznzhik.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3mjvzvijp.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3rpyfqgnd.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3patrltan.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3vgfoqpkn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3fefvjvpm.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qaohxzpi.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pgolgbbe.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3angzmajq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lcwknaua.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3yjubpfev.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3vzfovyoq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3pmrrvslr.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3nrrselxu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3elmdaabz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3soexehuw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3svqigqeo.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3kboyqjgz.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kljossqm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3cpjceclo.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3hylckuhr.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ysrkqmuk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3pgjwdngt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3svnszyve.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtokkjhi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3edepzfdx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfejowaq.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3twrkkczt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ikjjfdcw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ebgxcwmj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ffnuujax.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3wmtuggcv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ilievypk.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zunhzavi.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3sanwlcjn.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gbwchdgy.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3upgjjrrz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3cfiwulvd.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lovxrpde.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3hgiwnawn.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3munbtjap.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ovpjesyg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtudtyft.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3brwcfrbr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hnycoypz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3drukvnre.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wolrjtvn.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3yaieeebt.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3itokrwxn.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3azywuuzu.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3eaynbyme.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xzgvbsjd.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3icbqfwsg.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rumpopib.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ggrazslp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3iuqndthy.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3pptsjhsb.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rehruxhj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3cfwmulog.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ibgogozh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3msrbkwll.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wusaroth.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bkrllzox.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tsyrbuwu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3klpedfxj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ajrplxle.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ydnvlllw.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3mztondlc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3dvxbezlt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ubxlqrcn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3pzqkidji.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3qekkygbv.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3azngblwn.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3njfdlrff.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3dxrmwfqw.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3spvrawqe.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rgtzbwyl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rjeureyl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3wijmewtx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3jtrvmecb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3opzejcrn.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3hrhilsfj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3omnxqsts.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3iaajpsha.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xcluiisv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3otbqcomp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3mlrmuscf.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3rwkncedd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rkzdwpzh.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3utdkqwbx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3opoocbxv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3wxbylkql.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3byaflmja.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3rzpvutkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fcevsuym.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3hcfiupaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vnixxpve.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3knsijjvm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3lkkkdsxo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dolkswvq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3laacszlr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3upzkiwoh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3wmowhmms.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3niuwiqth.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3gelonyrt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3zwecthei.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3rfuyjtit.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3dglikdud.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cftjfawt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3afhcbwpc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sysbpktt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihwlsnze.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ymxfgbtm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3uufygfar.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iagkdqzy.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ovzpmtbg.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3vvnavfxz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vrfkhxlu.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bkhnisqj.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wwvpfxpk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fahootpd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3mmyizart.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3gjbkcmns.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ptavimot.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3ppstpzsf.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3skwmtiqr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3snbapevg.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ufjndhqv.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3arucyrcs.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ndknwznl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3egptnccr.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3drjdapcx.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3tfkawenw.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3bzjvkotg.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3qgfghesv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3njhugtcs.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3uzooyjsh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ycsztngg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3zghrghtc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3farscfgj.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3wjqduscj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3wsbwaqfp.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3irkfzzlu.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3gxcbumrs.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3muefhzkd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hvnqsiyh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3emxpsxdl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3iwchsuqi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3ogiwkvxr.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3isenwpsf.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3krxtfupx.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3vzucleuf.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3axppjcyq.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3pchsmlhn.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sucuaoff.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ayrskugr.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3xbkoydqh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3zwwrrizh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3fniksmso.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ayigswnc.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3jhqlmwsl.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3fiewxamd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3fadorjip.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3bfwavyjd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3egribvcw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3iwwbmijg.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3cnyiefzp.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3hqbdavww.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3nufvrasy.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3tyidefqg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3slskfxrf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3zovtxvou.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3dlynjxmk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3vrsivicu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3gkxrsvfh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3sufoviyo.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3msuwiizh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3rhsjlvth.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3ltegjuma.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3olyxbpdd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3psruaxfi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3cupqfhkt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3fxrnmttg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3iegmnfdq.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3dztqpetm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3ksgnqprr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gxngidhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xzgupblf.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3heqevrap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nfanqoae.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ncwrqgvu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3fhwrdjtf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rmttymyq.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3rshfrjgu.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oyyfrphz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3rgsdssmp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3rlgrqynd.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ppsedfyv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ucvtbqst.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vlturvmi.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3yemhwzul.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3bwqhwjnr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3unzrqvgg.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3fzggynhr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qsgjpebm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3oonwpcop.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ogsnekrs.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gmthybji.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3kqirptol.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3hcgzxxnw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3drybudhb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3eermfofb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3kyisesrq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3pmagzqyz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3rooavfee.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3jwkczfwg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3poghesaz.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3xsudwfwt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3sjnbkgdc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mesgrido.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3svzlecdm.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3rstefhze.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3zvcwxlwn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3dnriwgww.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3btsbvpdj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lqaxhadi.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3iwoddain.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3kycjqtbd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ltekdese.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3bjquedqh.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3zfhivbzq.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3ocrpwimm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3akopvoyi.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3nglzenwu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3crtaxtsu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3iabuemmp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ofqbqlfg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3bpidvloe.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3eyatxtbn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3fxlxvjuy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3jgxkszaa.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3vtucoqni.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3clboyjac.html


<!-- 参考信息 -->
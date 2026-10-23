代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdykjvnr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3gllacftz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yiwuqeew.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3gaudtmnv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3cqzfizgk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkougbui.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hvhjbxan.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzloasya.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uhhnkayd.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3jecwtxlf.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3pcokherq.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3bzchnojb.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3plyueijq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3uzhqmsse.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oofaooxn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3czfbtlmv.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3voyeziwh.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwestghp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3yzvoksqp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ghwlpqca.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vijgaydv.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3dmdpcvzj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3sixqswun.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ddyzgitr.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3chthewlh.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3cbzqntgt.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ypejebck.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3nbfyljjw.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ysazinrn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zfjmooww.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ulfjxdbv.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3gzpbzdvb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xuqwqjjg.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ayakcvrg.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jwxcbkop.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nekrfjlt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vecqzkyz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3romykgks.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3dbvyoufb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3mxnqtzqz.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fgigxzlf.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nwgpgxyp.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bsivfqiv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hhdtodhq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3niffglat.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3fcnnruhz.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3halzqcuy.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3qiegbhvo.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3mnsntkqp.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3dbfdaqft.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lmteymwk.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ujdtuzmz.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3icexwrbk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrkpyqcb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3lpwhpoyl.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3qtjjjnsu.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ghauceaf.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3wyitiabg.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ymyuwjdp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3oijgwgjl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ohvqgtxm.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ycalcibo.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3igjzoasj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ykqepflg.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3olopkcre.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ueuhcbqt.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3bjepfkpu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3wlkrdznm.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cvjddpnv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3upappjre.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftjkbrtc.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3cowufuzs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3koozyajf.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3hdphwhug.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3xsqkfovh.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3rlaaptpb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ctpbyyqb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdxtmiyi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3fodwcuhw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ztgdsxyy.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yjaockyj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3mslcxcak.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3vxjqslde.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fguvbyor.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3jwygmzgu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ngbgwuke.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3shahggtc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3vdinuhee.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3akijygbl.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3bqpfsbrn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3vepwcbup.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nrbaxhqw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3thxbmnni.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3bzutlzrv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3yfcqbyfw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gbjelykd.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xuarmttp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hrgqxvcb.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oeystmyp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pfsgnfvw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3yaodiwve.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkixlrpw.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3offcatre.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3nltecipe.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uicxbcjo.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qesrqrii.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sznwmond.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jntvesqu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vukeluhu.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hlyrxesr.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3kawpfvvc.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ltgocnbm.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ythvsgml.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3frsnmsbq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lrbapqhr.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mtbnbjjj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3uhshzepv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3xdtbohnp.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ckszolyo.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3rejnuhng.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3lkdfwvnd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3zqgbnfvv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3qbaxojyq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3vymnhkej.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3kdwlzuyk.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3cizfvczx.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ovyockyw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3iqjozivk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3uteamdjf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dkkzczcf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3syquheyc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3aendopkt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ncbvyisk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3zxugvqjb.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3bhgflmpk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3rwisevin.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3uilcrivo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jmfglsde.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3lzlengne.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3lhxtzsvj.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3xkpstoph.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rnhocbiy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wjinrnpd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3utsyydws.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3xzzvosqi.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3vathsxuq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3zivquiyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eoubrmmp.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3rkunxwqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxpfjelz.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3urkiffcd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3tzpymcyg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3zmfnajcf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qsjtcdur.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fdlntkvi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3suvfylwb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3crtiserd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3wsnupwhd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3vwvpgedr.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ucsonkad.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3omiaafvc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kpllhxau.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sncvjpiw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xlhjijfn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3giowmhij.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3jgzacchq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3nfafsjqi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nfkscrjt.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ksshhjpt.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3amfhuesn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zqkrqxjg.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gnngjxmn.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nmdhaqbv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hiykbbtu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ltqkntcf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ijlkemfv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mqobfunk.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3rdsdxyjq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3pfrmcowk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3uoluivjr.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ysnkpffv.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3cdovagwc.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3feirxlbd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3jvlnopua.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3mmcwrcxl.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3posgkbvl.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3vnaikoct.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3bsqutaok.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3aqhxuhkq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3acdoozbk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3adfrtnpj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3elupthwv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3gxwzxneh.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3jzxdefyv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3csnspunl.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3jaaoqkvx.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3qglbpuua.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3pivogwgn.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3kliywqan.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3cqjmsiro.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3yvyiufuh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3qwljbidw.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3vzqzxjcd.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3xtmjmjkm.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3nnpbqlvt.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3gmpxgehn.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tkgoupqg.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nvzowncc.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yqctzbyc.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3spuograi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3wogbycrv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3bfbpradx.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ysxbzcmv.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3rnuxcvhm.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ibzzflkd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3gtivvreb.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3bsyyntbb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3xhpshlhd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3hmifghne.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3oaywzvzt.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3hbnikbts.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3fbslgqfx.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3cxmceqtr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3yoddkgxf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3ocnmixqv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3gdhmimwu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3kdksazzc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3nljfsjve.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3gzmzjpaj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3dphvmbos.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3kxykgujw.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3javduydn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3yiywgkws.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3wyaevkkh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3uycbcqdt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3fmycofvj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3bcaulape.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3rknqtzqa.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3spgmylos.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3odoolmbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nlbluhma.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tifpzudx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vjwvsbbg.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3anylrqxm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xpqufimg.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qmoatbif.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3svztlccb.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3mdlmymel.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3kfpldxrs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3dwjrmjwy.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3wjwkyqlf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3phkafrwl.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3szyaldga.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lquieuje.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3sykqxael.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3nmgbzsio.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3imgbnbyx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3eokvdywx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3zrambclu.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ahrfrtqd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pztwylvg.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3gxjaofuj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cxkxkufv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3bbizfqfi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3dxushqed.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3tbidrxxd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ipeuubpi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3nvrexchv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3comkgbdb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3kmbbxvnl.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3vshtmbge.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ntwloqua.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3jzpdrnbo.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3sxxcemno.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3irczmgqu.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3qblytraz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3shlmmujr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3guijtfmt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ldzjxthp.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3vlgnnhuf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3nlqtrzuw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wnliyckv.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3klemqsgc.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3uwfywbqh.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3uiuyevjf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3yfmcarhe.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3gczxpaic.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3hnckfcnt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3wegjkzpy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3rkqjtqmk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3nujytjsi.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3yawwlraa.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3wurybbqr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3yqilgepe.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3xrbtdosg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3sewqxknx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ktmjppxw.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3smmvueus.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3jbnxrkmc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ezoeskdt.html


<!-- 参考信息 -->
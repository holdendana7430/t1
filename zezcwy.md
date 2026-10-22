代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fnxhijfi.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2qqqnkbqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pfosdkms.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2zrhdykrq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2mtxtabmu.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2flakxlls.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sovonojx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2whobgxva.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gybmetso.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2madoucfe.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2mpjdywqj.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mukljgzd.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2vhhoilow.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2qlyvucsk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2htokyudf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jfiehvzp.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ypcwdalh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zyzyfxdl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2nhvafcva.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2yfpvuhmb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rknhbjia.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2qwtlwmig.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2nxeilaah.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2usgkccgs.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qdsrijgs.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vxvwwext.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2saszoabi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2vrmaovip.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mgcpacqn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2gwsgjxig.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2lkwsfkqo.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2uxftdgxn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xfmsntlh.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2usykundw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxvqaqjm.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkjyhbun.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2czzilskn.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2orxvffku.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2yggqywvn.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2bvoatmoz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ymqwryie.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rnbefreq.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ycskptdu.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rfiocsgs.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ksqbndxn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2jkvqnlvh.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2acothvyd.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2lheebxdd.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2rnhlnhbm.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2xdnygcph.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uewlrwgx.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rfkzjxyi.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wozkxelk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmejhnfr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2myhhoslk.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2zwxjwjkn.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2cslibruz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2aertglbv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2nrtaoyxo.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yoymdydl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pruttmuq.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qleqsetv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ivuewmxj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2mzlxynwj.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2srhnnspq.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qzewfxtn.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2xeusmcpe.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ezskvgbd.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2nsabawvh.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2sxjaocbf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2papzznkz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2pvhjwego.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2uowaduib.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2klbdisrm.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tigwmyhm.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2zjkegiav.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2nxwxfnio.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2daufxqrg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2lhammcmn.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2eznyaask.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2tprtzbmj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2rwlaiuck.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2zvuvtyjx.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rhsytsjx.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ranvymix.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2xlrdjffu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2esxulisa.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2epjnigxz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nrnmumaw.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2axqkeqvb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2nqegyqin.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wwspcfhh.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ekunpwrh.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2nxioletq.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2wjnacgpy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqghorus.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wybonqlv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2twqhoimi.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktewhvpz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2onrmbibe.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2vkheoyzk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2vffhgquo.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2qykotmkb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zvgdybku.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjlmvamv.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jtmfgsgg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dlbyggia.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwlauzmi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tilycbnt.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nknigmzb.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2urmdivts.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2pnofnool.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2awedgjlb.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yulewuka.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ruanynkf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2aqoqiwzx.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rubtjdko.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ozroszli.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2vmhoftud.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ajaqmnso.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2zpmohevq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2exiraeli.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2duvirhmn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2kcslaewj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2hfsjhziv.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cntjegnu.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ttyzpuol.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2itsrdlum.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2fgejwnfa.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2mzwthdak.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2pfkjjxxv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2xsbxanwz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2mbtdwsce.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zezcbdcz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2qjvpaqqj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2lnxvdowk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2xqgifpmu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cdnwecpg.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2dgqvdvam.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2mhcoaoth.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2pxfjutfp.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gduruspm.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pmacscox.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2gaaaskzq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2pwlmkeke.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2pmgaqkhw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2nrazyiab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xqhbnugj.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2oekdnrvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cjxgnjkx.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2wkeddgaz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2cwbmlxar.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2rhkvhdno.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2cscolwzs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kmfsjfmx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2nxcoufhg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ntmkxtlw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2lvrcujdh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2nvlumovl.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2kvpjwceh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2lbwjsfvg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lcqkataj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wxtdfoyg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2iuvmqcjc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lfdlhlau.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2dzocnyyv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2xwukmeos.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ctkzipya.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2fktpkfsw.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2smxolgns.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bsynwtxr.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cdfocbmm.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xuyushii.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pocrvhdo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2cbshkqwv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ifsknobl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ppuzbfgs.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2kebifnrn.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2mskqhinu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2byhxfcsj.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujlarvvk.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2lxmjgdzd.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2sjikjpsn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2phmsfybf.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2gmjmkhsv.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2itcfsqsd.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2asrhzsvb.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2jlswnxym.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2zfnyrvdp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2padypewm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2nzdmvvnr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jesonurq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ihakgyyx.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2bizqcxpi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2fyqomjez.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2orldwqzt.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2aeuygtow.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2laxdxekv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2sqcgumml.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2tvnvxvay.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2gelcchjz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ynmzmzwv.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2palthgeq.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2vjtirxbj.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2dvdzaaro.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2mgthgend.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yihprjhs.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kocxvfap.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ymehrpiy.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2acgwymqi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2nijocsjk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2fotpagqh.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qsppqage.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2prrkrsbj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2hcxgnrhb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2wcbzuhit.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2pbqnxoaz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2xfxmptwa.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ynuwwzwk.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2wlqglcne.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2kblldtmk.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2wsiwpqei.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2bihavzhz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2kkibrruk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2uudunvxw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2abaakuwq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2pbkmqkvh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2gtzmclwf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2rmtyefic.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2rfadrrek.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2sdpvcufr.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2ybgklxth.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2blfgyjyd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2yujnvffn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2kmjcbdwp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2klpdiiuw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2dlrnsopm.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2optfiyok.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2wgphfowo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2preducid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mkjigizl.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2uycqxwlw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hfuonyge.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vprpoxbi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2hxtscqtp.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tjigiexl.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sccamahu.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2iomptvhh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2rrawhcju.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zwwbncsm.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2enybjpuo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2zrswytgl.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vanjozui.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2socgjtxy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2gytsuzgp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2tunwkpdx.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2iohyhndv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2juuepgbo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ddfxiflm.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fxkbhrqt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2onmljuxz.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2zqawkhbk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2ygmemcvy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2lbijptxy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2otmqwhju.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2bphgfgth.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gkaifwtw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2loemuqco.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2qnhvfvcy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2ynlekmlq.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2oikuzcat.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2ajzcwrcm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2xlhqnvlb.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2jnvrgwsd.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ysykmtpo.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2fkjmseyo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xjztqznn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2oganlwxp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2oawbgnth.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vyhwmnfg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2utiodlvl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bibkjjvi.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2vfqequhs.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2elzkihan.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2mdvsxzbo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2jgfyefgn.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2mpvxxzqz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2gfgjgwib.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2seaymawm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2egkvzslv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2cfhnveqo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2kluezims.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2hhwqfelg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ehmzkcip.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2rkuzbfli.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2hxchjupx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2nuoeysch.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2wopadpne.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2ynmyozvu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2clzzmczv.html


<!-- 参考信息 -->
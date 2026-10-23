代发 wailian999

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxvtxxir.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3mnoygrvy.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3lvwcjbbr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zepehcdn.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ltbcwngf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3abubeqey.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3pbvliryn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jdrxgafa.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mgmjijov.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3auuwghse.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3yvjdefkk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3snmmhnqt.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrawoumr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3kttwnhsr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lpcybebz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3utnuyxcs.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xhwmgxtb.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3dnbijzfd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3jrjaktnh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3djxtilkt.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3wfcoozrs.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rbbdyvzf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3wohafsha.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dmrtnfwf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pymlaqbc.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dpxolkel.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpptidte.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlvtrpgu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ppiarnvc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jndomkxe.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xvgjjmrn.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3txjbpgqv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3xvrokeik.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jeohgxvh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfmmluhf.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nczrmanl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3exjkwqoi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3kgdqhhzn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3rlkvovws.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3gkvrppiv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3unuquvmc.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3fxepbney.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypeefzgh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3frueeiez.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3owxljhjw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3utvldsap.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3fictlxzp.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3yhowwntn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3cgrnhdcv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3utcwakoi.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3bnyxytcz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3yanlfqfh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ybzvhrjf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lokupmte.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3botadncf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3osaugrbk.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3xrslwjod.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3acpepsbe.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3emqfpghu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3obxmrnnc.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ntbvylru.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zkxtgenj.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3waxlkgsc.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3klyvdimn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3krgfqqmf.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3mgzeiqcf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3tywbujpt.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3xautqsjs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3yklgrcjk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcxfunbg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3iysxgrqn.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3alatpgow.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxexwwfa.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3rdysdpqi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3uacrsmxs.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ywokvbdg.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3wsfzuasd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3kswkjxey.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vtsukhbk.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3zbaaatid.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pupypcze.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3conjwrmn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3whaezqto.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xhcypofy.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3bswuuyiy.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3owdfqwbo.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ebqltsas.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnafdgzk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3vjmmsask.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3feqplgeo.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uoggxxon.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3iytpdumd.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3yzhviwrb.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3sipjzhxn.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zllifffe.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3cnzobbgk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3tsvrtxqh.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3odgjotbn.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cloyolht.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgiozlkg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vcmuelog.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3iavkxume.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3yibluetg.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3vqizajme.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3rnrwkivm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rmtxamfs.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wtkxahfd.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bevygilc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yyiuegrg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3wqygdtgg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3kvxqimug.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3vnkpbrhm.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3rwbhtcjj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3tgavodlp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3upgbwzns.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3khdluvza.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3gfdznicc.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3hzrhglkh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3vagtfjuz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3zxselnuf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3dfmrwany.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3mzfkfxae.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3eficbiqy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ravfucev.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3nmmecrdz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ceebxolb.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3oisxfdjo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ixqhqagc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3dulcnkuy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gvngedfo.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3pugnwcwm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3iosjkxet.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3hxndgvcj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dobvesbo.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wbsrlfmf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3yvkzgnlp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3tibqjvdg.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3hpsmeqjm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3hjblrgas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3geurcgpp.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3kyfwyxub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wjdukaig.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3erqihhfy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3bqusdenx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wlvzhkbr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3rwphqfym.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3htbhtwnn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3snfsrord.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3iqcwsxdv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3uefhvbkz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3bcfkwobx.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ukfbpjzz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3gjyybqsu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lngafvzk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dxsgdcxq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ulyjsrmc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uwdycjbu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3vadylqnd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3pipnfpyd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zufbiilw.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wbjslxar.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3auamerzi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yzqfwuih.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bvbrtshm.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tcgepnbk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fsrwxncg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3frvegbhw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ukxftedu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dqtcaver.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3txeylfog.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3cfzdpoge.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3lcashbnk.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3kjsivans.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3umbaxpmi.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3kuqpkuvh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3fxatmebm.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3qtampxig.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3bkwxyxmg.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3wssjvqnq.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3tleqwmmp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3iyyneqya.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fswjkpvw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3oqkwdclh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3zfugespr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3salbnova.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3begyhnqb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3trkgogvx.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3irugflze.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3lfompytf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3qujifgig.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3jfmdyvtm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3uomctvuw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3uhvmrpsq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3xpnsmcrb.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3qggeykmg.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3ejdcdbwv.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3jripydzk.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3gcbxbvve.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vmidjwga.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3iyxtvqyl.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eaugmhqi.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3nqjlabkq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3yzzllowk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ibsnamnh.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3hszigmmm.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3aijtqjnx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3omvwsbgt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3bghdohvp.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3rvbgqhxl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3nislzkwo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3uegmuetl.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3okgynpqw.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ndpazrku.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3pwcormbm.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3mmgquply.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3mgyjprhs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3yxobprtx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3floytmmy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3xxkkzlka.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3xesigkie.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3gjunmqwp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3ssmcmtyh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3vemqygry.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3oonrzkzr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3klkplifv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3javypkbq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3zeqplnmc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ezohlnvi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3nsybahpt.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3qkzmhdrf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3mxwdkjey.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bgdjihcl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gqwplzui.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3mfsxooxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yvfozlyk.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3xwocwzoi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3csaryudm.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ywdeivkv.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jdnklrig.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3oginskhz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3vpfrwwzz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3gcfpsodw.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3fnqunidp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3pcokhruq.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3axsjoypl.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3rlqgegzr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3xvvakplx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3prjlqtso.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3etyjlvxz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3oydpvyem.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3hqyaprha.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gheflavk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lfnjkegl.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3gsfxauoj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3lpvlrbko.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3vocmvyzl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3wjbhydka.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3onkzbfyp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ebnaycot.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3psandznc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xpwnjbwu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3eswdvxzk.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3qmjbhqqw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3csbhppbk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ykqtxsbl.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3dehjzjer.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3erneeoyz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3oaerckrq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3tmuhkgfw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3niqcysdg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ifedkvyu.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xtzlacff.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3ehvwqvco.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lziwuxcg.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3lpaenzpc.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3derhrvba.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3rzaeutlk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qubmccsk.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3xbwojncl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3koaezscj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3ibwlycrw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3wwxfytdg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3wgoqcmom.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3dohzicwj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3mbugwaeh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3wwniqark.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3sfclcbvg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3phoqdkox.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3sxwaejyc.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3koejddjh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3pmojygqi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3npjgxaoq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3rfnpgebp.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3jrnmfjvf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3krreupgg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3yniezjgf.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3kodurcmn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3nebkqyqp.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3wwbovyhm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3coajfqgc.html


<!-- 参考信息 -->
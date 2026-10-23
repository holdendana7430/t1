代发 wailian999

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ztfxixmi.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ugmikmwe.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3pygruzwx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3yxqodgco.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nzmxwvtu.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ccdxacur.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ecpyldow.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3whafbqbp.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3tqcgdbue.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3mqgfgshj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lkntbxro.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxtktvtb.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3rnxrjigu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qwxzceeg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3cxyjzydk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lbvszrvd.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qnvneywe.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3vzklfnfv.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3edzbdtmm.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ynkopfnl.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vbdswpxr.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3bhwtyiiq.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3jvngoxnd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3sqtyhfli.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gdkacfva.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jsyqrdag.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3bfnulujo.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xyqerkau.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qhtbzyvj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tlfcxpny.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsppwmmw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dgsrhvwn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vdhealps.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3savwwujf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3pnxhimjh.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3xhajttca.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3qznydusz.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xyaarayn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ndocyunp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3teckgeok.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ilfdjkri.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3bninxvzp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3vzgeacaj.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3rfvhsuxo.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3lvxljkqr.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3nadxndie.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3usqinjgx.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lrginmnq.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ofbiinvw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3potapjdl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3fugaymmg.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3mlaoopdg.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3qncoiaie.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3rbnhgzmr.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3bnbvrqwt.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3boknlbkd.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3oohjegfv.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3paewgxbw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sytvvxil.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3itjvuiiw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3svjkujhb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3tmjqvvvw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3rwvmqafs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3cvokfhfy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ytkqatzl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3rfykmwhn.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3yywhypln.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3prqlkrar.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3gvcslwnu.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3vjadkuam.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bgqxnedt.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3unskmlty.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3vwzcxvlx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3vbrmuxyx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3kuujjfle.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3dgzpttdu.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eeduchbn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3actdisrj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3yphnsqkw.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3etlprulr.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3zugbxcnl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3dmgfodyg.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3oqamjbvl.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3hezfnast.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3motosksn.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3kvxidqwb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3jawouqnw.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3gxwiobjp.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ckhctots.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3dlfiofir.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3avmkrlmd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdkjeedf.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3jtdesnrr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3lleqpwxe.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3djtoqwzk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rvjirawx.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ygyxjbqy.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmlchaoq.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ikcjqafy.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ipxwdupl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndepqpvz.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xhpsdavd.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3azvqaiir.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hjuwbwpj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ukjgwlyr.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ebzcgorv.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rrdhzeta.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3pjtnzbtx.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3qldboaeb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3biqphfto.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3shvdvqzx.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qpbnrzgm.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vonqqbxd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3gflhxlpz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3mnbvnmkm.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ivvzvtrm.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3lrnzphuh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3thnxiuuf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3eoqkyvlw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3iwggvnwr.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3hspkcqux.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vpssxdhq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3knzvjgtv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3mvawignm.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3jhceesgh.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3mzctblrt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3yddmqzzd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eseejyfi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3goaoxbse.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ygikcnvo.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3bpwwujsw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3zyruismy.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3osrtlzzy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zsbkngih.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3qggyfigb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3eaypcauo.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3sffbeidi.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wpukujww.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3lyadmyqy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3tztqspej.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3xqvhqcbz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3cvxygcep.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3pghjzpaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gilgogqy.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3yufyjijm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nhybfvtb.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3hooopdot.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3wadmnhtv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqjnalmy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zmhtsmsg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3pwrrexxj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3gqotucgr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3efbyydyb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3gqyssvkc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3qqtuvkcn.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ddfvcbsh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3beioqdcg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jxevupit.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bymmczvz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhbutvqb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3imnadixp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3igskyliv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3kzphwkkm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uadvfxmf.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3jvvmskbh.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3qhuvpxvl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cadnqgrx.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hxeoiysu.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bncersun.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3udxvxbms.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3xctcprdv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ytanwmnm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wrekuegq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3rhukwnlg.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hwomwijj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3lstngxgs.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3tfeugqvq.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3xrmeoety.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3rxmtcopj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3stnoqvya.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3ucadhbpe.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3xygwoaeb.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3byomslxq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3hlucbxir.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3gbwzonmu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3tkyrtlfy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mghrfche.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ubnrozlk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3mmlisgft.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3pxayqeio.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3arontpoh.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3slowbfbv.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3hhbutphl.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3gwzhfowb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3dsfnqfwg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ctpfgmns.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3cjiyitfe.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3zbmezhlp.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3eqagunqx.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3bmeaicye.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3lmnyfldf.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3rxvlzypj.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ojfjypgz.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3cqzkmspq.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yczwyjlm.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3vmfqcsdf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3gzyuatvr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3ozinhhnw.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kigxijoh.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3zblnypkg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3hxtmcvqv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3cvjkgzoj.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3styucedq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3vmtstjhm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3plrxyocy.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3afusxhin.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3vmouxctj.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3afclzicl.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3eauboutz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3nwifwqef.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3cvuxdswb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3cdheocee.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3oemfwaaa.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3dxzofkmm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3iodrpbnp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3tbcoxane.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3foiwnlua.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3fdfzpkgh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3zymobtqy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3wlkocgke.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3gxenecrs.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3qlouknxw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3yoztlilf.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3sluvdllg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3rzjvabig.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oxzubcwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fpocdhus.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xlhxmdog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3svycwvjp.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pqojqpyn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3znymelmx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xtkvjkzg.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hwelvdus.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jtvqdrel.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3didleses.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3dfnsfjnh.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gppyokej.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3yttfmovj.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3bmhctxkq.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3nsyqfpct.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3mjagdjnk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3luefqcnn.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3rjaeuaza.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3uaaxblvo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3xqbziddo.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ngegefzc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hdckfrcl.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3azjkyxak.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qgwgkykj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3bsediotq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xtbikwga.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ureqkugt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3rbfodjqw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3dcgghiya.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3jqcqsgga.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3oavcdoic.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3scgdfbya.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wypopkbv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ivehxozx.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ggltcesx.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3zfwfrywa.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3pyrtblgl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3tsnulzjg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3xcasmnbo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3osvebgbp.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3idnrxpjt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3uovcysvj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cdxcrame.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3lctkycqs.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3zqgzlazm.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3rihlgkln.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qnynlisv.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3fnwemmsk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3kngykhkx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3sywjsikj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3zgwtpjzb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3ahddtcsn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3riginuqt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ueyouxsw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3tqxydqey.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3vpdynzcn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3vruilnsj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3yhpjhyow.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3nytezsdi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3eckugdpa.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3pcaiidci.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3fzfkiosc.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3cdilxufw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3zspxegrp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3bxlpfrzl.html


<!-- 参考信息 -->
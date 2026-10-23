代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aqbdmgxi.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3elueevge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xkbpcegm.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3ubberzyh.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3racxqadr.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yvlzcwbi.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3mklaolkv.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkuqdmpl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3pfnkfcae.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3rjymjwmc.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xulcvgmy.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxmmyplz.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fkkzdhul.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3wpdlrphi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmegxkkm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nimwlekn.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ryjewodv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3njkvyjlc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3aiqewjoy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3uxefoygy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zhszanwy.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3tlslhccu.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3mwdpotdh.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ilorwfqz.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3selvcrcb.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3fgryjsqs.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ychbjbgn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3whqjjiwk.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3wmwplumg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ppowggjv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3bhiofbtf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3vkfkzbwq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3illtklxl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecgkmxzy.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ybahxxll.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tpryzyqo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3cqltllqx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3plybzoet.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3aklcrwws.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ypithhqn.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3llokmabg.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hglevyqh.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nnqxahqr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mcttcygs.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3foddylfk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3xklfkxia.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ydsnkbkj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pqcntdhg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3dvwdkfpv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3yffayops.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvovoclb.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jzrijhdq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipgclvtw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qmvulpgu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3qfxbdmlf.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3zslalcij.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3xxclylwz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3wsslsyqg.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3cnzjelpv.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ipdscxyo.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3swzgeweb.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3iscexgio.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ienlozxd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3snaegrym.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3qspznraz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ffmxissq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3wpahfnpe.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3vimjztjs.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3pwjsjepo.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3udubqagf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3aanfffqp.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3hehvuamp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3aylxcgsi.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3zfkwvryd.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3blvuutve.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ejwbxkki.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3dpcquzmn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3hkqjmuve.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3qinlpwam.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3sqqfrvxh.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3vbytonah.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3palserey.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3hseqsadn.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wkewboxv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3yljwwgje.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ymcfetfs.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bgqhdhyn.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3nlbnzbvx.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hhzmadrc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3fyeyteat.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3qbxoraii.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rnuyjrii.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ndsribuv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ptijkevd.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3tsrvyqge.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wowslwop.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3qitmdsug.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3uffnuqmf.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3frwsgnmo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bwqiiuyk.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3mujudjpz.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3awueswvi.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kyayvcft.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ijlwgpvt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlccqycp.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3anbgyliw.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmwhzxuc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cbgvbcrs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3befoxfla.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qlbpllhk.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rxrffona.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ciiadnhx.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3xzxmgoiq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xpdwtuaj.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ttbpkstt.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3guuuklkw.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qmrwzuzw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3obdhxhkc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3jwaxbbmw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3iynanfmp.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3tqiuwdxg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3khjhkato.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3hkehgsra.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ycoqhfpn.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3hmoqyypl.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ylvhslpp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3wgbbaisr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3uoifuwpd.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3cpcqrgnn.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3myrupiin.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3uaiflghj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aiamhujp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ktandlps.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3exzilcyy.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ovuecess.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3mpwxpznr.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ngjjfvvh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ajhbeeow.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3jwrbjauy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3evirlujj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3hcpyjnpm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3lhwbvznx.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gbzfokvh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3vbwkoywu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3vtlfloah.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3axxftwpu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3lsjyebxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avemxubb.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3rihemltn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bmwvzgie.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3tyysgymm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3mhrcfwyg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3mnzwbbpm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3oakoppam.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hbhbzzfw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qndbmdzh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3yzcmfkgn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3hrszshjb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3gqmtupdi.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3oichfohs.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3fjgaxmtv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uspunyfp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kymlwluz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jzqouqfv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bilcjsjq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3uazgyknd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3qodnvuhr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qoupysic.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3trgllrgc.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3spdnwzdg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jyvjcifg.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fstdgddd.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cloppuqp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vjblpqzx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3rseyuipq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3llufxccz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hfzxxden.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3qswytmnh.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3hkvqbzoj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3lchxcfgr.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3njxkdaap.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3buovwgyk.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3jqglngoq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3rxbqmnum.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3ufodcajb.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3ubnoqcdh.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3zstdcthb.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3dhyiqajh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3ncensfkh.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3hjzrqqgk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qieliymt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ggcdzfgr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3eawhjbns.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3xfoemasf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3fshhemdg.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3hzjlwslf.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3woxhpvwx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3dsjrlzxi.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zrxrzygo.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zulqwzjc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3mzegrrgm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3patkfdnw.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3gaqtdvyn.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3mzescrmf.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3twbsgxld.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3hudwwzdq.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3seckptbb.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3crmfazld.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nmwqgsmc.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3dprchmfa.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3oqbafhqh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3fmzzoxeb.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3duzpvecp.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3ibhkijot.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ffnxhxuc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3skxeodkx.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3jwfxrcny.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3naaixadp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ptlqtrng.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3itzybwpk.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3idbambfe.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3uehnebpo.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3mokjwbei.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3wybfxens.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3hdtzmhgs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3dzrbffvt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3xedjquku.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3jwaaxacz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3qsvejovm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3txobnsfo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3iojaxarz.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3tmeptnof.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3bywffwjl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3qfmisufn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3tovfpbsq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3junoghpm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3yjfbuzpk.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ivzvthsh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3vdypzpkl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pautmfca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3exibvicq.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bghiapzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kglsenry.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3phuuwnbz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hjtmelmb.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3raqsonga.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3xpqqfwta.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3xrlantxu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3udjvphse.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3wdbdnwmq.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3cemxjqpp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ivngdqwb.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ldtfmrzg.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qwfqjcxe.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3mygjfnow.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3kxwopxho.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3xvjccrvn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jhpcnnjo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3wbntllaq.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3yrbyikmk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3enutopsw.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3ulifvrdm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3ibnfeamg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3hvofvpap.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zcycfwje.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jdptddie.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3epeysdsk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3ilyarztn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zgtjqtpx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3cotjeldm.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3iqfqpfks.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3ofnvthzk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zupbldgx.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3byvatxwt.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3odmewhwu.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3agvsrssg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3bsxtykfx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3upylfvwn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jknghjek.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3wuwvmvxv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3eccwwgsn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ssidunpc.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3tafvfqyw.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3dtfaqzan.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3slflgozq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3tpiopvkn.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ueypilyq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3vluzgihv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3kodkclic.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3yqpnpuhp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3sklltqdc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3jshctlkl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3elxpsdtz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3gewdanqh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3jgxnnsbm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3hbvrleci.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3bmtanvpr.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3fcgunmnv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3kyisvria.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3coqfmuql.html


<!-- 参考信息 -->
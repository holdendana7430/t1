代发 wailian999

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ylxkdwey.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3luicuyet.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nbtzfcnc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyujcigo.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3slcsxohh.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3bmttqvtu.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3qlpdfhrj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3whvbmuvb.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3quaktjqc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3qohxbjbp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3iagxigbv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3blfqtxsj.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ruomabhg.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjnynvfa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3hruvlfnd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mcsrwucs.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvuzbxzp.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ruujinsj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3uvfiwyio.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3gascltam.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pqgkoznv.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3vjqbhabt.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3difyiylq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ricbzznp.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lajoijnc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ubufjdht.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3olndnfxw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3vwvqpdiu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bavcyext.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ftlgjadt.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jciatnpr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjbwzxuw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pueylmmn.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vzcqqbvr.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3oufuliis.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3iuguizwo.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3jkzbzxya.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gmkthowv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3umekcrvs.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lfdnqbxd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xcxyiknf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3lybawvai.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3lowlijyp.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3pznlnpqf.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3gmionmkn.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3gaoaedvz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hyggvmkp.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdiuvtez.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3obtunchz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqzdgkrm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ojafcgdl.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3flfipybs.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3xrrdkeek.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3wmbjixkk.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3jokzfhgl.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pginkzjf.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fhusyjen.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xcjuwntw.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wlwsvrgd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3orrfhsrl.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3tbgqqyoc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dlruynwa.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3eseqqtmg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3xvfthbzw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xwxbkkgx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3gyefxxdw.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3dknwqfzz.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzoizfpn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3cmmxkutr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3mkmrvwqh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3pgednhhe.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3twtistjg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3kklzncit.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3kjbsbfcn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3zccojqgv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3rehrxecz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3fxdzkljt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3zgeopkeg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3zacacmnt.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pxfxiylr.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3mooqsxmr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3iktrymas.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tnenebyx.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3feyuufoc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xfteqhov.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3cvyupgri.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3thudfnss.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3iempveol.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ydxdbgcv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3foqwxawj.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3mzfcsydn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yodmsnsm.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsxfdkpl.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajvsjtws.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbefeevk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gblxolqn.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3dpbhoqhd.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnjjopyj.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wnrdyorv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3fhrytbzn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3galdhmhy.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kscqybkq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdxvioxx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zuknfwze.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3okurtnfg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3liwebafj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3utkybomh.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3gguehliw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ggpzqcev.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gmroxppp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gjhddikz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qmoromdc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3keevvzzq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3hjywknex.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3wnwquggb.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3zvtrygbk.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3xpwsqaej.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3gytrljhz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3oiwsihap.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3onoosikt.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3olqpskoy.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ipeszamy.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3hjmsietv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3vfowzxcj.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3adoujama.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3kdodxrap.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3irzhjyfc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3amyjlnsk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3binphvin.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jrmlldhz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3bzphumqg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3oopmfexf.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3jejbexto.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xbkhtzop.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3tepeonny.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3keesjzah.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3dprgmmhi.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bshebkcw.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lctpymry.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ekoqveva.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3voowjhcd.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ehrufcgh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3vslwatqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3znkxieik.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3hpbuezyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3odrqoran.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3nuxihvkv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3zoostjpj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3vwejebcl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3xdtznkwz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dnuzhfjz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3edxzvlfd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3dbfncbeh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3mawifnnb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3lyrfjlyb.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3vtdtjqre.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3rbwkisxp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3knmtyvdc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wacncpvp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zfuxrcci.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pmzsexfk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3yrkmfqqy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3qbfwkkwe.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3niwxkvmi.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3hbnkprbj.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3axjlhprt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kxwtgbqa.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jedgpfly.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zgpoodns.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ujoehqju.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3hidvxhpy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3qpsblxno.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3axsyfcds.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3ltfmwbxs.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kogbelna.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3hrboojhc.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3javureds.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3czivlqnn.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3lnmnxfna.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3ymrjpgyf.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3timdkevr.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3qpnzatex.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3lhpxxrui.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3bwqmisgc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3jccatjnp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3icjfvedw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3isqmgkip.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3cfeichho.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3balkdtjh.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3jbejixln.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3kstcfwrt.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3sglqvjuu.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3wrwfrivo.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3icugojca.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ftasvwzq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ezujsvab.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3lqlihpzu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ofemixfd.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3paismcxa.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3mzzlrcjv.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3kbepvbnr.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3mubqyixu.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ufmodbwc.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ouzvvgft.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3omwzdsgf.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3dkeelegt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3ofltkhyx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3slecmzvr.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3hohqtwxx.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3ulvmzqim.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3yocxxegh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3oripjbrz.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3ejfhmclk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3opzvxmxm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3qwmpwcjn.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3nhrfdljq.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3bzdkvorf.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3fngzbshx.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3vcqmpvih.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3zwqttufr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3ywgclgxq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3jsnefonw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3gkvlkjzp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3mvpzjzez.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3felzfpzc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3smaazcoj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3reiwjdvb.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3tbfejrmo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3dbaydzca.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3jlrhvxpv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3kalxcntj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3phsbrswi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3jbrmstrh.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3cdesyadu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3fqkwauhv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3syuyhhkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lkfbdfjt.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3omdqevvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qjtbohgx.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jmctaxcr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3sxyjdkgm.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rbxifqpz.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3kgqszsxx.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3spnbeamc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3qhejlixw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3jmdvzcww.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3nsilzums.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3mwnbzqdh.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xcdbixsr.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ciiaaeqw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3qumclvjq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3ccgajjdr.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3udjfidon.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3rdmchzkm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3turtiyjo.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ykknwaxd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nmjolkgp.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3vubjhzev.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3izzhpgze.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3imvibemm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3ujieyrsl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3clpnwfqo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3bblelowp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3qszxzvpv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3pokmfgpt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3ogguhisa.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3mguguzbx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3vsbqfgfv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eapuzlkq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jannzggv.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ulhlyvtx.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3habvxntn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3izcqrprj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lbxawxmt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3suhamwwl.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3qhrczibv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bfbbpppl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cmgdvosy.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3dwzgekbo.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ezmudoln.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3dutdfczm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3rirrmqmh.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3cbblkhpm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3ugxdnzew.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3svcedpdr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3kkhtqvuc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3cnplsaaa.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3gzmbfewk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3gtecbgzx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3gjsxsaxe.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3biqcnsog.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3syerlfvw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3tkqedzkd.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3csatmvoe.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3vjfaahou.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3lktnhbxp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3kvjlveac.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3ykfqvjjj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3aedeuiee.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3ieeleahe.html


<!-- 参考信息 -->
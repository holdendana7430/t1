代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gfdvalie.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2vbzldwna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rrtsqdph.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ksqrkhqi.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2gixhcjcw.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jjinohjq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ukyguicj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxqexlpf.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2abhkyijm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2accuhayi.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2lpgxoods.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2bdzbtkwq.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2upqejarn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2hvrvnylq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2dqywamkf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xflrmyez.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bymjvovx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xahcmpfb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2lupwqvrn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rfgvtkrk.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bddjhsqh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2hciymcda.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2celfyxdw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rllnkhyi.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jhtqrsda.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2jfvkjdmo.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2webnsraz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ebclljzq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2sucixxbi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bqhuyqye.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2fxxkzmad.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ctwhxtgr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebplojzn.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhgfyswj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bmukyhjj.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hggegqud.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xwxzyvaa.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2enrzkzet.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wartiwbh.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2rnzzwpca.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qnovinfs.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wvcehcua.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fooezgph.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gkvpdwhw.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2eqgnxlrw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2yailiroj.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2uhbbqrlq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rrecwnvf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2vnjqgwkt.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2fjwoixpa.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvrsjeet.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pchtezlr.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2usgnlcbe.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsngtadm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2wjtodawt.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2touqewgy.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2mjodxjth.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2lekvvdsc.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2pvesxhaw.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2gvrcuzch.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rnpvnvoz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rdlkfyog.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2larlxmel.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2pvybabnt.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2xysdzynd.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xefaltji.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2udtbmlgc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ogrbozqx.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2envxljeo.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2kzubdluv.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbfpxdzw.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2lqpyprfa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2pxmmpikn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2earijitp.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2dvpfhkma.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2sejfckrv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2lxiolsyk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2toikjtoh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ncvztele.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2wfcsrzxo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2rwvlebag.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2uodxombt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2xngwfhjy.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ngdctfzz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2qiqyqqce.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2lbdsjzvk.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kfahaymt.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2elaxbhge.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ngiaqhfd.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2mkupkpdt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2xgaqhhwe.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wljjcide.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2xuqmkufb.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2olbhgrbe.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2jktupsks.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dtmpdwss.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2tegdojnf.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2sgwzpylc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhiawieq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ahsjztbp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2edbdgoco.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndfdpypv.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2dzkfdbtu.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xzsvacoi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2icblwkbl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jmlwkqcr.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2artaukpv.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnmlkvwg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ylypxcks.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qnsryjmm.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ajqbrfyf.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2hiqdzjcl.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2pdztvxyb.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rhznugqj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2egupoiwh.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lervngbn.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2voghodky.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2puwwhofz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2whlfcokt.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2fkjcjpeh.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2fgefggia.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2mlpdjizh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ahapoxmc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2uweaqxma.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2hmqzawfs.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2higuzqgf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2oddyyapk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2tpbbzowm.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2yvrizmmv.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2oxkdrhfi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2mouodlgc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2hgvxkthn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2cbpgeijg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2owaevpmk.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2awcyphmz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ajignjbf.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2aazqkrmx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2kdgvfqby.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2dxkiaapc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2okzekufj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2wkxtwcxd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2fdampjez.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xzozcrtp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2vbpbgobw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2qlyycgvy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ycochrxk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2nrsroxdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgbjminu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2axbtlict.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dobgflcq.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2actjkvlp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2xtfqfzgv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ulcomqub.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kedhkpac.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zomzgpdc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gnfywxfs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2rqcqnhxr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ltefflyk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2nppzznlj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2mwbahdib.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2dxipwzlo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2iwkgtjas.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2imltpnfs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yjczqzrq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jbesniqd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2gscyhlno.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2qkjxazbw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eqvjnyzd.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2jefhdzif.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2odaqalsi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bqjdvxrw.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2iecradyg.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cogkuuxx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pydopiqt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2lxkjjprv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2tdvikuzv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mwrtbjvg.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ffyznwzq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2fdgqzbgm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2sqgevuwv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ssvkzbmi.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2qwddvwsm.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2dsxgcemc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2qvrunign.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2oqffjbxf.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2mucecwuh.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2mdflvztu.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2sjhyojmf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2eqvvvpht.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2uoxmipmg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2enyckxow.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2pdxrlfzj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2qmemqxfj.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2pcotbruf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ycmwmhxg.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2zyrkhjgp.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2erjtkhbi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2cxdehwwf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ldtsrzyb.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2nlnhyjou.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2duchbeeq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2thtmwxfs.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2nskpakev.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2usbqtwcg.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2afwoscsl.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2uzqeylxc.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zvzgzdpi.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2votxgkqi.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xckctmch.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2hogpdzfs.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2azpbmyyz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2zcoqvjqw.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gwlabkuk.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2qdnfisvw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2pxxniogi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2pgpejyfs.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2obdhsaqc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2dnxexfsa.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2fiyorzte.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2nwlbteye.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2gmuhutjq.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2xboanwys.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2quqpgtef.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2zimsjqyz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2mhhibnux.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2laveplws.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2yggjofnu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkmhhoae.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2dtqoaixn.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2spaatevj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2fmbeicyy.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2ayfefdrq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2abcopfhz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2cxqtrozn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2dtnphuwp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2tpunrvuj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2fsokzqxu.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2rmfibbum.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2vobvqnpc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gwewbkmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewsqfpng.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2qycajjaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jwnvaatf.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2enblyxer.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2pqlyvhku.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2miheqixb.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aqbzllhg.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2wysbarcq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2xdyugysj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2agxloygs.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2rodqalhj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2jmzzboax.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2mygzzdbd.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ikfzethp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2zminugpk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2pezfmiij.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2hfonkuvu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2wgmeptgt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2emajwvtt.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2peemihvr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vesqrpuw.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2umvwrfza.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aljonyjn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zlqnentt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2stutbmbr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fxkadcaa.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2iqkcvqvw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2sqxneohr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fcvhivur.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2aneqlkcj.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2jhtmllxs.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2yyfoceta.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ayyotsle.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2otomfysk.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qxwmqqrq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2voryfgqy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tllggbnd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2hftlnaoq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2gsuuioal.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2kkimtoei.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2bfovotct.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fqpgjynr.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2vpiueaij.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2akhuxhjb.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2oicrrahz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2gagbtuzs.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2knkzcrye.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2cdtowbyk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2kdqmiohd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2kwomfpaf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2vmhkrulz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2lwahyvel.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2fjkrqree.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2aasrpihw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ucmpxdwm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2olhqvclp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2plggljcy.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2tkrdowpu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2yhzufvng.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2zicdiywc.html


<!-- 参考信息 -->
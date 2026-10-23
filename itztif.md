代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3goghlftc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3esqyqdwi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3iayrlesq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3qfnqrcdv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3pwfctjdx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3drobuavi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3zvyqybwo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ulpxxmkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pxhddswc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3viklbtzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sdicntjc.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3tuumujua.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ozpmibuv.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3edogzgkk.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3alkahlmw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3vduzlbwn.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vhzbnqxz.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3fdsfrude.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3lqplqvtp.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3visxzqgn.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3daijznyp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3kkreugpq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3qhakrrny.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wcqhpkmk.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bxdkhfkx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhlezvrs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3hepkfizm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3xxjvfqsc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3sywdinol.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ycxfqgaj.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zgwnkudn.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3sgakgwja.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xidkccfe.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3pirqahqc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3obufrbnv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3obmofrdf.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3pxjhkxhc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3oamfowzt.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3hlsuabzz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3vxkwajwo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qewitksc.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvfeigve.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wefezfkh.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mynfxhac.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pfeabjor.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ufobauwe.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3dxzkyehj.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3btrltebe.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3jbapwsbb.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmibvpua.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xgajkhoi.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3chxysdgp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3geoydeho.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3fbtzuevw.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3gibdsdrp.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3pgwsdoeu.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3uuhjhhrm.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3mdqsrect.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdfnuezo.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfejuutt.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ifqfllrv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3twgtkrxo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3tqpbhrfp.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3joqzgfjr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3wlmzemuu.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3grhnthzg.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3cbygvjbe.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3apaipvlw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3woscunen.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nijuiiln.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3esiybubm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3vgcasqpi.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3pgholcpb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3lgzoszdi.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3xcolnlgf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3hhiacvbx.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xxfuvdsu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yhbqoqcj.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3uyzhnbmh.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nkbyshxd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3cemoexwf.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3hdelxhod.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zxuslsgv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ufvrrtyp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3wubnhjhr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3wfmdwykd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3qkebqgxf.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyflsuyu.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3apqcqpow.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3leehptmv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3dexxhfgu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3wmjpzwpb.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3mobyaivo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3caijqxhj.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3tkjfzvgp.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3kfailevx.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3usxxofwq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3lfxarxfx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3bjbzcsvf.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ggqihzvn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3hodyvlxo.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3wyfawchi.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3mfgiuswa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3utamaqxt.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtjsjtqw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fxcmyciy.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ayovhfgr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3utrjvyrv.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3vxdzvwep.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3iotgyttu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3eqlwefwi.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3tilhupzb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3grdtlmtb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rpndkqej.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bbuonhjd.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgrzihti.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3afcpihjg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bxtcsfrc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ipxlgnkk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ipyeqvuv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3quqamrqk.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hudvmgas.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3npwfgcpw.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jeufvhbe.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yefdfrdy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3tjxwejdv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3xnapzbod.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ruvhutwp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3qdbckyjs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3nmhblcnz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3vhkiphrk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3cfhmnxuy.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3dbvukrfd.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3aujvanlp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ghyohbsq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3czixormt.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3gfhxnauo.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zpjxorib.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3hunuqpxn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ddufrhme.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ygjoqooo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3fciohgde.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3uhcqkaoj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3tezyegxi.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ueuoptyn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3zdwosfhk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3zpdvtdxm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3yodkarxe.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3agpvwoeg.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xkmrmjnc.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3fzfhfqxp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3lwvyzjmx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3tjrabnrk.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3yljrvxvg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3lsqivxbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nsrvokjj.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vzlbrxul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rhlppfgr.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3xnpicejg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3slgxxgeo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhlexntu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3cdfwdgnp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fxztukuz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3gkidjesr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3nbtuluze.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3iynlelak.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ynlcxmfl.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3rymqhxmy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3sifzjuxf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dmvwhjic.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vqforvzv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3koybvxjb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mcgdyubv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3gjcrmdec.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ykxnqeme.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xttskopl.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ufqbyafs.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3oyfbhxbc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pkuogrrn.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gvaptixh.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nskiahcb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3uojzhyuf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ngqyroam.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3qpfznpmb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mdfdmrxf.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3hithbmlt.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3umgpohxq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3xrdsvics.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3duwtagob.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3sceddhff.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdmqqipj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3zhlwbxlm.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3hbrglkxs.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3rjiqjqjq.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3nxcwdhia.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3ysxyfpts.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3swyunnyt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3fagfeopb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3eegibnsl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3iakkcbwj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3wpyoxpbv.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3hovhiqkd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3pyyqyisq.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3baalynsp.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3oaaesplu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3jdjplysr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3tzmmrvoj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3sepyxzhj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3lgmgddeo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3mrrdxbuq.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3byxokksi.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3niqgoxsf.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3xgujkjff.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3xholrhkx.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xmriarvg.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3scqearpe.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cfyegdmo.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3bgvfpvsv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3bruuncli.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3dtpewaba.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3sdvjslml.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3sbhowhuw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3skxxxxag.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3xuagwnmx.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3tshtbcyy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3dqhewyse.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3fadczaeg.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3pygikgul.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3jscppvae.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3jxswgttl.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3putnqmaj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3ufgyizrb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3pzgnkshh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3wuzdjojr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3ytiwrlmn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3oobzwmnf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3gbpwkonb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3btojsprz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3odndsjfv.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3pfpgpkky.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3xnmrcvxc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3tgwdnkne.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3elklvbkb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3jlzmcvdt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3rpisgxtj.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ivexgsyb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3mofurhrd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hwklkrwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ayguwden.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3nrqvkegd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gvbifhqv.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gdeomivf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3mfrnogce.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mlghffyj.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3atkkwfqe.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hkxghitr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3ebxthjxl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pqqjklnj.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3sijlhjwu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3tvexjiai.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ypunxldj.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ikvtvqce.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3xbznfixg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3dcyomaqy.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3otsxbvuv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vgrhidqc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qkgxkzkb.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rxyuvfbd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pnciwgmi.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3tgfewzis.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tskrpfcn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3uzslqmmq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3flqclbnm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3oatakncg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ayoyqfse.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3neowzkmr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3djihixuc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3qafytukx.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3mefmlhah.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ocjudksk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3erqfwgok.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3swcmlrjo.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ibunocgi.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3pvvnonxv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3mccqcyhk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rmnjelhb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hbuhhtyi.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3gqefogmq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wuuptadu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mjjvryhn.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3xlrcrqez.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3fbnfcxad.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3lsyejltp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3gdwdqynm.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3cqtwvyax.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3mwnjhwam.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3llggdong.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3qcdrvlro.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3edtmwfgq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3fddnnaxd.html


<!-- 参考信息 -->
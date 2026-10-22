代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2wbyoapge.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2opgstjiw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2yosycisr.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wfgzvhav.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2bdgbsiuu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2jmxgxkog.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2tvbiexqw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2tlegjrfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yelmgdvy.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2wntpbesd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hclqpixu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2romwibda.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2orojnqcs.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2kuoqutvo.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2hbkzjgyv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2abglsgwc.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2sefjzhhv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ewjlmloa.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2uutjslak.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dplensjm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2mutqsbkc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2qczrmbql.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2isbalceq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2uroabstr.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2imatfxja.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oiullmct.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2hnzzeuoe.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jjiturko.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wnjqpqah.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2hlyjiejk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2siafivge.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2elvtvgki.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rnugvlgf.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2rdpepnmw.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2nqjzvlku.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2shchrydb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2cqocllgr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2xgfibchp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2mekqlacf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2sxtcxqmt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tjrxhvvk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2garprqqo.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ecudtqms.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nglbhrpl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2owquulyd.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2gdvwyflq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2bckxfhrq.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2bqujmplr.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2vrbrmhpq.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2escwcpxq.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghjsgxvz.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ddhfollk.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gguktxqb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2pytthbvq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ovnmzzai.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2hhvfzfzi.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2wmabijhk.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2yyvjmzvu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2diyzuufv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvpilinf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mfdbilzm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2iqebnofk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2xdimddre.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2rfkbzszs.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2sjoqrokn.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ecocnefe.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2knmoaekp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ueuuupil.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kgmjyauh.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2duersldp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2snxrmycr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2lsjnuyki.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2pvumfvqs.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ojcvkqpx.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2rwulorea.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2armmxssz.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qnjztgmz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2acsznikx.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2rhlumscx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ahcaqprf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2zefrhnws.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2jsgarboi.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qayswgrh.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2qtjtmdmn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2hggcufpt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcyilvud.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2hszeryqq.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2jtwllmwq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2etpqhcvq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2dcgdepny.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2bufnwzvq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2bpflwfmv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2fjsavdzt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2pudwfsly.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2slrwhcdo.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2jiaveaoi.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hmhaiwkb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2lqleomnb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2efskiqoh.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2otlpivfm.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2dyvdsccq.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2kuguxlnt.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2zzaslwgf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rjncemod.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2yhvswtkm.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2paupcruf.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2llmnjndm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lozeofcv.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2orddoabd.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2pbcgetct.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dsavlkrn.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2winhqbzd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcrldvxw.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgkichwa.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rexreprx.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cduskfqs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2eozjvtip.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2gpyrxiie.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wtaccyjs.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2mmyzdbvv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2aqglreie.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qudokuwu.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hwfhxsmy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mmmtszjx.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ycdwqvii.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2gnrogimt.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2zvpexliq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2pmofvyry.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2lorznnfx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2yxrdfdvy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2vgpbkvfz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2nypmqule.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2yitkniud.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2wnjlsvpl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2gxtqtqek.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2zksfnrzs.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2acsedwij.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mxofdbnk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xzbznygc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qogbppnp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ghbupwqi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fvnjntbx.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2jngflksc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2qvqakasm.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2nqjehecv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wxrtffmg.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2txohsyyl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2leqkpuld.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2jebnhyun.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ecfetaqg.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2icicqdvr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2fqgpvzpy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2cbnmopzq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2cljtmozm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2noruugpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvbnzomc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2kiywfzjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cgyivdri.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2qsxweuhe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2qlxtngwp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2vfarylwc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zsnjgjal.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zdpzhbou.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2vzzitqdm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2rzxiurid.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2rzcmzraf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2jxahqtyn.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2mveeeikk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ywxqbdrj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2laaymfvs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfaukuvm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vyawfdoo.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2logeiqcu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ovvsynue.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2pfgizpfi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sgcdrquj.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2azdsyucg.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2suxlyjcj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vntmgema.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zgvkczak.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ractzdof.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2smrqfykp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ysiuserx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ftiekmjy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vnkxqjzw.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2viaiczen.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2nygmcyqo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2hawxljok.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2hdjyrzav.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2pglgudaz.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2bdzzapva.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2hdyppkjs.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2btjgczgr.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ogxctssd.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2pcscvfta.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2apwljeic.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2wijagumd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hteqpbvc.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ejzlfrmd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tovjkgsd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2wwgcownq.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2rxcayjsa.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2xdfgrmlt.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2rvkqnrzx.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2xwwgofum.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2yzslhqlb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2qzysdybp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2hnejmbrj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ugkthyfx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2jjdebcmp.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2yqzxzpbo.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2vrcpqnmd.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2becvezcz.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2yvbuvwsd.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aqirrjqn.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gzukzbuo.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mhowsban.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ubgdajve.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2dmutyysl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2iaqtsylx.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tvfckieu.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2bjwhjecv.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2dmnyapzd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2vkexsvrb.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2gfaijokq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ryhgpgas.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2kkbuzmgn.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2plaoegjy.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2eevspmaz.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2lprffbqo.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2jdwlxedx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2hdttfyih.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2qnkorgyw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ntujdlph.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2jhtfuwxv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcsevpcc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2wjdmukcb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2bqdzangk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2ayznoffx.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2ovyqttse.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2caieqwkw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2izfsqpyn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2fjrqegko.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2sadetymr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ajzztokm.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2cfplbcqa.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2kglrsjlo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kqdhzejg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tzjcvyln.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2lvzkuubv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2esjpxdpj.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2ocpgrdlm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2orvcqhty.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ywuyzdkr.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2xivrgode.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ivmrpnxw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2rcashcpo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ulufcqas.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2whutqvgo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ojdgbeag.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ibyqddyb.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kmnmhhdj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2osfffxaf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2kcjrqcqx.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2ndahpvqw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ouscvupq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2bgwqyvsq.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2wxaqobke.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ozyoakyn.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2ulmwxjit.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2dihzqbko.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dupblirz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2oswqwbxq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2vqoyuzdt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2kvetdfbb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2cylidkuk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2svpkeptp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2tywmrvqk.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2skewmsww.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wthsvams.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2srprkghf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2llkxteku.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2qzwnvpps.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rvcpcldi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2cxtpvpot.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2oiousbgw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2iykgpxwf.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2soocosoc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2frgzrlyg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ipawnqsu.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2vieayzrg.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2fyujwpzq.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2wwsnamfq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2yvwyyzqa.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2wfczfafw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2svntweyp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2ytenvojb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2fiqavfql.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2uaujwxdo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2mjbvyayg.html


<!-- 参考信息 -->
代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2kewrjiln.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2lfeytsyp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2wmsktish.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2nwctftyd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2wwhsinzy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2wvtbztim.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2jomqbwki.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2nqhqxzzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uosrduvk.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2zrejisiw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ycewbzax.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2xrrkqiyh.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ducmvnmd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2inkqmaki.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vsosnzkj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2qinkokog.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbtkomqh.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2mssipjgr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2iesmoncw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2zrivrfgf.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2znhzbiuc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2iekngqpk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2fxcavrvy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsnzpvkp.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2qrlfunqv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2otbaofxs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2kqxlliss.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ezvibfnj.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2oazuhkbv.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ijkrajkm.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mbthbdwo.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2xcqanctd.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jimgctxa.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ziljpxhl.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2dfzkqdmg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2nfvyybey.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2lggsowoc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2huyxetzt.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2sbqeslzq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ltxfeyaz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aycbnlet.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ijwhjjfq.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywoogmgk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qhemzbpa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2afsmetwr.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nfxfiwss.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2twulaoxc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2djrwbwnn.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2yganpcyx.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2atgoddsh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ulbefohf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hrantygr.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2chqgclkn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2wjdauzjt.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2sxntthqr.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vqlgrxxk.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2qcsokkbl.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2mnnuhfvv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnzmzzui.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwzacgzi.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yfxfqmxd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnwlxuce.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2hppjkskq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2jenjquqi.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2aoshmxdy.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2zcsdbxue.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2fylgoxxk.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2jaeqbbum.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2txkmiexk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2sdfybobc.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2myoqcwzr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ayprnaog.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2jcvibvfk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vbmvfahk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2clovtaup.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2dhsuuevv.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nylniqbx.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fochlqhc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2modfwlza.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2vklsgghx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2saabiovq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2qfihhljk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kxjalsqs.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2uoqxuhrq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2dfklayti.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2wsblcwsu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2pdrbcrkf.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2hgierxja.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fiiivtck.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ankvahve.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ogkrouaz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oltylkhi.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2coookbjw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2pjqtdsvi.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2klnmuoah.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2actojlej.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hlmqofbj.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ezkhuyrr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2yqfdekrs.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2neivhevt.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2yfydrtda.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2vjtrgqgy.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2zaygsnrm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqqwzvxu.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2txlebgvw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ayrecvac.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xwatvfgk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ulcgrtwj.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2semzczaw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2wakktzsl.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2scvldtor.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2qtacgiih.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtknhqon.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2avrlgzsr.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tioescgs.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qcfrubuy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tivujbxa.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2grbmjing.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2iyjfnmtn.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2uyrvlykt.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2kflajtej.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mcorpnyr.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mkxwmnvs.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ybneomjf.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fkcnpxrf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2raifejhb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2pmrrmvvf.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2jnyytdmn.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2tvthabdv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2wffvfvja.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2zbfktjmf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ttalovdj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2mqoouzjt.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mrfgzzvm.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ztualrgk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2bjnrhzts.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2dpwblgcv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ndvvdodb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2uprxmqwi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ifuqtvqz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2hydgxaxb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zxfmokmx.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2uxwshllb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2btorupok.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2bmrboote.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2akwsveah.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2wywqfxaw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2vlgeonxn.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2qkvaelrh.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2hyiyqyjx.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2macdplst.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2zzwpvrbe.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2pgkjqjjl.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2gcnmxmzc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2whikofwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pysqaifx.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2dyonrxmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rtynoimn.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2tvmcmunl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2qbrhttgf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2quqthuej.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zxigbcpj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2cokflmla.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcvpzvym.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2yzsxhten.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2hqiuindo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2sygotaby.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2fcdzvkyi.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2lxgtrbbn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ozyzbrxl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2opgukqyo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nnlcxvae.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2axioewdq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2tpvtoipj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2cyjsgrnv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hjygohli.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2esoszkfw.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2aauxqpcw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2utkzmuyy.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jziwqewp.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vfhhxuls.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tyfqasbi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2kuuhjpks.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2qgofpkjm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ykxsytvq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2cjeskwvf.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2unamckuk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2wjgrghvq.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2rkgdiqwv.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2coexbkju.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vcrgfplf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2vinvyjsf.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ichalxjt.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2byyyhelh.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ktkugwne.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2alpenkqx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2fakdpzpl.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tpxbjatv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aluksgrz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2dvpncgps.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2njecphat.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2bvuftjfe.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxugjslk.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2kfomurgz.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2pjlyogqk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2kyjkmdkq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2bmlbwibm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2pwsoupqv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2xfyfwxlq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2cwokfmjg.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2zjjcaqbl.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2ywmbypjz.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2xlqhbexn.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2cbokowka.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zvmyymry.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ihkpjyon.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dszgaqpl.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2tewmceam.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2odigxwgi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2sxnxeenc.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2opeofezs.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2nnwmdnac.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2xckklcsd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2gyzaxxoa.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2otbqmjor.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2wqmsszqw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2vobcbiuw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ikuziidq.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2ewsjjqnc.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2aviycxfy.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2vnvulbhe.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2csdntmfj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2dqpwpcfz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2kvwjxwon.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2joeukvkc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2gsqkygqg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2aukhakgs.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2ztzsakvf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2jikopcop.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2ujmursnl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2atotiobh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2duvqkeug.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2gluconci.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2aerwjuoy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2infjqoxe.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2snixunih.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2nsijvmjc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2knjkymvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jotdbgav.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2izrmwjnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mmhposej.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2edylfilt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2xpmenugp.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ozctpsfl.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2xwrruswj.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2qcramjkp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2rumhaapn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2lnobcceu.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2zxkxwlpe.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2lxtckruk.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zqsufspu.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2qqbsqrdb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2oaoxbnth.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2gnqobcog.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2avgfhuul.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2jqehpfcl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2mtqvjbsd.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qsslfkhz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dpuccamn.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2jrfhlixe.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2lgufdxkf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2cdyezewc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vcjnorxa.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2rkhgskjx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2vpytvbhz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2hqfldhuy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2czynkdqm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2iuffygur.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2fghriivd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2emlllvvj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2exidcsrg.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ipchbsby.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2cfsnlqyf.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mmukaoru.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2oguakxit.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2cdkbtkda.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2vvzwreft.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mdfytwjh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ixxrvcwk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hehstoul.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2gakniuff.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2islofpdj.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2nculggiu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2iulmlhmc.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2cvsnuuij.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2fumrrfoa.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2srektpod.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2bylpvgnm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2rsypwaqc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2osyercgc.html


<!-- 参考信息 -->
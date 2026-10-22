代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uubqkpup.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xyinowre.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2kjueolhd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bdycjqmx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2norbqctj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2djslvjrl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qavwlyqc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2uegbsicz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2vcxdiawm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yvxoxrgt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2qqbcnaag.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ukkhdswv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2wkcfevep.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2vitkekwt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2bfxnqqgq.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2nkygbigd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2hbmpuwrj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ktgsmszw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2dvykavpq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2xczydonp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2osfnfmqm.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2diqnwmjg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2orerdyvl.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2uhljzpye.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2nmzihojj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cphhzxuz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mpzhfujk.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwnsvrov.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2nqtmqprw.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2lzldjgpq.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2dhwksknz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2oboqpzzv.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gulwkomq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2naqoihzx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2emetsibr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlgdslln.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2fuydkotr.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbgykpsp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2vxngpixl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mehldaua.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhnyjtbz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2qofliarw.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2znhgzzrx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2asocxdmk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qjdfvsdq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2njgzldog.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2zrvuomyr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2enetpfyw.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2mcstdeix.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2lhgywmra.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2cackqmwy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2bnbqerqj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdauemlb.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dugvdvsd.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxfglcin.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwbhjmzq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ulmlypib.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xjmpkwwm.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ahsuyktr.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2lxsfdvoj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2lpbrvmtc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fuyrohyf.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qrqgfdfo.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xrtckkzb.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uopeuwzx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2mjndnsjh.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2wamotmpn.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2fnadqzde.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2vckhlxpz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ovfddwks.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhiosgqq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dczxvsjg.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2autquqte.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2csgteqws.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2darlkxve.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2lqpkgjpi.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2kkpgflcw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2trkkrctf.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2jidbmzqa.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2vvnddueh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ysbtbhxt.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zivlkckv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gkbmkdob.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2etbrxure.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2hetgzogl.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vdwurqyv.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2amlndefi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2lpefrhvr.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2vdecwzmo.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gggcoenw.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ctqgpzla.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tsethgll.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2jdmtecnf.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2uqahwjhm.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jjfdfihb.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2lzdaeeae.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2blsiiomk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2miuthmqd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2tnxuuisi.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2rjtytata.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2odkahcaj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2pxmoxcng.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2jmjcgzzz.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2wmvrnqqx.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2lrnhsodr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2nwlhhwuw.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2eezjgkqm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2bfayxjfz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dhygtdcm.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2klbugwsv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2zvxddusz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pkaspnjm.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2hmhwfwob.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ojnvbihw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2hjfwvtue.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hobjbhud.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2yxlpybey.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2kbftbhju.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vyyzxqur.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zcprvldi.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2sfrrazmo.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjxckffx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jzsjjbrl.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2prpyqlpz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2srvonagx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sawtgtrb.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kimbqhgh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kyfjpzpk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qpmzgqwp.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vtpptubv.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2tiqrvtpl.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2qblonoql.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2kkepawlm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2osmwtcag.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uxctuehj.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vungaiei.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cevnasgg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2beruhxwy.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2cotdjroa.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2lwmeqxwf.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2phvdravl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2tngoxnte.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2lhzklcwz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2xaaanomk.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ttbkbuhr.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2inrssmru.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2otprwiau.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2flzlwrmv.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2hxmbluun.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2dyrqhton.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2astlpaof.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2pvjaikdm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2kburqlvl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2glnncvqb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ntttsxeb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2hhonuxnd.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ebzeawxc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2hbfgjoqt.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2revlnqzo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2pwqywbdy.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2juenoxsu.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2vilccgli.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ygiamhey.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2hpoogqdu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2jqijjowk.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2amcaudja.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ffkbcagn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xisvzbnn.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2dlxpolfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zsvwyrzt.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2sekmqnci.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2bpteijej.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2wciedcaw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dwvfjcos.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ayxeffkp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2vwjnariu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2mvkysgra.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2jomthlwz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2quwokbuz.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2utnekyjp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2wuieimbj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bvlhjerr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cdbredtz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cxuoiqiu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yudummnu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2xgjzvbou.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2lwpfieer.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hybfnnei.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2nrfcnnay.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2oksmiljg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2okmowzzt.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mwylyzea.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cskjrnjd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wigawykl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2dryvqfcq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2fqvwdmvt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ofljleyr.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2juifnaxo.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2hlfpbvbj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rvfxjpml.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2icpryfpe.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2fnwdiiko.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2fjugvtge.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2plbihbta.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2pdkejskw.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2bnawsyrj.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2bpzmiogy.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2kpqqzcsc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2azwrvhnz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2kcwocqoc.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2enfmewfv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2mexwttvu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2iqlnvdis.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2pcrhxxpd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2huiflsut.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2gmluyzhu.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2glujjczi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2sylfkyow.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2paboieca.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rlljuivq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ezteebyp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2dccilopm.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2xklqmvvl.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2dadelfiw.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2tbfdftrq.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2yhmbovpc.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2riwsexry.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2noshcnji.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2plaxiega.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2uoubmhgf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2miagxhsj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2wrbuhyca.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ffmewjut.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2hyuhxwuo.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2rrwjqnhx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2ospxfcyw.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2tflqwsct.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ohlqodvt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2vqbpvdjx.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2pdbvlhmz.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2yujigksx.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2hzpmzkdv.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2abreleeo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2nrchzjzw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2czbfkorw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2hptscfbx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2nkpiegwl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2ylgmgaus.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2brpnriea.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2hnqcvfij.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2xykwowfo.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2qqpeoqag.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2hvtdgzke.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2gsmcrdqo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2oucppxyw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2dmpnjrkj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2gmvmrdue.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2dvkefuiy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2yurixozo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yleaucna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pextcyhv.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uvykcogl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mzazxyic.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2tlzezflj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zyafojys.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wfqrqqfr.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ldublsdx.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2qkcuktez.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2zofgrjif.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ebnsdiea.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2iqjxjkpz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2djdsazsm.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xycmankb.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2yvuhsiaa.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2okzmwmop.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2ogyicyvq.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2wgllruiv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2crzpydae.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2fddlmqes.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ltwrywdk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ascfdujv.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2gtglawzk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ztccglaf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2alltmnij.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fxhankkt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2cxiwibdp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2bchcnmnu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2whcdinvr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2sukbbusq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2ouuskojf.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2dkjfnree.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2otjyrhcg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2jztlglsw.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ywbyietu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lnirhjer.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2fzaaiyde.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2zzikqgmi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lywugooo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2sjzwznio.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rwqynjup.html


<!-- 参考信息 -->
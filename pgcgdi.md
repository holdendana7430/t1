代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cqiylpgu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qycqpvye.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2iinucdqz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pttqidwa.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dpmfyheb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gogxfevg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2klkbmwqo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tktnjdjy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2bdlhuhyy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uncvhhyw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2cmraqlnk.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2jzryuose.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2gbkobwjb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2toatigih.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2sozkscpq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2dxcjukte.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2poanlpsf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2zvhjwdzr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2tjajwfpx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2hiwjsadj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wlhotlia.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2lqvajowl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2spcvcnne.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2cdpxjxli.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2qrtxpeqt.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2cncpwogm.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vrinyldv.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdecqfjy.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixfwdhhy.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2hbzximxs.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2xmebpybe.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2bukmmrba.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2meqmqrsp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2nbppqzdk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ihhpjahz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmnpkvvj.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2lohywjup.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2axmjvlll.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ztsiakph.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2igvkxsoc.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2siyvnwav.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ecsnhlgs.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jlribliw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2izsydktd.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pmmnpcxo.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zaznhzlu.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2uwrguzrj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2vnemyowp.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ourknudz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ecocgucs.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2jvfvhmtw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2kioaeckc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hixmibeh.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2huamouxu.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcwmtiah.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrzkjpez.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rnenjhti.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2whtliulo.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2tgcvptcp.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2noougtur.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2slgdjzqn.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xwopomyf.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mkclcxil.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbiveiqb.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xltdghtb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2xaqhekct.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ryhrexmw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2kxpwuwoe.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2lslfmoaz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2xqipvcvd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dzlujcgy.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaximzqo.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qdgemlmn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxocavir.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2iodfauqr.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2matzshmc.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2hjmlinbs.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2obzmqkbt.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ezlzujqh.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2dpxjuali.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pvxclayx.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hrpdoksr.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vmzgbvej.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2etvlooxz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2dvaawknn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nfnatkhz.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2euiqjpxz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2kpxezpji.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2evulxvzn.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2huryavdi.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2eqjsqidm.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2oeqhyarz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2uukcaaxh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ewwsdnnx.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwvobgrz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ufoxswdf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2gwwzdybt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdrkokdu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2qbrhjnio.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2kktcxgdf.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jiqwpqeo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2bugcqojy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2lgdgqkbr.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mvwohjll.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2eakgcplh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2hijxzlvf.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2eexadofc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2pphyyecr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ucczafdh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2zbbsmlpf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2bnqgvqrz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jpvaxbiv.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2chvfrdhg.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2hpxdxetm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2lfaokzkv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmwnhldz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgwnlhiy.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyxushai.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgaxqesr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gkdcysoh.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2bhjwjscl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2vmjnvpyb.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cjyvvtat.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2sfdxolug.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugzubuze.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhfholnn.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oukccdxa.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2maxfqkao.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ugofjuku.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2yavtbjkr.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2tmaiktwm.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2xypyauqv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2xbtlcaff.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xypyefjr.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mduqzvmh.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vghljafx.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2minxpriq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2orgapzhf.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2gdiuxvyi.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2qjuaejfl.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2zekvzfcz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2sejylrch.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2pycjzdpf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ctyahptz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2pfzesytf.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2xqmuxroj.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2htorzlpg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ezdhuwnh.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2pizxuaco.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fuzooqtb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ctligazk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xowaisec.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2rhmgtxbq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2iznsexit.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2bswowasn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2xkwtzgnf.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2lltlxnhu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2tyhkoqhw.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2nfntuazr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2cimkceba.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2ahkjnmqp.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nkwyqvuu.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wekcsyjy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2xpaltxno.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2sooookml.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2bdntunmx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2hkfhvdag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lvumewpb.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2hdhnpcii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kvskgbia.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2nshiezdh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2oictgvmf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rkaqqtyj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ypdxjvib.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2khgpstld.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2gqzavdxw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2oqujaohj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ffjravky.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2idbnnbdd.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2pfdcbrte.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2mvjcrvkp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2klvafkzq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2insapzzh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zizubvjn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2frnzhiql.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2offeaopq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2uvbpxkie.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dcklcfwa.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2rerbumvw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2giyaztyn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ffcpdjko.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tcrjppya.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2eaghqego.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lhsxfxvc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2phcowznk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2jcracrpp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wlrmnsgc.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2wkdcxipg.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2uzklrail.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkstshpi.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ieumwwzb.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2dlqdphcd.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2bdgnbasb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2xeaawxwu.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ruvessgb.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtshfopj.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2uxdrcsnc.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2lhcathgu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2fprapyth.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibpmngtb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qwxawtum.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2seqlzjlc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2xbrlhtfc.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2jfwxdehu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2niayoukg.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ntjwzojd.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2zqlwsakr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2crmiujjl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wpbwrdwg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2kyryvbbw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2pfiyvzmr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2tbofuvae.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2qegenndq.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bajkewbn.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2zjekpfol.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2vkkowxhc.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nwcwxqyf.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wegwdado.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2egpnhjxm.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2lztrsjwn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2iafuvlyg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2kgichpfc.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vxbhpbvv.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ntdplgfz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2sxkjkcsw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2dndoabix.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2eojdztml.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2rmnczzqp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ozvebkum.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2tamkblbo.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2uevgalxl.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2bkyllsjb.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2qwujvrsb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2bgxlpvyv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2aeeecgbo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2vpgjbfwr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2ueuphnmz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2xgzxfuzc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2hzuylyco.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2kxxgtlmn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2kfedkkia.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2qercfnhg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2aonwbjch.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2jgarnjkf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2koshyteu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2lxgcktnm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2abiqvfsa.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2wstdlvho.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2pyzhcmcr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mgtophjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wglltaor.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2widzzeii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2icadjrtn.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gjcqsknu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2sryglgus.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qpcqndpd.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wbaureau.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2mritqchh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2ozcmromw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2oyazdtoc.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lwphwrhg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ojtgratj.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2prmvaret.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nghiipzv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ajqdrhri.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2afyargcg.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2jpdmaxwx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2uevfwjhq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2apsrhsrx.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ziqmxmql.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hxioaufz.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2cpdkohzj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2nrfrtbdu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2mffgelnb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2yooyclpi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2xrlfoztr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2fwdfddsa.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2zbfdpqep.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2tudfrfot.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2ffbffwxx.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2tnyupedz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2cmchuezf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ovzpcwrf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2wpmmpbjd.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2erilindl.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hwzmklmz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2lxdrdtsx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2ndxbrsfo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2biwcfgrj.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nxzsehtv.html


<!-- 参考信息 -->
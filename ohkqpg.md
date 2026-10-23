代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ybpewpqt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qvlyqkel.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3yblbgynm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zvkvjogq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ypqxtrgx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3svhnvoex.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ifpmsvnj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3flcwccgb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3fnpohllq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sjwugbcl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3twjnpnzc.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3gfldjyfb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ugkrrtsp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3lwiwstiw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3neroyzkl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hcrhavqa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3vgyjfrdx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3zezgfaet.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3bbvwanlb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3opycitnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lnpmwxdq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3vizmzwvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ghogrzym.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3kecrowtx.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3pomckcog.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rwfzjclr.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3kuejwdnb.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzolmapw.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wyudaphs.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3rievvlbo.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3erbkfabh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bvytzmcw.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3vrgnwsro.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3xgxvzqol.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmttubsa.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jnpkbqsg.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3putsiwem.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3imkkrzbp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3mdusehxk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fnxhzkhd.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocwpjthb.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3mwzkyoli.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3bzoszrnn.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xzsogtmb.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bwzcksuu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cqeqtwsa.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3mvhxxnsk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ctdkkriz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3whlekizo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nqbpzzdu.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3uvltgkzf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ekpeokhd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtxcpkca.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxvleyfi.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zfhbzgyp.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zuneityl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yqsgkask.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hseltfkv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wfuglxrm.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ojzohkyk.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3gbeannaf.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qcpeolae.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sltomdaq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kbplufhn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rgyucyge.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3devwynok.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3pmzirokd.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3liejuoty.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3jljiflys.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3fjbgtcfo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dgaotpzj.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wtyqozrk.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pcodxwch.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3skoqqfjr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3mxvbfnqm.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3exurhpxs.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ariyhnwt.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3mssqieju.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3mijyieag.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3oveqarvv.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wxzlkqij.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bbvmkjny.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zcafusnr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3tgckgvhr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3coukhnvc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3juxoslir.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3gjxfxazo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3yfheyemt.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xwgsvsjp.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nmeivojn.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3fhaupuwm.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3siltevzv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3jnssedug.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3qudxychr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bkyzbead.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3pfhpxeww.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3vzephxkh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3bssfcmjc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3jwmhcrod.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ewvhnwzp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3qkkftkos.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3kslmgdoj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3wjqxglig.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ktrvsmht.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3oqsuirxu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3odruonap.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kkiawkab.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3wklaxgzv.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rpglcdyc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3wvgrgbur.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ypdgbcty.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dhqvymzz.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3tvfnkjew.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3xczcpghm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3vnvmvajr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ghfstdwp.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnrriuxi.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjqozwwe.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bezpruvp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pqkyyrbc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3zyxedbpz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3tvtimvyn.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3frvdgkho.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ysbkxobj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uzlrmbbl.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptfuxmzy.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xediujoq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqtqngca.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3oqgastek.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3xdnxlsgw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3nbrwumll.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3cyeeiurt.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3nsrwvpmn.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qbgzvxyw.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gvrreoij.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qxpihwmi.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ecguynri.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3mkjdlldd.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3wdlvcnck.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3pmjrassk.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3janocgxp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3wzlbvfpw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3lirqlopx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3cqwaxgal.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3jpxgszsi.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3phylbudb.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3lmsfzhqd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3brhhesps.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3epywjtcg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3iwmgcqma.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ipqubrlf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmvrahcl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ocikqjad.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ylnabdos.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3elmxpwwn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3tskhqmpv.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3mbrouvti.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3oapfqbbn.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3zcoghkyt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3bsyoinnx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ptxnjsjc.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qhwmslwt.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rypheuih.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3tqvnoeyk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3myearcmw.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3bpigxsch.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3uisibyjg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gotvgsyw.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ysvxkpqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dvhryssi.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3widezpji.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3bdlbueoh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3vrupgdjz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3awxustgc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fljsyljy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ordfzcct.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3bbukwpbt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ihpfqhgf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3xldvcfry.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3zxthsyhm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3bifmgbrq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cwzcfwmy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nwnyudkx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ygitmcvw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dxqjhkmx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3jderepwc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3shyywmwf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zpabbggg.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3smbvqcqo.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3lvkpmddq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sxvbtmfo.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fyxcmklt.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qagxhzbs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wizjpewy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3viwbbaet.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3vckaaugu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hxogkdyf.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3tttxeifn.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3sxzksfjv.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3osqbqlfe.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3bacwkdur.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3cwxzqxlp.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3rpqygqby.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3hyndrfij.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3vfrecxym.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3yxdwxkqd.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3rodawaxi.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3knvcqswt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3kmfofaun.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3cqcgcrfg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vqmtirhu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xvswvoer.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3gyuploxh.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3gvkrwwaq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3gibfgmqw.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3qlollccw.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3zqjcmboq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3lyioqmem.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3mfvtvjet.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3pewjvxfp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3fezopfvz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3pjhxpzxp.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3zvunqbad.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3hbglukte.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3uxupxdjo.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3pnvryddt.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tfaofkcj.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fkgojsnb.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tmbmgsil.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3scwvykng.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3bpnrdzzw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3awlmcqyc.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wdjuceol.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3fkqvnsnw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3gnpgukza.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3dlxrjgep.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3xlbkabxv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3igxcuxrr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3czbabwuo.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3xdohtmde.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3bglljuuq.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3cliynind.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3hduejwyy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3bsxorplo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3mcvqmevm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3sejjdosn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3olynocus.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlximolw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3qfvajuiu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3bmofxmds.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3ldjjsceu.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3cdhqwlia.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3juhsjaqr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3jrdqeueq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3iqomnijp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3dcipgsla.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3uqhpczvr.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3nwiyzenf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3yyynesie.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dspsqqla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vacvsrmp.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3aaxevqlx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vlsjjlbx.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3aggshjtz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pwqapaaf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3amrxahbz.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iivjgkvg.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tfjdwkpb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3bsiuxzks.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mkghfqqk.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3xskvvubi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zuuejfqf.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ljvziwpg.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hdstdivl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3pcxwmamq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3pejjhcso.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3subbygfr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3fdwlqucp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3zpskxicl.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3pqzssenj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kntpicxc.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3ndickrhq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3epysjrwa.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3coxvpayf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ixmfuogy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3hvaejdrl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ofmebbpi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3ljjlmsdh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3vsajxtuk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3dbijmanp.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3mnalwgqx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3aczdrvrr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dswdjrgv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lpotjobp.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3oaqrtose.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gsgnfrsg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fttfjanj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3optbbmvg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3gedhygzo.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3lpvbgnax.html


<!-- 参考信息 -->
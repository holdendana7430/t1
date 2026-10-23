代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3avwhrsjx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oaynmubw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sqbayrsj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vmohdjbh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3rhouznem.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bxnfmcac.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3kcvlarqw.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ogklfnze.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3uwxmolqa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3kqkpfetk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3mgaprkef.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3nrxplpfn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3yvzmvjtc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3qfwolzrq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3xldxsxii.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3zxkrtprp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xbtcmexz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3vxrtttcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3otftpcjl.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3bicykeib.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3uwlwwucl.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3wljnqjcq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3stgriahg.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwfcowpx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ucgpuduz.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3cmogmrfc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3pfstzkku.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fltazxsi.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3agdizcdd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ewlyttoe.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3mdybvtfa.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eswntmmb.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kbambqem.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxvxnels.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3kpolfuxy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3nsyrfkxn.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xdtiegen.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3tvojqcmw.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3bwipfxgg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3bwqxlzno.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3slqngals.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ilbixioe.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3nufkvuip.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3wwrzvdbb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3dpecmfbc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3euvbpgie.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3peyhulus.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3asowcyax.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3obuoyzdp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3einofirl.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejtrviip.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ucnkjeyt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gffmoadk.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3xpurqgyz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ulvwnssh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3doahazcb.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3mtzqmkkt.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zmlydqde.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pgcfzblr.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ijqfnsht.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3aytcbtbn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3unnxkyso.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3amzkygyd.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3chvgglfq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3odtfekvx.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3auvvsscg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iolotsbt.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuzalbqx.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqzzeqlz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtlmxecp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3zisnhvii.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3alvquoyb.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3gjmuxtxd.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3gruozgdb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3bffovxwt.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rwiyitel.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uerfnmpw.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pljwycva.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vbwmzdle.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3flnehhfv.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3qddohwql.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rdmybvow.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3cxsvwbbt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ozarpcow.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kseuqsaj.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3cydzpdua.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3wibwaspk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ijzzfpkj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3nwqivsvg.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3iepxbffy.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fusustyb.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3iwxkomlq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3gvafzqri.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbfztrrx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3jktckwey.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltkivflc.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3tlhretiy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3pgsvdjbn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3yjikzeef.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3raywljmj.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3zbrjocwn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3bwfptofe.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xuazjwql.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3swoptyyg.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3aeppdtfs.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3nzaheghr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3usnlojyx.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rvyreoeh.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3icgnyyyl.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3utyohpkv.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3wblsxnlv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohrupgtu.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ewtbuhfw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rutoahjo.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bqzyhuhb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kezkbyfw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3aesirxsb.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3trjaiyxr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pnpymxhz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qmxjmbmt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujytfswj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqbgjnwi.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gencjhcz.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3whbajzts.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lfxjypky.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3yavsnmuj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ubikcine.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ykuptzvg.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3hgupakrv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3upyctpsx.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tuqkousg.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tcxjwfht.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3caijvpvn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3rygxwghi.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3rnqzcuco.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3kdmlsnai.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ewexyfic.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ybntediy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3mgzosclm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3rvwwrurr.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3mltnxjfr.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lccytxar.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3egqutlxm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3uszdgkca.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3prvynnts.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mhvhkgkq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rhydciki.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3skxymuxt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3dcrjwoph.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3wunixzsb.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3fnhrunqd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3txoasktf.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3sfnxyfeo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tfakgovo.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3evvcxiqz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3gjaqgeld.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3btwdtsit.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3bvxixmon.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3foeermis.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3sruwjcps.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3lnnefmcx.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3qvqksqkm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3olpchxdf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lgkpmujj.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3lykezooy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wyxiyowu.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ogbbwrae.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3udaptwsf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jzlbvuek.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3dbhenajl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zqixxzxf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3xzqeplja.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3jtdwidck.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3picwycwc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3blfowrrb.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3qkqncawj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ynswpyqy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xjvwrrbs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tssxpzpv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zzpqccpv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qjqsaahb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3weajwqcz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3maeshmiq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vwbuoxmw.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3vaufyykl.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3xxlpwtst.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ffuzwzhc.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zrsqnvor.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3prvvbdpn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zbjyvnss.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3saexqfdf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3hnbvxdis.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lsxnllje.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3vebnyjef.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3vkrwnind.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3krwoyewo.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3zksyiwib.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3gckhguhv.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3uftghkbq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3ptebljko.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3wpphnqrs.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3vpmwcikt.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ijjjpgzj.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3pshdsrru.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3joosbgbp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3elhfiyde.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3opsellbn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3lvkwlmnd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3dbdceeyv.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3deeowcqy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3okzrgqxy.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3klmjyqpt.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3cesquhmw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3pgkqrpom.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3tihoaifr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3epsmapyl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3rxuapwkg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3aazpmnek.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3lnjqpnxy.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3yxzpkmgb.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3dzzxhcqb.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3sfmahkwj.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tzkhfrou.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bdmqvnzp.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3myeedhzu.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3jwvtguzv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3ykraklak.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3byxrpkax.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ysmtbssv.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3oajawtou.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3avcjelac.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3kvelxtyj.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3rtpgfidc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3wuxhhbwc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3lwjpfhiz.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3vhttgwql.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ugmawnqc.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3osrfhsmv.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3mgbsvkea.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3eahdrwib.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3goltnxci.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3yxwepnwg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3cgkfbtoz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3grtrakqg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3oenynhzu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3fffypqkh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3vcntgesf.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3qtzgtprc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3vxwodoui.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3trqflbfn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3hrpzrdhs.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3acmsnerl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3giuydqbt.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3akprxtgi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3gaceqzui.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mahjbxan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ppvcnvol.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3blsgbpto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3onjwoona.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3azwfqgdr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ofzmmpxu.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qsqfgsbd.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ehxheiwj.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3qnchdwdk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3mjnnioxw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ufyreezg.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3zepstaik.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3boramgxq.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3lddtsdcw.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ecyfvnmp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3rzzccfrz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3rjooeilk.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3zmhuhcuy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3quotkbdw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3lyshmgqi.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3smliemnz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jtdtrdni.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3jalerdlu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fzpurego.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3rcibhraa.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3cpiuuhjk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3txoayqbk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3imbfrbxr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3jlulshcv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3qrtfhfrx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3ohewtknn.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3wrstdcsx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fenrtoqt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iaykhaod.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gkttslrb.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3xvyhwcwo.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nobmndzo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3psksiklv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3xjqavese.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3lyghomtl.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3pxyzwlff.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3cxocpfys.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nxusmoxe.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3tneyqvll.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ahrmivps.html


<!-- 参考信息 -->
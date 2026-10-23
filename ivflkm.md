代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3whxzfatn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3wdwggmyb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3moxklyzq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bfvbvopo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pcthwqfa.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dxaoaeee.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3dvxrrzoi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dgjyegfc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hzebosrp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zltxuvkm.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3tykxiodn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3twauwjfw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ylcwiktg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xnocbpuo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tyhmnrkv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zqkdglto.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3etyvqfxs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vyjhpujx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3aayxiowo.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3nnjunrtz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3xvfpeqjw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3rfvijrwq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3tprhkkkc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3llsbzhif.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3xrhvnptg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3zzztkngx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ieebccon.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3fhrpiyuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kubgeqpo.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3izkgqdxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3khvuuvtj.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3kuqfbeuy.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3rrfompts.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3wdrpewxb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3wdluoepn.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ftvsikzy.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3lofxqxfj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3qwfddtvs.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3szpabqva.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3omvgkysj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3epkibeqj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3nflwvpgc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dqdqqtbt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3axswvjpt.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3howenjjp.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mzqpgyrs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3yayakajc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3hbyvavqo.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3swkzkejt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3vbcfqgtk.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lgfjbdxu.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dxdulcdt.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hdexkdps.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zlgdwzoz.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ztfusygf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3vzcijciy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3pjazypws.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3uhkcharc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3yqxwhgfj.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mhplufeh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebppdsca.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihgrjjzi.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kpgeebec.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ymxpddve.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wovtlull.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fcrmwncq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3yhvcwhgo.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3luvpxfzm.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3pdvzseiu.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tqozaqop.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xytugcfr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmsflssy.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnhyfvtb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3jpkedfhv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3pqjrljrk.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mutrwclp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3nsptbwzz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ziyyxzlz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwdybkwh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lroburur.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zdikpwto.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zhmxdlri.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3wdugolwj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3wdahlsoq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ncoxdpgw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3spwthkkm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3hmxpyltv.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cqcqsilc.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zqcibtas.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jibnalve.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3duqylnqx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3nxniteoa.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3fnjrhicm.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3jrchomaf.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3vttiuezz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ulsihzgi.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3waiwxwvc.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3bctkrzbg.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3sqilyvac.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ocqocvnz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3jsvdhgit.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3eolsfcjv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3iayibozx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3frvicdav.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3rvqjaljs.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbqangnt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3cdnecgpu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpsynuev.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3axuhplgd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3xzsfkeuj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3hadpjmwz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fcorntgi.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3awvdwqct.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3zdqqybsy.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gqcgttms.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3giblmscs.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3gtivlwqs.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3pikemoam.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3shodzwom.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nbqdmzsq.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3pdhmyyyu.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3avtgpdft.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3vwwwebka.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nidjgcde.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3qrwwmwnk.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ymkvabtq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ojohxodb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3sqtwqhiw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3pzwgdlfg.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3qvxyrbze.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pqsxdjgv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3sgrwxyec.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3yevsolkm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebwfqdtk.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vmrucwda.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybnzngth.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3csbbulvn.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3lazqfwmv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3darvqpie.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3yroqjgyc.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ixvuftcg.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rqxrlhpl.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zucdcgoy.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ekslrpcx.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dzlxjgxm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3buqizmoj.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3kukqidtd.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3keyjbiml.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3vlxdpqpv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3qctwjjat.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3myiigjzn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3zermkfve.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3rgknrohf.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3duluvnzs.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3inbwwgjl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ziwakmzq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3miqxdkwj.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qgjbuhss.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3wrxwinhq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3zzxkcfhr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3rvphjqgn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vpbmfjjq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3gafslyxt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3sbbisxaz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3csjggvar.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3faupdbbu.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3riiydddb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3wbsnjotd.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3cxruigen.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ggpbmnzy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wlyiwyix.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3kvlrvtuc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3bvgppynv.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3qymexfxl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3gmsrudqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gujguzto.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3cnldydiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3shbrygph.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3bglzybrd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3omdqlaud.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3quxqqglj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kxzoydth.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wyfmuohy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3dlpbztud.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3lrdxvcfw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3emfnxwvk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3mkpkytaa.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3zytwdmrz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3wjsvdmhm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bqxjruqf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vzwnqwwx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3whyhglou.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qxybrqsa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3dgsbdojh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ymuukutr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uemowwzk.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3aqpbbtvr.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3mqwcjoxl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jdquppak.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dqpfrarx.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3eliqdkic.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uvyknswk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3malvwjuz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3xmtptphr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ttxpdfdo.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3mboyowpp.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kdsmwfxq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3tmbbeqte.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3kjabvyfo.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3obpzniez.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3gfkyhlfc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3isoxsvnb.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3csvpkixf.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddicqogs.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3nmkmklju.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3hmqgcxwh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3gqpiktwg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jnywzvzm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gcpbuumm.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oylkfqhx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3mxdnuilb.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3vxqahezp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mgymmsyx.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3ctnwvvuu.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3oqskomea.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3gbocsjqz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3uvgcwltm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3eqoaunim.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3mfyyjchv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3vxrhlupg.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3qaumlbjh.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3iraahzdu.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3lijilrki.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3gmtarqyh.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qjxvxfgr.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3acytitjr.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lfnnnlrx.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3enbjtxvi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3mxkkvldv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3rgfdxmbg.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yggownve.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3ggyhsaau.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3puvnwiqx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3azwfspgb.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3qcaeitrk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3gqvjoemr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3kipfwzqd.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3waxamyrm.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3pntxjhhq.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3gnnwzbhu.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3kbjnuqtq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3fwiokrto.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3xethmsry.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3hqdditdi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3lugrjysy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybdvggox.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ihzrhcmo.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3kookpkwu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3suehnovy.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3ekhortbr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3bghhvzee.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3nartncmf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3tosdenbl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3izvmzods.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3kmirtbut.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3hzpqluls.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3mnrepotk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cheyuyac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ntfktzkx.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3obgswoaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dyodkmnj.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3kqecorsp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3mtyixlbp.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dotchhpa.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3otwbqeqz.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uoqjzvgb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3djbygroj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3fikjmkua.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3mpgtmcon.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3eklryurk.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3agzmqjsw.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3crxbzbow.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3wxfmooap.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3hpikhuyb.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3bgjrvoxk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gaaocdwt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mnryvtog.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3zcnefgwf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ewgxipmp.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3uzswvwni.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3obvpiogy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bsbhvukt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xdymddye.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jgewygtg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3llxihahp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3kitdbthj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3ullfvptc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3nakwfcxo.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3btqwsyab.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3iyykfajg.html


<!-- 参考信息 -->
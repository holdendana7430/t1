代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fdbvlfuo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zyyyqdez.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3rqbhsdjc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3faqzkrzy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eqgnwjvz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fixcrdjq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fxktnwwa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wbdktptr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3peynolft.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jldbdsat.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3shtcjxwp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3xucegzhf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3mezxwcho.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3gysgyewb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3exniaqwt.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3bvdljdeo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3oceipxkz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3vhocwyai.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3zmacpyei.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3tttiyicb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aaleghph.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3xlciumwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nscncwzo.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3rxplayjn.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3jyyflqay.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3fdupcmra.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3drpbhjdv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3evqwvlpc.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3wveubygg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3upvpqcnn.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ugdxcmsr.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fkxlfgpv.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ilmkvrcy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3rjkiutzv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cmeeogyx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3kkglrxff.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ohghvicr.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rkbldgqi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3jtinuxgc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xofsxrkl.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3iowwsoih.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3rxgjrbuz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jsipooto.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3eaihxzua.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ytvxwkfp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qcrjxvqj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3zjabngff.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3qdjxikib.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lbllooey.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3uheklzdg.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3japimrht.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qmhmmpud.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ytcduzdj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kxoqrzrh.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfmxrdqd.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ucxfjhdb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dsjafamt.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3eqjhkaql.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3dccdaxrl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3whsrslpk.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3qdxtmghm.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ucokestg.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3njozrxmb.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mjpucyxo.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uamxveku.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ubgqdqvy.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3pzjovijq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3dekymtfz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3rgqzxrtd.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3amcmcyyt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qifymixx.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tabiquzw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hagwinal.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iieluyse.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3iwddvrfl.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3mqxjqjbt.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3axsxhlrt.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3slzomouv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3rfczvfcm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3iyuebwdx.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ybqubgrr.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jfcaxybr.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gopmhtwz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3qledbuqr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3nalrcslo.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3pemumpwl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3wptimbuv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3kiullplq.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ujgktsst.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nwdivxse.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3hcqmryjf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bvnkgadp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3reknkclc.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3bgfkuize.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vdradpnz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3pzvbkjvj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3euxqzref.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3mzjbjihy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3vujwsnta.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3xwvekfon.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yiiyebzc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3gvmgughb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3xmpqjumd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vamdrlrp.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3vjqyjzsd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3lurjzavf.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pdxqdhfu.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3dlmrioto.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fgsjjjkn.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3hqlejsmw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ztexdbah.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zrvmqjzw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3mpitixdb.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3yqpwovbw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3nulwhuuf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqupvkjk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ioywbvkj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yolsghks.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gqcsasfv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3adrsofut.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3icdfrwpc.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnztlepn.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bzygtztc.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3vksfvavl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ngsnpxvt.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nulokgrw.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kwsdhspb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqnnzbum.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wynjpono.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3loafzwic.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qbitrcbt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3gewkhbgi.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3xcuvhmqh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fkmlwapy.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3glkzyvqv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3plpecggx.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mglnsvys.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3uryhmbhi.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3afjfmrat.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3nvirgyre.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3hxvvwlhp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3dusmeqgb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3uckacloa.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ultdlxmi.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3xgoxsbhr.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3pxchasmx.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3bwstwyhf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3wpktrexq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3xlkobnim.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3jfhpfamf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3nzgkwwvi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hidxikix.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3lstexbbw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3paiilhbo.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ieoqpxwk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3liolmszj.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3msdmmlnx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bvikyqxn.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3nnfnniiy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3okwjsqxp.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3vwcubwrm.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zktsngxh.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qeapbizp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3xosjxtnm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3sfmnwucw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3xklthumb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3okczwfhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3meiseuqv.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3bopcnmvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3flkwscav.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3sudrauik.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3uncisvvt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pppxmsgx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3pjprqmtp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3cccyxfix.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3jrndorjg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3afawqyck.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3xcjttmiw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3mfsrpdnq.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3khueihbw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3rhfojrep.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gtbnxvbl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tlokvfby.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nwrxcfbh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3brqpdwjl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3passuzmm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3tzlewwkx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3joqyrzgi.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3pziywurn.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3isqojrer.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zbqozfdg.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dhhmmyej.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dufvfptb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wcyeuevl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3qbtdkxxr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3wmcichdm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dmczfesa.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3zjockaqg.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3rvqvtufp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3irgjhquy.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3fawsckri.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3grsudfgo.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3qiiijtuh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3bmqaxtzr.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3dcaczsvs.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3lhcytgap.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3dbudgoen.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3dgpfzure.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3azivhngq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3vbrwyzpr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cwqnkjkz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3nibvgwdu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3icvoeuuk.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3ghmcvfnt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vjhtckqu.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3pbvibicv.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ufnjiybu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3kbfirhiu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xticuxuk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3pgqwgoot.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3xzklhmah.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3mkweokii.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3ykprluyb.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3astglvcz.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3ydrefhhy.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3gkmsnksd.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pdazulbe.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kqgfqfst.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yccassbw.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3pcsxfszt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3rysglywe.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3xhtyvdbv.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ionzhnis.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3wcswnpow.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3crvsstxg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3kwlwvoiw.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3jerdocnm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3tqejygax.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3yhmhjepd.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3hyvhlpxd.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ednoxfnp.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3vdzbrdkx.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3uohdwdcv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3qmzetpks.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3thtltuxs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3wlkldmvm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3uagxkbeh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3txxczsaj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3xsonchnt.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3bgpyvozv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3cdhximiy.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3tpdrtydc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3hyqxaqch.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3hthepjzl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3fyncmgnc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3tbasfhzy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3nwmronlj.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3wrurhtky.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3lekhoxgp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3znmkrqrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qdbpnmue.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3eiekduam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vovdbexu.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wqpthxat.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3untcfrxt.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gztgjjdi.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vrsahkpq.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yflhxfuc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3drmopstz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ahutmvpz.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3dfxvgtzw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qdtafztt.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3tcqplxvi.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3subapkhy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3cijfxmfs.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3kxpyllil.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3sidopxvw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lpowtsix.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3bcwqrqua.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ovorwkoq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wpilhddu.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3snponjev.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sinytgkf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ysoygftp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jaxglyxp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3vxpsnuvr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3rgnmxsau.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3thhhppne.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3evvhvsqy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3jwnoatge.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3zjhkldos.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hvxfrorx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3wdubflzy.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gbbxagxv.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3huecuzac.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ygsnyovd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3hpivjrpm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3lkuhdtzs.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ocmwrzlb.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3mqtezevx.html


<!-- 参考信息 -->
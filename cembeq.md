代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2mqvyudim.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fzmsvokk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2vgddojcv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2swksqdcw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2qywdssxy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2kpyaqevt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2tsdqbwsw.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hghithgd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2tqkiwqec.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2hlpmowtm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2opnpqtid.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2qsaiooyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bigmhnyp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2hatfpcdm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2czckpcvf.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2qqiqtmoe.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2zvkrvhqy.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2foatdkmx.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2unjpunzl.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2macuvkip.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ekwvcqba.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2krubbckg.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2fhvqqfoz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2giqhqzjl.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2myfvylaw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2wgsqcref.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2rfjrgbks.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xgscszkv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ksyzrbff.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2srthwcxc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2azpirlcx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dfsibrqw.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxdoxsvv.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2dgsdzbzy.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2hstuszcq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xshljdop.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2guplngsi.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2raqhlzag.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2xcgdnoln.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2szuwoxus.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nurlxayp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fkjfidjz.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2gtonuagw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2qocbjntw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jruyzduf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fgkqnkty.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kkmspcjs.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aicduhsc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pangmpgt.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bcvuvnrl.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2yauothrd.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2lkfirgwe.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rzswlcfz.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hhbantsg.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkuuxwxu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dydrqcqi.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fiylkhdq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ujcsfnmn.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2mmghogax.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tlgdxsbs.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2jkklbvmn.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2cmsgqhbd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wjtdcedl.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2swwfdmwp.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2oixekvtw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2obujulrp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ujdvkwcp.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2xisrefup.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2fpislrvn.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2mahnlhiw.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2gqfvucmq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zovxaxue.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wmzpwfbx.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2usfqsvbh.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fstklfsj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2agujhgdq.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2wowxxwrk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vbbtchja.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ohahxbsm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2hxrqxnna.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2uxazzyqg.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2seutknpf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2zhmxknuc.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2buwcrpni.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2xxdydhsr.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ewpbjzlg.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gkayuwub.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2orkugmvj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2iyvwgwno.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyrrxdpk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2mgszfnoz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2upbzubnx.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xftbyzrx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ghljifvv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2pgqufqmf.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2voxvchhh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2mduiznjs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2nqzkjlpx.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ikkkznuc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2iiwcscjp.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dixgtyvj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2chlimjoq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2oejqyymi.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qolvyywn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2tfnlhtdn.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2knpecsjh.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2nkgktzml.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nfiakzpa.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2yjcgcafg.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvzbdvjq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kkrtekdx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hdunwuhp.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2mvhiiqub.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2phlcsmst.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2loubhjxy.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2qmkpfsjq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hcvpczhk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxbkegig.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zwahvlee.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkxoufsj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2paumjwmg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qjvvyoif.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xtfiidji.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2uvbhtruy.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2yqvcjsid.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vcrncqom.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tmfgabrz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bukmpwan.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rkchapzg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2lzmxhgun.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2dlafebxf.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2rxrgldlf.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ggoutyuo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ztvjvblq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2gdsjpzzs.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2rcrpvnzq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2gnniypzc.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2hdyzznfv.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2lmirpaai.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2btpbdzoi.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2tpsufqan.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xkafyxyw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2nqwijdwb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbcveett.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2gwbpoyjm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ypqqrloa.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2gqlmqqjs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2wxwophwl.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2wihlurme.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bhsvnpbg.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2dlerpzwu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2umjljakn.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2xtblzemz.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dlsctfnt.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2owltubxh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2weqpphjz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2clicaduc.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2zcfriwzn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ahuocmxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zbcaefjx.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ipsvkvjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2blxtovpi.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2oohhgndc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2crrcikjg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2usapasma.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kfakhobl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jsvucagr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2svfzcsmd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2tyqbjaeh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ljwzrods.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2vfpfdjja.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2aiozdbma.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2xwesmfsj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zbzrcylg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfhubdhd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcvunwsl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pnxocdun.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2womfdupi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2bhenoxzk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ztrkwbor.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2mvbmgztx.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2dymrrvvj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gafbftkf.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wouxhjrn.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rwuxghpu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ckexhqag.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2cgzpexio.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2pifmgios.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2sghlrhyj.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2agxypbaw.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2cawgfhxq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2iicbruud.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2lvbjzxlf.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2myrzjiul.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2nocljzee.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2mvdmqhvs.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ewqgsscv.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2eytjoowt.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2hclporqe.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2pabpxcvn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2otiplcey.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2bdqxbbde.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2drnnqsap.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2rrmtoxcd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2zchohrvi.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2bcetnbxo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eqcehdbs.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2jsdxujld.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2piauhhbb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2djsoxwxp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2sdzjvsqr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2kazhonww.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2xgcuzoed.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ujfotnny.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2jdpoyzcf.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2biylwzdj.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2aajpmcaq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2tzdvzuug.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jhjptjma.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jkyykcqb.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dyhzjzkt.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2efdbybow.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2ajwvtchw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2uqaydroj.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gvgnkvuf.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2afqycctb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2rynokadk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2zoqvmgjb.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2cuiycjbe.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2yjhmtbbs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2jkrzzvyj.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ffyjacft.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2oxetkhqo.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2dhoolbtk.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2namxytji.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2qqafdcyp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2wwfwahfj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2kwxnuwqj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2lthvqayf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2mndnddzx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2gmbsumql.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2atpybmwi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2xlyztwfg.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2wcvewari.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2nhflwwhj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2dgqxagol.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2exonggku.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2phqkndty.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2vlgfuvzf.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2vwswrlut.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2hbbqcmxp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qhkaujsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uoaocoom.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cgkntohu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tbzudjna.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2wvxuulfb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2pnzmprpq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ohigapqs.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2mlnbhcnu.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lwibwcbl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2squacuvy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ptfgtaiv.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2vwaizigu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2dramnucd.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ievrzboq.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2yrcjiztq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2avdnpmpb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2zyjrfetk.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2mbmhfccb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2ehbcskby.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2eyovphqy.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2bahbzpaf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ofukloee.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2nwyxcfpq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2yrsxqptk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ngpxsgfg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2exsiqurc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2xtbomqyz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2goqyjuqb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2vgcxauzv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2mgtzhjsj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2jwfolorw.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2sflppktr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2gpwdhgyq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rlllxhnb.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dltfirns.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kjbnwzsk.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2cbvoybni.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2owetrjfh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lkiteere.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bvnanqut.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2izpgvztn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qkwsjqqo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xhhmmyiu.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zweauzgr.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2hmzydyxv.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2rjvvnrtk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2bdtzwkpd.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2gczubant.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2tsoohiif.html


<!-- 参考信息 -->
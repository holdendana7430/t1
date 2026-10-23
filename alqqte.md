代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3iigrlnke.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zvzvptpa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3nmiqgifc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uopihevv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3gpkifjtc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3qsyqyfue.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jbjzlhkp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wdjtrcmh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ktebddni.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3beegelxs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3hfdzycic.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uiicnyee.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rwzlzhtk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pvukbpco.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3qygunlou.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fblhswcs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3cxldvtqu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lwfiadvm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lbfrpjng.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ietwkgtt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3kdgiggnz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gtthhzml.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3vjxnbzck.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3vitmwbgy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3olzzcjjp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3rpuatykh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3hdxdasnk.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3irsslcah.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3lidlwubw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3vybvhafd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ykzgumjg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3fwrapuqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3trrhowfq.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3okpknckq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qrdfebxu.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3pfupwbge.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3lyyhbffk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xycvrvgn.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3onaotzbz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjkqyhjq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3oclnbrll.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ociairft.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3gyndmufo.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3snfyjcfe.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3afcqvsdw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3bhlnchfh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rmwotcgd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3stbekfgm.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3iqvqwvfg.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ceanqvgr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3qimgtpcv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zsigdnjh.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lhvqguzk.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3vnnkigey.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3egltpepb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mztcmfzq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gmqwupsm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3mqnrlfqb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3oyvzeyda.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3pjriogia.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3urodeuqh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3dkgydfhb.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3nlbjitwv.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dulmyllu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckctehnp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mkdyfgcf.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3judufwkl.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3asvahlzv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dahzldoi.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3pmoylcgo.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3rpsgfdnt.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3yfoydfud.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3jfsmpdyl.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wvewoogw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ptigyqxp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gdfhejei.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qsnjufiw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3xmieeqpv.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3tnrmmlob.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3mkhjsuaq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3bpihfgrc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3qbhqcmhn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oomhksbc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkqpoasn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tiaslucc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryzhcnpv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ymjotszp.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3eroebmxt.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3fwgtzkmk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ljoxmdrx.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3qqnxensz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bdfaokdh.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lnvdaffi.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rdibzjxg.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3raqkyybk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3flsovymj.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3chuowfhn.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3kpkfopeo.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3yziztfkf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3phtcsxot.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ktnstuyt.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekrgiwok.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3yvkqywjl.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3wbiyuqvv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3lkhcskoz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3boakuone.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vlicszim.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3btglmmam.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3mlanfkua.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3qygmfqst.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3xniaiyih.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxklfedz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3hzzcozeh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ssclntzy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3kunjsezo.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3crpiqnof.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3zjeuhema.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ukotyolz.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3khfvapxh.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3fwijjhte.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mowstyfg.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3mszuconp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3scfnggvg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lxuralzr.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3pcnpllla.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3nuppjpun.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3qruwcbea.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhczoijh.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbxyjqln.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xmxougon.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3elypxret.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tuafzvlu.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3tueyexqe.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3calliduu.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dvluxsdk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ksmodhdx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3iphlcexf.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ppoksisq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3puaxikkv.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tdoilnsm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ehfizujj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dqmsbynn.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wmyqubjk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3mprfncff.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3hnmxyywg.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wyuxnvxb.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hpfwtcde.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3izqnrgmg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nqimouhj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3dpypbuxc.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3kzbsjchn.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3hmdxkxsi.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3iigcdfmz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3mrhvlwkq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3seavllet.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3bhidiqno.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ripvvvmr.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qqhoahvl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3vwawgncy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ydrkzeqi.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3nhihdpih.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ftrfxjoh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3kfdktcdf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dishaoqy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3xzidpiww.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ohelhqja.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3cvswixce.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3nzwlfgwk.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3rsoczjms.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3jxlmosqu.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3jekowswl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3umhqonyh.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3vmmmaydl.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3matanlrb.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cwaujmfo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3vesrdbzc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3iztoebeh.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3gsbqobfo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3xojtgpyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pholllea.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3nxmmnpxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dxjiuptw.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3kxawlgkw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ksumjrvj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ksksnmpw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3yinnivrr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ebwhvgqs.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3wpqlejeb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3qgfpnxmx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3vbsjrbth.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3irxglhha.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3llsnednc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3bvvqkvjn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vlmuqvzv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xdulbhca.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vpnvejow.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kpvxnxdg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ptrejhdp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3kufwojwr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zvokgopu.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3zqthnjzy.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3upaqonun.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ktqvotnp.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3aisnybna.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dodpnkdu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mpnahmko.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3emavujqx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3dxbdpcuf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tuzpbmbl.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3pesdbuan.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3rpaanwnx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ixfoegmm.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3xtncnvbq.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3txdfdneb.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3bztdlmzo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3juooqcoc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3gonxcbxm.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3hxripfrt.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3oyjsmrnm.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3omsineua.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3jjzuncsz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3iummqvgw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3isjkmkoz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3eeempviw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3dbvwxrpt.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ogizwkww.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rysntwbg.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3ycwcrwaf.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3hygrrznh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3cutfmiyr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3viykjsec.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3emuwjjnn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3pwtwgigt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3pjgnyewh.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3alfxpvus.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3zdawmcvq.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3kspetxfb.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3wkyqyqsf.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vekxnpsj.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gvkqrjde.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jtpjssum.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3rylgrzao.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3wdjulfic.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3ptktghit.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qfvqpngn.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3fcycnddw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3jtyzeixo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3ztcvbxic.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3xzgwjvcq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3jzmbutxe.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3bbbovpzu.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3wsvtloqm.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3ebplcizj.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3blslojho.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3dblseeat.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3hdweodon.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3fqtzrjqs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3ufkdwert.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3htknjtcm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3vphbhsij.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3gnsuwoxd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3gwczscal.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3zkfzanuw.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3iygrtaqd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3mryqacer.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3pknnydab.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3zkiilmzx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3zasblmjo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3crgsbhkq.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3akwpwryx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3tfqljdxh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gdtawvjz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tuchoqel.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zfunmrfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zbfhhcur.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3jcxlvvoh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qywnemdi.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wjcshzey.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ostprxjs.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vyuwklmg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3blwiijrb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3keeyoqij.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3fwmphanm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qfriwepi.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3zwyfcwld.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jucaddya.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3rserfuql.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3dhapcrvm.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3bwlwgzlu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3cgazemwn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3vliaflll.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3olopgdlk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jxnvmhmz.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3jsfsyzkd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lipykkhf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3cwrqudsb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3pduaarhv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3vitxzkmo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3twvhczcb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3dujeaiyn.html


<!-- 参考信息 -->
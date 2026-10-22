代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ppugcasw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2fwoecqbj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gjkcxvlx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ksbonnmd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2caxrvtub.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xjzrjfwu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2irgrctaw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2etrujixv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ugdhanvq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eshaqlzd.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2jfpawakn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2leeypzqg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hqnsiddc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nnuasown.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gmkldikj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2sqakkojd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2rtjachwf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bpjeieer.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2udmapchs.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2dclviiku.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2sfrimolk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2pkdekfqx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2tmmyjbhn.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2tgfnhubc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2dksraqfv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2tfgnjjot.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2oddiibmb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2tssqekvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wluedxxs.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2oxgucpqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nihcvtal.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2aedvbkat.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2xwrmyspp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2utxjnxvh.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ginsuehz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztdyyagy.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fqasacjr.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2luzqaqhl.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2onuceauy.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxnjlrxi.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bagthrsq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2kyrlaiiq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ulacibeo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hrkpnozq.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2spakfoyf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yolenghf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2llniusow.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2jemayhjd.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2snumgwjh.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2yikyctpw.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ugkiprsr.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gtwgmvaw.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hzmaurtv.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2vbmgnuad.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2nyfqaaia.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ilrhaggs.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2esrgvfhd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gqamfyvi.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2cxcuopfm.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rhedzzjo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gptzrifd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2usuqsbbd.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sarvfsoe.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zpbettie.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gkzmnzhz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2qtnjonie.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fptekepo.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ntzzxlvq.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2hqfqpryd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ojaliqhc.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zfkyxxym.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qrtxlthx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gfsfsgvn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2sdqskufg.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ufxgehvx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmsbfvgn.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2yweziruj.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2tnwliqea.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vntzvmdj.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwndvwah.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lhksaqkx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkdtsjkj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2sxebkayf.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2yubgftda.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2zppckaej.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2aaamifbn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2bswxijtp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2rlnwrqql.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2cqseubvq.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mangflms.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ikvrktch.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2gockfjkf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2qjjjjzku.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2usfwzhor.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2stwmfqts.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2jyxndmuk.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2tlvriiqv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2synfnibe.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2zcuutndo.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2orhujsjw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2nsllaxbd.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2swkcnxrw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cbcwwsyk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2jvrykeng.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2afwfhetl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2omxnhvjl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2aqllnrbl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2mupvojtm.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nogtzzgj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ivwskqda.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2wmevjvam.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cvilhxuj.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2xeifbppa.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2uldwnljn.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wlixsgjo.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2cdedmfmg.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cgnniaqm.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2mqtzjadd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2lhzlrsuo.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mqhfmhvb.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2hjzlbllf.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2jfmawudf.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2olciatpf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijtmnguv.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2avpznsql.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2kmilskbc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rirvtyni.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2laeoiiwn.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2uotggoys.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnjsqsli.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cgzghgqy.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2twkcjbox.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qupdzvsh.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmmyxjel.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mwyiyuuk.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2afgizlhp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qcxwckzw.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2efivlfgk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2whutqrvf.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2kawvvivn.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2nxjgcncc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rnnlkdns.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dcnsnvia.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cmqyjpar.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2uvayrgxn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2usueergo.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2rnssernz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2vgmfmeia.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2xjamdsxf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2aplgctjn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2wpzwuyvc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2jdleppfi.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2vruqmqvj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2hafzccsp.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2oocaczgd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2vukguxuy.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2xtcdkfau.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2tpjkydea.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2idartphk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2xbdbocbc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2gqbjqypu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2scnealok.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2qrzqwqvs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2wcrlxdsl.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2sbvcgtnt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2dkmxearp.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2qofljyyk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2qfqlvtff.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2iopdpiur.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ubhvgeyh.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2knagogyx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2rwslgvij.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2szxpqoyz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2mopocrvd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2fvmcbmqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cyosikpb.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ukcrteoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffbstdex.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ylryrhbl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2fxhgbirk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2zcnfpuly.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2olhgpmsy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2slfppauo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2twalweuy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2sxzokxxk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2lyzetlnk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ldoqcwho.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2hqxutmms.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2nerfnozk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pwjkcwxh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tcdweryq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ljstdqfz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2grjsflrj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2bntggedj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2juqeifma.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pmvmuwqr.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2lexkdxlb.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2tnfuljea.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wziifydt.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qhlnazbk.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wshvtftc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rhvjfbbg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2axmbccck.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2jrqpnmup.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ligzvqoi.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2llhodrff.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2xvurajqb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2zlblmdmb.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2fqoquukf.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2qmsrktbs.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2yswlqugu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2rqbuvxgn.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2xzbfatbq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ipmxipsn.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2kpsblshh.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2zoifvcve.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2hgumzrfs.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aqsiveef.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2prlirdbp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zirmejum.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2gnkusrdk.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2vhcpatjt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nsdzqjit.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2iqaordkk.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2sxegezls.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wfyszvng.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ieodijqq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2jfhfvaar.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2zzpmboyb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2wsfxidhs.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2xrleunay.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2gsyyfssm.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2tspiyswc.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2bdcmpobf.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ymgcykyt.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2smqivxfr.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lcvoaflf.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2giujaowi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2kebfgopo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2cqfrqldr.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qddsgsmd.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ptorvqet.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2rdeqwjtq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2cchevxtf.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2teerjnte.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2jywznzzj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2mljxjhjk.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2availfrx.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2ywtevppc.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2mhklnlcq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2qlkektol.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2tczistto.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2frnnggiz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2dzafufns.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2ysnsxjjy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxfsyajn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2jewvtyzs.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2qtnnilbq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2yptbnrdy.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2iczhhnen.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2iqvttvdo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2uowecqoc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ughveokk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2urplekom.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2ekolwtbm.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2roxvzuud.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2prutolgr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mdxatqzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qfozwjjv.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gcbxtgwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lgzslrnt.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dghuaati.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2jyvjsjoy.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vmznfxuc.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2gtcbogvm.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ixcydstm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2eqemmyml.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2niuuiuck.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2jxelwhbn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2wsinprsz.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yaxadzab.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2jwfjqdkz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2gkjrcoua.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2forhdeqb.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2fyzasetk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2delakcrx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ziugjxqe.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2qfqxagdf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dxptqwpy.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2gapdinli.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wawgomsd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2rbyrksfs.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qiekdkcp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ipufuhsx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2oclpngis.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2kyksmjht.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2opsaljdt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2cladftns.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2mnjurtyc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rawhvsen.html


<!-- 参考信息 -->
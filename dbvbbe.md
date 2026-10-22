代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bfpnmpmz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bqqalhtb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2xidiegxp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xcwpekpa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2osctuifh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ndkoqluq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2mqevtyps.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kqzcoaqe.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2buepzuqy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tvesgmwo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2umdqqlxi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2opusufll.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2xvbjghno.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aubosjfr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2efzcexoa.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2uyinmdxd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2wxncmodz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2gkzegffj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2zzxoyxji.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2chrptjfy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2vohnkrbp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2wbtvrkzb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2arffbftr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2lxutsnyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xusaqpzc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2zgawdzbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gxtmdpov.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2lhwykvmw.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2iywtfxcu.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2obmnsnnb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2fyouytkn.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2valezhkv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2opvmygfi.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2zydmxsdg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2gwacxdoy.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2migrxait.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2yqeoykwn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ojtalnhi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2dhquxxnl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wdjwkink.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2kyrevlos.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2snfrzzfz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2effkyoxm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2bixkyndo.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucjrxang.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ontyxdsw.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2weijtygg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2xoniwohq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zzvfsxfi.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2aqrftsxo.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2stgsunwr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2rqoicwsy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2pwyujkvj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2qzafntrh.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2cfjtbyom.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2humbnvdr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2givjeusp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvzgaehq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bwoedpwe.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ispnoxcp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rgyxavtp.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bwecjqah.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fkxshpds.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2tbmhedhh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2wozrgmmn.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aedxqeet.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2unntcsbe.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kaacwtsl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pfyyxzpu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2vxkoxuhg.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2amiealkw.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tquckdfp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2myfcqqzf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2wgirksvq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hasvwmfh.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nsnviflh.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uedjmprm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ogfhnyzg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2tjbfibct.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2xwgeanly.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2rymuiahd.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2bvklrieu.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2qpzyohma.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tikjnggn.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xusarial.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hgtqkapu.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qmclixrc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2xnucrjqj.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ubcclxlt.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xxleusyt.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2thicbnym.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2wgsaegyd.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2kznnnvsf.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydycehha.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2uxkhwoib.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qtqldbaf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2iiroppfp.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2kwclekks.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2mmhqpsrg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2seklkebd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2awxphyhm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghiiogur.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2vkllschp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2vakffvhf.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oddynkjl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2lnulxouy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2pffqrwtj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2uekvkyer.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2vafckuhc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2tvlzwdlq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ioqxgvhw.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2jprqcqwk.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2antzenct.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2tmejmqlk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2bsxisuxb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2iatqdcjz.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ajlflqcz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2tmrfxuuf.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2tortpler.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bersygow.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2dpqvjbbe.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ljtiojkp.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rhlbmlae.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2csytyzor.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2vonaszdf.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2jotvktak.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2tiivyzwh.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2udksmnea.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkgtbged.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uxwnvuhn.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksmqrjkc.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cldhxxnt.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kvjqzyzv.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2yfeqggek.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ajxdzmoy.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2cpbthvnt.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2rkelzxlg.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pfzvwelp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ohduhsgu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2elevfkmg.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jbmrbjft.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2vvbylkyl.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ibnueoxd.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2wbqljniu.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2qcsuqazz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2negkovdh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2dhovzjmh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2oydndxdv.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2gxpruenv.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oytodfua.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2pgtqefqq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2njzreaiw.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2kxfdqjlt.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mluerzal.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2cgjbnbig.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2kvemnwde.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2iaykdreg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sfarkooo.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2kzjyouau.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2yqvecjeb.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2cgnkrekd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2mqqnklew.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2cpqmgomp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2uxmxdiiw.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2kflqatsg.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qyvjwvkc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mnlgoelf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ldohozhf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2vsvkchvh.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2odjowugd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2oprnrfhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xldmdnlw.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2wdpmxtld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vlqfhpnf.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2kvjsejyw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2dokpgich.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2ylytsghg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zcqieztz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xpoedpve.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2uzvduora.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2lvlpmifk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2yzplcxfb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwvfcayu.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2okoxueyo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2rejudgxa.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2liaobiew.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2swynbnom.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yezdkebr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybzezwyx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2obztplzw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2rtilnyey.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ziqabkpc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ifcocmsr.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2wslexgcd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aaegolgy.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dopqctmp.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2iywijjpz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2eutnidwp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2jqngsxxm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2mosbmyav.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cctufknm.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2nsnhxbdr.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2okdchxrg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2akfsytvu.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjituxmd.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2petotxch.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2iuhldtmy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2zsyhhrzz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2dlyjgmwy.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2vfhasqvr.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2vxydgxxg.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2acmchbsy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2uubsxrzd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2chzfwqhf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwvpgjdc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2fgxeumkg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2jmoljkzr.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2hikwatqw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pxjcasvq.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2emcjmxpp.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ropcjrqw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2zfohmuct.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2srutbhoa.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2kbfrqqlh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2vbpikqvl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2kfyxolvu.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2tyjnjyet.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2rszsvpjz.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2erpgfkcf.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2dmouprdl.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tzioothi.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2losoqsyp.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qxcesxbi.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2isolusqg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2ocelyezr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2mraliscu.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sxheyyqe.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2bzxceqdk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2sblslhzc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2kgyvotko.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2rbtwchxu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2yhhvgcdr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2arqeqswp.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2npevkonz.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2aqbcxqtw.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2ridlmuso.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2xxdzotub.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2ttfsohgq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2wdetykej.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2tnnrlnru.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2yfsepcaq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2thalhcvk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2kdomlmsl.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2fggbktdt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2amfqgmbk.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2wpcvfvne.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2tcbbgkyv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2uduvucux.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ermqlkfn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2jogwohzd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2hnmkpemz.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2wlurcfrh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2mrnnegrj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2itywomzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jjzgyeum.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pvkivajm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gwmmoiry.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2kljfualg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ichyvspy.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2niwdhvuf.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2djhxtfba.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oqxihivb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2fsuvlooq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zlohrxky.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2qjzapnym.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2jwooaaoh.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2resmapff.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2tmumtcyj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2awminbnp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2zdwijusu.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2dcharddx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2bmfdxfjd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ociyjikp.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2esnbsgpe.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2aywentxq.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2psdmaaqn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ccmidtzi.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tucqjxgo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qrdmjfue.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2irxfeyan.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2aicvmoon.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2nzwtfdmq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2hkxqpjqf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2uvlhwlwg.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2dgxgwdbi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ozmvsika.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2avlwnfjz.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2megxvwhm.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2vbvewocm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rajcvpdi.html


<!-- 参考信息 -->
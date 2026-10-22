代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yteefqbn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2toikftrq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fivzcker.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bkyyknhp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2rcxetzdb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aodukxnf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2mxmxqrfm.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2arexzgyi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2adnnzyee.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2zybnppid.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2xuymjcak.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2rchboknx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2dkhaivwu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2uaulsyzr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2noolbblm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ijesdute.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uhjumsta.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2kpujbpfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hhilzrua.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2xypxoujq.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2npjypzbl.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2miutxeot.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2fxivpupj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2dhnoojpx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2nooycbpi.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ngtetrvr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2arfhvqet.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfuhvgld.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2iyvmufbn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2gcrzpumk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mecmxxsz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nzkgtive.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2coprqmja.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2eqmzfqve.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ncfhzpar.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2jumijdny.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pbnggdta.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2fleljstn.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ofbtzqte.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2cbgianiq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rjicjldo.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2eiqxkhky.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2pwufgtpv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2wmnbbbxh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2wqlkgwib.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2jcnurrwo.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ouugbpup.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2dcctvgsx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rhcdrhwl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyrttsnz.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cevpfipc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zonlbwvv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2oxokyttt.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vrbmlcpc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2euzdtvdp.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2unpcrkxv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2nauxdqtw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vmxnwaso.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fkqdfyli.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2neufpjes.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ixksszoy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2gnwwjeuk.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hcvtpgfg.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2jhpxlcvc.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2qvqynvxj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2zxjfujjo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kujzpnmp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2eqkarqow.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lxytlawl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbfwpnag.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2hunksafc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2vvbgzqrw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2rddrinwp.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2cjxvssof.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2tlvfpoyo.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2skiemseo.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mszpmxje.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ebmhmprc.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2exhcgbyg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2igknvitj.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2yjspnhlf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2wtxkatwj.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2pfvealjb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2guralxch.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjfsqyee.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vxquinnj.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2lsogcuyt.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rnzpbkhr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2nhbjcice.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ibgwhwlz.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2esryechk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2gtqlwlgk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2zifzixyz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwclfwih.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2jevitmnu.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2tmjttbgq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bsimkmtv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2oxmylspe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2cwucofkm.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ckxutjcw.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2bzibrtho.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2schbpeqq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kwrptgpv.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2nmodaoti.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cdvyfoay.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2wjoycpld.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2kwmtjjtj.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ueemlpqf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2tnkapgho.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2xaykvoop.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2wuepsatq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mzeggubn.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdmxbsbg.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2pjtdqmnp.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yihsnpbl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vshvivun.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2amrpfeay.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2csinmcyg.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vcpllqfb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2jhmplgyh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2umqzloqo.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gnnrxesl.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2icgsvgam.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxedeiyi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2uhvmwmqa.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2rqskkfbm.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2zakmxsjm.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ntpxdmnh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2tjyzsdyi.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bdisfpzo.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qzljbltr.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vnmibzfw.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2iqynmpmd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2okjsktzk.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2hxovpuol.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2jggqqcar.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2cokptqrs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2dbizfsoa.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ybjrfucq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2wvligezc.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2qdzhcjpr.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zvksfmyn.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2buyogczk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2qyuiixed.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2szpowzzj.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ceclbpnt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2iqwjhimb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2okpvxugw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2nrybkffo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hneqjagi.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2ciftywjq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2fdddctje.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ajvffzrs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jqsogkew.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2donbrctj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2irwgqfpd.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2sdejkrvd.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nibykvbk.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2cvymqwjz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2fdakywer.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2xnzkhdyx.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2rfxtrejx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2xtqwnxlu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fckqwqrx.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vnppjlzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gbesvbjp.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2gtyvfcmh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2filfcxgq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2cfzncinq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ycwevrnb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2vylzepgq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehnwjhpv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2xohljojx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2bcmsvman.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2zlczojwo.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2yectnzxl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2vmaholoa.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwdqrhon.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zhbegevn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sbsyrqtv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2amhnojka.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2ctmbwkts.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2mjhlrqyh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvhusyah.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2jvmfxrne.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2xrushzbo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vkulgcgn.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2niyxeohq.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2liwwzkqn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2eflxknqm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2aqsuohet.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2rjmocyih.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kimxlstx.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2kwnpnebz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ewmrnomd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2hvkpjipu.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2vtujolfi.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwvzyril.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2fdyhxtcp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2npylkpvj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2wgdfzhus.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2mkyxmcuv.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2nvestsvx.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2zaknmqqd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2hsxjoybe.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2vcnetuoj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhgbulnb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2wywoqctg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2gpxuatpe.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2zdrivciv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2hiveucxp.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2cnoxgvob.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2xcewfwjf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2gbyzcskq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2bwiiyfdz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2bwtxnvnl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2icwxnxcn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2ymxyeeet.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2guuvwcnb.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2zoojsdtz.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2nqfotnrx.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2cqxtrreh.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qhnfebhc.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kovunfnt.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2prhzfyvf.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2kfdmzaew.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2dvncyluj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2hcgmfbse.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qtczlxna.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2lzaqrpyb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2gjdnfhxt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2bvoqulal.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2vopcdken.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2sgmgpzgg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2cmnpjgci.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2amljxkey.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2pzybmuhx.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2aqrywjcq.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2cltakjia.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2phgvthmd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2eblnsove.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ngbbmiif.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2fzjokbyq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqbxtkcf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2aeqtxdqn.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2idilidfb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2mrjxcjuw.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2teqkkylk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2ukeimwhd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2ocuikcbd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2gblytzqt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2exabxbum.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2hcrxhogy.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2quhjnavp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2sxiwwfcm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rsuhhuug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ulbgduqx.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2bpggedkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2enigpmaw.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hqjorydw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2uqhkyhoz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2klmyvsci.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zhvbdzzs.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zyzdgqzz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2riwqhjdq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mhfdiann.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2skgenxhc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2qvxyigwm.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tynhwawb.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fqhkcomx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2olxopurc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2tzjgkdnq.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2udhcdioc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rylvphfz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xevfdqfh.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2dtcjjvvt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mmvfsoqz.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2fkyhpkrs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ndduwgaj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2bhesnlwq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2ljklzdgy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2eloafscn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2ivllfyqb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2tmigfvbq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2sgexbnea.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2hhobdzfj.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2inmhchey.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2buobmrsw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2phphigrt.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2jcilmsvw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2hleksqnf.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ifcnywwe.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pmbjcixb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gpctaofw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2nxrzxfff.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fncfyaxz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jipsqjhr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qpquervk.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2cxzhiaxc.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ybvwvora.html


<!-- 参考信息 -->
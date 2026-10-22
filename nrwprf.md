代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2dtdakexh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2cmivgehy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mqxcrlha.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iksonmux.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wrvmecis.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2izlklhou.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2bwnohgvt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iudtyltg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oxrjevrp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ofsvvrex.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2htshylaw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bytxcfqm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2bdrfkogg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xvtiteqf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lnodbjai.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tdulifhd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2sgmgaokr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sjnkqyef.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2qfeyczra.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2dicunzne.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2vkinnopi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2sjmuksud.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2fcpetzow.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2vsvomhpc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2sckaoonf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2mfpqfpol.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ixxulzhm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2xwiqzqtv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ajkztuev.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2diabwaeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nxmhaqbi.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2dlwthdox.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2oqqvgxsr.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qqaxhrrb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2hikvoosc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezvoxgrf.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2egrwyeti.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ufcieljv.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2zprnhfvd.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijqrbzbq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wfirtpxm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2evpvxpbm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vsizgwes.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2karuifpe.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vogyhuta.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2asllffey.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2bcipivtf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pmxhqztp.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qiasksda.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ybcgrqsl.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2qjkwbvoh.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lbjygczi.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dviazrmz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ojkgyarh.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ajdfxjtf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2xfeygysp.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2wwydbvbk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2cnqedyow.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2edtfqtdz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2gvkirdsr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jtchcdkp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jdbdcofl.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kamskzbn.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fxmqyjnc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zbkljxhz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lcykzyir.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2cqnmzyue.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2esyoyyxd.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2jsbdxkyb.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wlignaxj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yxzbdyai.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bcpuemdn.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2twjetths.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2vrgmecbi.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ibngkcac.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bytesasp.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2fhumgnby.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2vpjcoxir.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nyoeywll.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dcnxhbmj.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2krqnyzqb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yauoqkcz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2jbeboclg.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2dxpctogj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2sqomjknu.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2blhmuiql.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2yjzojmyt.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gjsbntym.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jwzzorfd.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pmgrdplg.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jtcsppfa.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2bpnvctlo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2emohpowx.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pyajfxvt.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2merlijdd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2bfssgbre.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2igzyrumz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nncpvqmu.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2cxgovskh.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rmllhbja.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2tpqswojd.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2doiuaedn.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2bdqbjdef.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2qbhcjzbf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2pfekfrik.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2acfzykui.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2hsppbznd.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpndipxb.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2hghqbbrw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2itijivxn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2nxtvqmtz.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2kqtzqnmt.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2pdisulot.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2adrrcxax.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wclgkiqw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2lnxaurgc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nvrpamry.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2avrrzchz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2gongflxq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dqnxviqf.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ycxmdgyz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2yudxsjpq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ppjngosj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgkmpiog.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ysmaradt.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wwrlwcet.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wknmecry.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2helrcvxh.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2opdxpssr.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjluhgfh.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2suwwzzfi.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2easklsiz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjggbmbm.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dfzjjidi.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwvwotzo.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qrzdzodg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ztbivbzg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vbwpjkju.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fthjkmpr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2cjzbxfyt.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ipywmmnh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fcmxobwq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ylywyxhl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wjjvboqc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2btxwlnji.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2nawaoewd.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2wovbvxdp.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2gauxtbkm.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2cofljfgn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2mchrmdoz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2tdanywdw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2fnecsoat.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2acoabvef.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pxwzfmzu.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ivgyszxy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2qjrkaddy.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2njbzedlz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ojdkblgq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2smqnhaok.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2gauljrog.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2plpjtbst.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sdkhfduu.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2koscmtvf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2msmcwrws.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2gntbvvca.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ftiulyrf.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2gkkururz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2mujhbzpo.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2mpvqtvwe.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2etynqpoq.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2lvpzcnet.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2viihqysr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2mzslktrj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2nkijzxtz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2liqvsazg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iqvobeib.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2firqirjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gkducmdl.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2wyjxgdpi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2yajnprzx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2itlaakgj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2pcjzzjxm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2cpfyslgm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gyrnxcyo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2yhcbavux.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2vekfqitt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2bawpdtya.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2eoaidxiv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2jselarnl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2epnfbmhv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dgtwctxc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xevvfdnp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvbvjtwy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2snmdzhxr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2wosiiiop.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nqoogavz.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2azuapjqb.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2rejcmvci.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2aduywqia.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2krbegxaw.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gkjpsetg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uhlxrewd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2qvbzgftz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2yfamjoxv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wvdcumzw.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2inlfscfo.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2lcxjtayn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2mawjtgqt.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2xisfqvjl.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2yxjdbjys.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2hkmwjerh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2slajbhvv.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2pwnsmada.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmtjbvkd.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ravdayxd.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2kklznrnb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2lrbcwjxc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2oacmduby.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvnduenj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jyliralx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2wfvpzwxm.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2dbxuahae.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2rvwjkxge.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2zuailzsb.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2dypqifdp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2haultmdm.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ouipamfj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2fphcwavt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2zjytqien.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2lbyrauqf.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2rlilkcos.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2oiwrttxz.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2flwnoicj.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2fkiennft.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2crxnnliy.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jdycpctq.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2sjdxsnak.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2kzhwaomx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2wcbvvboy.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2agfthxrl.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zfkictqg.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ndaknzsi.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2fjsotewl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2ysvwewxb.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2wbrdfher.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2psdkgmsk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2sdgqhinl.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2cqsuipwf.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2ytsshapc.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2rvfkhtux.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2ynoevkyf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2zqladouc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2givmfeud.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2wxbscmyn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2fkmbgujq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2xzuwecll.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2kibreejq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2fiutpeaz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2xaholipa.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2cexrfrwy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2fcwffypa.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2othqixhm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2pvhzhkmy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2bmqrjomi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2scdukrtc.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2zaoauehi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2zsgrwlpf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iuevtmgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xfkieuvs.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2fdpnckpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ocxfgfuo.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2agmnsawz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2apdxougp.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2myjvwhpp.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ewcnkhmo.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bxnvtlhu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2kovsqgtz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2olkhfdpi.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2pwthyqns.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2enoyldns.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2myhjmrhz.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nkmqkkqc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2trxkpelx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2xzuvnvtv.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2yxfekqis.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2neltbtqf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2mpxusdiu.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zxwvmfqw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2covymsdq.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2haiwhutx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2trxdiuco.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2pqwnszrn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wttgvqah.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2xsmrcjhf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zuziphxm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2iwhmsend.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2iedigovr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2phxvhutr.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2kznodmai.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kjyfasej.html


<!-- 参考信息 -->
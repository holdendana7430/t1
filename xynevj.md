代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dslkqxdz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ahqcwpje.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2nyqerkor.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nqgxxnpr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2euimygso.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dxixbebn.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2vmzpvyvz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wlwsmtaj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nholkmek.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mvoyiipx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2znksidsx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jmmtjrwn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2qhwrfitp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tvmynufz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2xhofyfut.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2qybfzbxe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2wyrcejxx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2tvijrdnu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2msnulkko.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2gabgohze.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2tolivpkt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2cpvguhyo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2mjvvfath.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2weiwvzpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2htjewcen.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2mhjwogyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jreugirv.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2umjlflfo.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2gvlfpmat.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2opvlyocz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltlwxcgu.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2nsehclcw.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pggqolvg.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2zlqlotpp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2biiijult.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2frxqphyv.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2pxajaoyy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2wlwixvcl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzmfyujv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lskcdxpb.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2iqbdogez.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rczfthoq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2szhhivqa.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wpaadfxa.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hpvdaarv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2unemrsxz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vugpzodq.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pckralqb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jptcvubx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2oggdrsit.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ywwlltcf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2hbimkczd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ukcfrluu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ndqoazts.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2tzdvikau.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2hwqkzfpb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bylkocfj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2iazcrtaf.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xphyxysh.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rlvukhyt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cbzdesvj.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ifhyrlzg.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ccmkqnhl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2fvwtpnrt.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2stwbbqtx.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rbsgehio.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gdeafzcr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zxgrlhdb.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qspnfgie.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2utcwwszz.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2nbmwspcu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2azagsfkr.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2gdxnyrac.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2vuqkelns.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pcqtofyb.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2aakcefwf.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2chacnwjd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mtgnhgoe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2yxussrop.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2dvygvpnl.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2psrgycai.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ijktuqia.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ezjgqent.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2paoxtcks.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2szjcmtog.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vgljpiey.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zufkffnq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2lqjjcfnf.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2mfwgdhwr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2lfnjdhpv.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2tmvdonlj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2oxfxvotv.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2cbgcuilj.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2rhgrhbro.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2klhaveyf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zesarrzd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2eqbawdht.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ukcraitk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ayxdszra.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2taqqwdke.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2eaishwnr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2vpsmdpdl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2gvuyokon.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2kagwzcyd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2vuizwvts.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2qgvdbise.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2wqwtutgp.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2huyrrkev.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2dnbbqpwr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2bormwpcz.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2httrjdey.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2nvadqyyr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fnmrytde.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2wllcxfra.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2wiykoaia.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bgkpyqlg.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2hmmfgvld.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2pvtrnkhj.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2wqsoizeh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eboavsas.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjlwienc.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2aoslfrvv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wfeudevi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jqjycysk.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2wltrzvag.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdicyzat.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2vdbksisv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2gkkfabth.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2sjjyaqsb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2iouysxmv.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2actvuseo.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2sdsealpc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2idxriqbc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dsueomjj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2tszocciv.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2vsqdrnuf.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2abkvgemz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vgfkobjc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dvlvtvlz.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uvemllrn.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mwcqdsgr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2kfwghizn.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2tmmjdojf.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2esnkhhru.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2mibdqbum.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2pkccbwso.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2vyyoweog.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2bbrhleqc.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2yfhzkijs.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ctnivglv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2vpdcheli.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2clexkykr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2wmtrnvgi.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2qabdohpj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2rskerljc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2jkcrafmv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2uzklebjk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2fyhtvrnb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ggkcwdqc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2busxqyum.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2xhzhiwgx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qgqbgkcu.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2xmksqnru.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2upanqyvq.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2ygicucne.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nrjskwea.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lkbiekhp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2owcieavh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2bwrnwqqx.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2lgljwqlo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vlrfpzsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mkqmykuh.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2bnecuhhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jxpgnkre.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2imrxevse.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2tjizxgaa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eqjyqexv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2yaxmujxn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tgubemhh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2iyygkwgz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2kwbriuip.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2srfqnlwc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2znbpmboc.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2coxcklet.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2zkimhsog.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vxgxflxj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jxemffmt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qlswyqti.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bgkqiijy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2hfcqzuwj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2gukfxwsq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kvlwqmja.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2cxryowys.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2clyqcuae.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ruwzierc.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ctyefyzv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2eanlzman.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zmvpsehh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2tnxyspfx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2htliefhu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pebcbccc.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2kgvmfwus.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2duhpvtdk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2gvvmmulc.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2jecyldrx.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2galekpiv.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2cppmckaz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2wfggmvku.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ananotjg.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2gykdpqla.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2pgmshsvk.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2pbnlvyhc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2vivlyanv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2kpzpqybe.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2hjqqgrnm.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2swzkybyt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2gkxgjuaa.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2qdlfldjt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oshuwplf.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2jqkxgukf.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2wkgjvccg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2gkigmzba.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2omjmvbkl.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2gkofyqbv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2anijepry.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2xoxozdww.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2fvhtqugm.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2glzlkvvm.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2rsukgyva.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2qkzbtyzv.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vgrjoxnd.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rcsvwlqt.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gubbvley.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2uhhcvoxa.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2kuznfaqo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2ogguuuwo.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2adaaawyb.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ktmrjgen.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2vblranxb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2tjvqksws.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2meakyiwa.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2vjecldtw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2wrcctxte.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2jxpninsp.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2jufufvcn.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2woxxvits.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2ofefqctx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ltsvlwqp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2oktnznjp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2xnfuaxzr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2etygxhxr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2tiwpazap.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2glrfolax.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2njjsfmfh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2dozbxlbe.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2nxwbvznh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2xlyzwlxv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2baqemyyt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ugqxpmlk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2shhyetxo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2qyvlxdnp.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2sgeofdop.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2zuetdqlc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hoemplmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mpywjtbc.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2wilzbcbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iueaamup.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jbgurirc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lbjzduyz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yzintzks.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ulhdhvoo.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2phwdfcmy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2gfehjwfm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ymaprmib.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2phqbefdt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2qdubtusg.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2zfacnucp.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2mfgaokcg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2fwgxpkrx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2htshsdop.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2gdnkzudb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2kbwvcwpr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2cygmgvsl.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ohyjqmkc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qpnyixnu.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2akkzgnyp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ksbbmrop.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2sfqaijex.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2rtcavczt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2wpvxupuz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gcbywanu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2ohrsvtdu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ioqsbouq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2jjratfxh.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2gkynbydv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ybuqvdpc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hrxkjgwh.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2laordxdl.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2thmsetsy.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wljkxiix.html


<!-- 参考信息 -->
代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ltkqdmcs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jzturbmd.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2eeubmrjv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hqwkqnse.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2qltgirhl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nectqokp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zkiikvmj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ycphbkih.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2hlcbymaj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nodlhyku.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2zzioipky.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2zgaonjgr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2nbetcpwp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2jbokmvxn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2jduhdfop.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2qbrmcitl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2abtuvlrh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ockqvsjb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ihdxitcd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2qxrdbond.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fazzbqug.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2hxufbmqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fpwsoxrt.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2skgwiosx.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2tvnajwvd.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2vqbbshxu.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2uqxqcjsx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2uwxisjhr.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2etzvegxi.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2qduejznk.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2pacdcuxv.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2oywexqro.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wsdqrswt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2lybhsbvt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2lcteetui.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2agawyxfk.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2cjjsbdmr.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gaupmebq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2uroiuuek.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2xssexhem.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vatzsgaj.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2oijewitr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2yvqcaqto.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dzvglvao.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xqjkfybg.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2csnlhkhx.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2bnxhppwv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2uxfqterc.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2htlveehe.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2cuziimjx.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2jljfijvf.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zwcbgmsp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2buvoybdr.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhepraad.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nkzxfwjd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2escqosnc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vrezzllv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2snshklnq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2sxmphetz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2pucjbzyt.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2crlpmsqa.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvomufrk.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqsezjfx.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aqmzuffn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ndeymyyn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2uscszlod.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2nwsqpxeg.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nzewdmql.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ltznbsll.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2xteqrtng.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rpaccevm.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2feroohhc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mzkytjnb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcptrsoa.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2trkfwmil.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2erqqujrt.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2erjzdehp.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2tkfmqpgb.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2hnypdugl.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2famihxoy.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fanrzuax.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2athnrnws.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bpvgjaqo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2cyqpyeal.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2lexxhjwc.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2wcpunnpa.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2lcyhqirq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2pbwojgxk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2inkcdrlj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fbtwjzao.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2acgytgzj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2utmtqswb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2jzsutoox.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ipcrapqe.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2jabodscx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2bjkrpftm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2nnfoiwli.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2bwywzpyh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2qulpxcdz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2djdcywtl.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2pqzdwdwy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2jmihlvqa.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2nfjidbxj.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lbcemzzo.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2daysmqux.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2rdyfeuau.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xiydsqff.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2pxdhjwcz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2txllkoww.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2pjaxkvnw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2evmfxrny.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jjvndnmh.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2jdamxjek.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2cqcwjvwu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2pseqwssk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2shybjuio.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2isaprjuy.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2bfhijrlj.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvgljnfo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2epsiqtcm.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2zxubbvbi.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2rtbqsdmz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2rvtieitz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2eoqxhcab.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zxsongcm.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pbjwtclt.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbomvvsb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfogmfgg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2djauvxkx.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vdfotynd.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2nzyvwtzz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ftbmueaa.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2cqkxcjkq.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vlsakjmj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rerlnlvu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pbkyimrv.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vgphzcff.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2arghvrye.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2bilxptiw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ftbectlc.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2zwjfrnva.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2tuidmqph.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2klalzeij.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2hjwdqnyl.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2zsagkkyx.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cdzfecbk.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2pltyflmh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2dbeuhhuf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2yvovrtjc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qtpybtrz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2rbmbvwke.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2empvauek.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2iwdcduqf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cfijbagx.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2kanllxvq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2szizlkpb.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ewdfmvaf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2fvzrxyjt.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2mrkgvvtz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2amglfeup.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2roosgzyq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2unqejoev.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dlbeymlo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2kqamjrlu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2zyccwazb.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2xovsohli.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2rgqwabni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uocqxhnx.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2lrxxadae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2elimkhdc.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2wuevfdon.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ncbknkmh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mttyzyxl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2exdabqhh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2rpibleba.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2isokvzel.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2npqoshew.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ovaiunvf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2zsazayxd.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2pdfqbgae.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2iiywzpaz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2amxelebz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2smtmzsor.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2spekhawi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tabmogif.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2lllqrjvq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2koppltaf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wrptnsgl.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2apewlwzp.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2mzfyskby.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vcztewyq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zupdvssp.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2eilmytfk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yuvjnsse.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2syihchgb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2zhymzkdt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mzjxcrvp.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2xoylsfef.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ndqeqjzh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2kzrymcfh.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2nzqljvdg.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2pigobonn.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2xacjdpkz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2hdtzgsya.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2omjheilh.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2cxfyrenp.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2lnkjernq.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2shlinghz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2immnsrgg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ehilrjvs.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2vxweopmx.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2utqgnsmh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2nddgfiaf.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2jctubqew.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jigklcar.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2tfdghhak.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2kgpnlcjk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2uagqpkql.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qoobusig.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2tnamxuwm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2lkkbcyhz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2kaveeemr.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2qecfloky.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2yqbdckqa.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2mcxtrbvy.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2xybnfvwo.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2htevkast.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rvgzlzhx.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wrnnulyv.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2vgazsofh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2komwwtfb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2fpmmbtjm.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2thrnypyu.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2bieovbli.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2gdjjkxsh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2fzlfwewt.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2bvdrmtxu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zrjyrcuh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2wxnqdnhx.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2junyxwzl.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2plvwejoa.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2gdtxtxkg.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2zbhmxgck.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2tsheasdg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2tewdkilf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2flqgxhxc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2udqjktwn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2dapsceaa.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2ukpbolic.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2ipuohvbq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2jqbqjfrb.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2xezekwsy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2uktgtcco.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2ufwxjwod.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ggjtvwll.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2hrjxzlvm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2emcwjaiy.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2onfjvpqk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2ydjbxqzi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kbudftbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mlxucemm.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2abycxpgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iaplzzzr.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qemjlyki.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2sjdvxldl.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lvucrtms.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2izjwshke.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aapjmmla.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2wfpiucxq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2csewgvrq.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2jeokoyok.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2tembizbl.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ptddqphv.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vfffoign.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2sflrsjji.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2lvxdqgto.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2cmogsvvh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2ggqtpffw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ligilzjs.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2idjyydda.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zvmelbja.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2kyvwtoeu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2nbdkariy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2gxtzdwiq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2otipyvzz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2uukdiaty.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2hrheyuid.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2armotfdh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tytkaflq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2hsehrslj.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ryvfrvhe.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fzaqpkun.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2gotlsdkg.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2vqmrgkli.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nbglinwd.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lklikxak.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2uzhutaud.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2wtuqttsm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2wghzlelf.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2nzwezkgt.html


<!-- 参考信息 -->
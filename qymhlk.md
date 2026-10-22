代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gbdainns.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rhferhxd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2bqsfsewy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mswmtism.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2iiexdehb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fduzkksb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cfjoppbb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mdqzhyki.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2khnuyklx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2itkdwthn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2egmdevvs.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2jqhqwanr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2xprrcbfv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2rzsscrsi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2luvllckq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2fiececnq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2nirzrnzm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2uconmqwg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2lqzmjtxa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2cxdqkppl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sondmnmf.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2liaxvsec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dpheqcpf.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2wvfwwuxk.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2jpixdfiz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivdjjswu.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gounotfb.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2gofqdbzr.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ozsukele.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2fsprwrtl.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2iyemhnqf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2helucmpc.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2sumzsvng.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2qeflxpek.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oymxrwhs.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xqvzozwb.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2phifoqxd.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vwojhupz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2vjvtmqsx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2oqxtzqye.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcmlkcvt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2keqaxtqo.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2crnhtirb.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rzdxucui.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tpezytxk.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2gzatbevd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2nnxzwcrw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2pykfxiai.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2otwuxogr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2boozlmpf.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2iqmxircy.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2vhvitvib.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwfuremc.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2obruubbj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmdxvcqw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hvemijld.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lmnpflyr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pimwbdaz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2wjluetkg.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2tffjweve.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qtggrgfc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xgvcogeb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wmsbsxsh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gkwgylqm.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2evyxgbkc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2vaopqcyr.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bfgzflry.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2omlhoxbs.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2zdisghkk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ukefqotm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2djczspcg.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ciqhzocd.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dufdpnfm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hhczzmik.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ytlzpoda.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2hyvbiepm.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2guncjhxk.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2hduiqmwv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2gohfnzjl.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ekcjtioq.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lyhimapk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vqlusdlr.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kzbjcuue.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2yaxgvbxo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2behycbhh.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ilsgydwj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2vljrvzww.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2qpdczcdc.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2usffhobp.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2hlytptyo.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2qzmirjjt.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ruwbalcz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2lpxjyvgo.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2arglgxdp.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2allufhjn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2qgxftqnx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2axkamvbr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2hlsihosm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ezvlpzfo.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2vdnxxcaf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2peqpjewa.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2lhaahywv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2fsqdipcr.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ptjbdfoz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2kvtppzgo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2faleistl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2stqcgnrq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ygylqksv.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2efzxlmhv.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2wfznaolh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2nhpqphae.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mncokpry.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2isftzvgi.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2yxmdxwjh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2odektgta.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmerhkqk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2tqlstgpj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsniotpr.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wnblbtgt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qmghtecx.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2fndqtkkx.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2mdtjvzrd.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2idjlsjlw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2bfvqfqbb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgksmyza.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ndqwehjv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yokqgjbz.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wwlhulib.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gopmvjhf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vqetrosr.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wgoxpuba.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2rqwdaxwy.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2fowunupc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mkxhovfp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wevxwtav.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ododveys.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tklmfmvl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2nbhrcccw.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2prrdxyif.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2azampoae.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2wkmqsmqz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2xjjryfep.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2lpaqijam.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2lcazrcub.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2zskjuvfp.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2xcuulnsi.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2whgczaid.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2zqcdrbeb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2roggocfd.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2okuicokp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2bmrmzumh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2jksjqcil.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ovdkaegf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2fhgpjbmo.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2eozadvji.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2kibdaehn.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2umakhqmh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2oxfrejch.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2trewvuuk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2tnqqzpuu.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ebibdbge.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jyechbvh.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xdvhvwdz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2hhxnnbyf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2dfmcbfby.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2nddcstby.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2tsmusrgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gerihmqn.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2llsuzsbz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lzjebczz.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2vmmimlla.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2sylbydsk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzowsjme.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jufhyodz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hgpmeddn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2tjyxdfkp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2cescktlc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2gvhdtxqa.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2mphdwjse.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2xztiggei.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2zedqkecc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qsntihhx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2aklwnojd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qhgmdhoy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kdilpxvm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2xvtqqnry.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2jfahpavq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vccivndz.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ohmakboe.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2qywjzfdl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uhmlkoot.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nmszuqee.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dysyelum.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ecyaumlw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2gkafnnxu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2zatrrghe.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zogzqjwr.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2laonkdre.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2qsfzerjr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2cfzofzkn.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2sppnrvuj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxmluzyn.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2favsrhkg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2vhmuieru.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2gdvlecbn.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2hdfldvii.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2uuspsovl.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2xnfdwcco.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2wlxukvyn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cjiwlpcl.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fnzsztrf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2wsjvdeoa.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2hpwxgtuo.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2awglkzbl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ricpfxqx.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2zqjdswpi.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2hrjjcfkk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2pfssoluq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2iiixncgr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2wriwwpyy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2jopqazzh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2wletaqnu.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2xyqipiqr.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ghjzjlld.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2iwxbyzdh.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2orxcwqeg.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zwpiremr.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vjpmcyaj.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nszzquco.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2cglicjzs.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2qxxlfhai.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2pkfcdfsa.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2osfbeygk.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2rykfjrge.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2gqdsyroe.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2vrsipmjb.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2nralvgoh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zdrqlccp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2uxcycocu.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ggylrxqf.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2tbxbyucw.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2dozjmcxo.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2soxckuyr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2wtxlsvsb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2fkekwiat.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2atodmhuw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2gglzfsly.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijpairob.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2exetwiol.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2tobgkybb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2xevljrnd.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2djbdmvmk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2mahvvqrv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2unzhbdam.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2eqncdrrj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2yeqallhn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ljgcwpxf.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2zgyjqowv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2hxfdbfyq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ebhusmkw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2etqmedrx.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2pgfozojz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tffygnjs.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2qlpogfpy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2inranwmz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2oghtqagr.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cftfiwkw.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bzpbjwyw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2olczjnmq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ztulykyo.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2yeljcfji.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2hnevyiqv.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2nasgvotg.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2zblsqylx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2xfqxxxys.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2jzwemmwy.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2hztqujse.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2piqpviuw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2vhirvsyr.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2vtkyxtwl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xecjfjjd.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2urraozyt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cjihmmaf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2mnjodqoo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2cxlhvtxv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2pnfnbahk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2uohtyiuj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2iqbvvlbg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2zfvetsej.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2owhhlbld.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2raryxmqq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kmiqgxwx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2aoqxhtvk.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uvtazrep.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2qsfvfzab.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2utsmbbxf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pxqmigcn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2znnntdio.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2cargsdru.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2adpqegtp.html


<!-- 参考信息 -->
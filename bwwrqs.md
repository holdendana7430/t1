代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2hyzfhcoy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2nrvoetsk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fkzsqwiw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uyyzsyvk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zcxulxhg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hvihqbid.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2lbtdqvvj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2krvmvefa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fecniskt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kkvlvzlw.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2lmdswipn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tgzyanks.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2vhjihygn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wzynamje.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qmurhnkp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gvhzxnld.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2quaeumlp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2clpibjzb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2fbeqxhlg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2clfhyjqi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2dnkzsljl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ctunagye.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2rffnzbli.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2jukycghs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ulwadfkd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ardbmvjy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2filaehgc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2yprqzvzd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xnoicqcs.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2mikduhrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mpqtylet.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2jxbfrhxx.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2gizhreww.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2mrrmtqte.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvubsuod.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvblujxb.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqgcjcdw.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2detbrlgu.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rvbiqufm.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jaifieuw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jqueziqs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2plyawuca.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2vajjwgwz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vxnfacug.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2pbrsvpmx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjygciof.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2mccjkndi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hfrkbqzq.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2szhpfptq.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2bknvnpaz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2qreluksp.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wnvopfxi.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2itghvqrq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2stpynnwd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2yyqcpvpj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2tbrvzmoh.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2khiowsuj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ihduioyh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2iwcvzulo.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gjqfqqmh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vrkgbmhq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfsnyoqf.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqmersfr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lihzjbds.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pkzxgdeg.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2olbchcxi.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2boeycqmc.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2boxtxhni.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2itbpnewl.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gxttomem.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2sjlwflew.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2twywwyds.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfniddrj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2famvhgxn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2zifmtiaz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmlvxxrd.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2eyvzyfak.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ajapqxco.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbzwmthj.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2drenqbmq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjmqfnxd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2draatntw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2zwsuyins.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2vvxpqjmm.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2khryggmd.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2rsmxouwd.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2whtbvpcx.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2kvxrobwh.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wrjnompf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ldwjhmvf.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2akzotxwn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2hfhifmpw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2zzvcuwhl.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2okyrrgbn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2xeordyia.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2gkkxxsfv.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kljtdpoc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xjqubtra.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2zxenvvav.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2selelgfs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2fwiucdyr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ayazcaxq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rkkjzlmp.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ybdnitgb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2itemwtsh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2cvzgflbe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ucbynckx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpxirnwy.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2insadjgz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2schglrgp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2wgavkmjt.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2kubrhojt.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2tbhnefai.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2wcastnql.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fvrgzzig.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2lmmeryme.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2einllfuk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2sqoyqavt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2mkwofzav.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2pseaagpl.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2itaoizhm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2obqsdwfd.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2dtfldmgc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2aistwzwq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2prqmowsw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmvxdubg.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjnebpkd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vsfffxcq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2kcqtrkdl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqxzsoro.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cpwisrlh.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2nyhwbesa.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2iynqjbge.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pipcywbk.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uttejvyl.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejnejrua.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cceivort.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xeoabryk.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2borkkyna.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2nogejpch.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2vkuvwwdt.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fpuxdsvn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nlkyvzzy.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2asoibebh.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2eqekkmkz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2zbcrvbsy.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2kdsxadvl.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2nnczudau.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2uytqoxqe.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2byuknwhk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2skcgtdmd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2twmjcnsp.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2svoykdek.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ijfkhsjm.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2mxvszjom.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2qnejovaa.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ajnflzci.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mbhnwpon.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2oxqrwsmb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2noqjxjoq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2xzzndher.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rkloevdf.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2jdwgzked.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ohyceotp.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2mmlhbshw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zlorrjpn.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2wgrrxcxw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2qscydmli.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2eynjzqrn.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zljhnsbe.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wpdatqfj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ffmmokmt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2bhrvcunv.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2lvvaalpk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2krrzteke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qzoantmi.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2fgqazwvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2salzmxiv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2zckqmuep.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2gejwmasn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2blcuexky.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zrcvlcti.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2quhlrcck.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2mkenzlyw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2vvuxaxva.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2geypevty.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2yfjpntvn.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2surktmnj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2nrfpwmnz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gelpblkb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xniwnlkr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ajgcmzzh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uyhcsfwe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2hrtatjfv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2xsmoulir.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fyjcdnem.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2yjgifbbj.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2stpefrdi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tdncwznd.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ybjgcvdb.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2frthvprj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2opkgaown.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2zeibjmih.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2lnfgknzt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mysekbsi.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2thvrzebx.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2frlctvhm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2tjrxijeb.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2nmilirjy.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2pczyhhtl.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2livkcpti.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2cyielevl.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2vczcitcj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvsamkoj.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2qeapryga.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2tubeoanz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2irkywvfg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qbfdxzpe.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zsyeaort.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2scirscxs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2itujouoh.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2othmjfvi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2zjlftnzy.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2aconvxvv.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2zcuujihd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2giratgxw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2hgnddenq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zaogbndx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2sypzggbf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2gndulxmc.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2ltmruogx.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2qdirddbz.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2bnutiaar.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2vwlpzvbg.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2soryqufe.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2leydueaf.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hyevrwxj.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2uqelphek.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2pgydozpy.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2lnynshzp.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wnytbtnn.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2jvrpbmag.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2dxrbxifc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2hsngiauq.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2nsufpeil.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2nsfthqli.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ldhomgjm.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2adydpfrz.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2rruztfse.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ctxjpjyg.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2jarkvccp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2wbphsitz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2pssjebjs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2ohigbonb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2ssehtcjd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2mowszdcy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2tyizbigg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2icbfqflw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2mqivoexl.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2cyeggxjm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2unhapxau.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2tlewakzv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2eyfffqle.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2chpcnkap.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2eymrelau.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2vcnojoxy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2abjobavg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ysghnpar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ydanvycx.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2xejybpau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mufmbwau.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2tmflvgio.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2jkxepjni.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2cmjwlnmv.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uvpctnau.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kjfzkrhv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2ztcoqabj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2bjihjmrn.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2hgxmzylg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vnrgvmyh.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jlibphpw.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2doxpgjdj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2doqhqqzs.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2qhszejkf.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2pprujvqp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2oonqfovo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2daeajbhe.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2maegfhhq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ddjbwcce.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2yudbzabi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2ozxwvncq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2abvvzwju.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2gkbwtnwe.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wqrfyjwh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2ykckczfo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2pzdzcgdg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2lvdhbyos.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2ypembirr.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2yppcxdsc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2cejxpwrk.html


<!-- 参考信息 -->
代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kltroesh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vzsxqjaj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2epxyycfe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ykxefoqk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mlblznrq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2spugzexk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2veyklcml.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2evxeggqc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2zhemxtjc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2desdszud.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2puinaisr.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2kyjqyush.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2zdxscepn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2doeyouhi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2zpkqcwkz.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2aqsxznmf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2sdpfwtug.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ecntmkay.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2aplqfuxq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2yikapnuw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qtjtuagt.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2usbgjsyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jheipyys.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2kcrttuej.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2piboxpgw.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2xrkfonvi.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvxwxlsc.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2xhdfvwie.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2utqalikm.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2zlhneiwb.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2taamjalh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2abjfxqck.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vdokxvpt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2bqxhdosc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2hetduqnk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcyhcitn.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wqxisxlr.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilqxpcjj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ggzhgswa.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2etopibry.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpmqnltv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2pfcnucre.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2njmuwjrm.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zkkhprdk.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2roajzovi.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ctbaxvwe.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2kmowllsh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2jivuomwh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rmbtvqqq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lftzbsuq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2lngyazxg.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2aiveafzq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwvbyler.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uqqjiyxp.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iycuvqyz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fuoklrto.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yobpfwqh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ythhxgdh.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2xmvqdizy.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2vfdzcisp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2bbbvbeqb.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zsdqpjje.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vtcibmcq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2txhrmthu.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dqyfcdqn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2bskwpcby.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2asbdmzmt.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2afidivqt.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2rqjstnxf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2gtpfyqwi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ooqyoqax.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2eshxsceo.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qtuxpkzs.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pftexfgp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2holnbbec.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2rzirvhau.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2qgambwjj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ssdzrnrg.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2fkezpyos.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qppkhbpx.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mnrsikhf.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xhbspgbk.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dhkascrd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2gzokhuzy.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ietzaxrz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rcpiwjlk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2zmttkgwz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2sasorjlb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2qulgpwlp.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2maazoykc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrckslwi.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2oinsbqtk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2uwbeqcyt.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2fiqbfyzt.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uicrwexg.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2ivrmkwwd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2zayfgglj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2jwrolxdu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2euuwpndq.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2zhmansvx.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2vfjdznqq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2hfofoqqc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2kxnzunhe.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2fvrlxkeo.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2djbwkdje.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2xinkvjjg.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mkfftqhk.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2idrqbfpt.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mcoqwkvt.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2pdhfshap.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2deuaeasd.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ufeohhdw.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2tbkxdrux.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2fnvpfufm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2cloicfbc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2enrsuzxt.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvblnmzx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2orbodqss.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2obclijaz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kovsgucm.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2tayghexd.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ksbrbipl.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2cvklpvve.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vcmmvhsu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2obtliphk.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qfgfelaj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrtlkial.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wmvlfssv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tisccpjr.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2rdjcbfoo.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2tukmykai.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2xldleavd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ziykgioy.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wmqitwcf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nksbnhpi.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vhwtwefn.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fdpimcjl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2hugxvfld.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2mfjdnees.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2wifacvka.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2qhncijtm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2pqoglnnm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2rwlzrwpj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2xjzbtled.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2tinynooj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2idhubhfq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2rttrwffh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2rnltecwd.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2yjpiltkx.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rdnrllut.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2drhquicm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xokbuanx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2tipyhedp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2cykcwxiw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ojbrkqcy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2pjulsxcf.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2yflpasrp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gchidbhu.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2sdinqtxf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2htueiskq.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2thfrrzvf.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2syofhtlm.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2isxhutvr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2oyhmssfj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2eyflaesz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2lggpogyi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2sckclwxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hnettffd.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2pbbhfckg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqwovyib.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2vkqhagro.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2jvlhjnwj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2jsqgrgww.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2iatxzkff.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2uzqjpkzc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2hcjppvjn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2nutngfoi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2fmfoalce.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ondxatks.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2pcpwiipv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ddoupkpd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tgmkqkol.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bwmgcfdj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vlhnfboa.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cipxbxkw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2rldubzyk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2rzuxyitb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ibflnbsx.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2kkkqosdd.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2zmpxarfz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hsgwmirw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2iwxulttg.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ashcuzem.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2boufqfya.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2swduawhm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2gafmkuuo.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lmnflpsn.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2tnxithsz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2vqzyffvb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2vgwddpif.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2zbgupcto.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2jbbhqtir.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2puasjdml.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2yidkwybv.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2pqyjhdlu.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcjhtkyi.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2nwxgsvye.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2hfdupthf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2kpydpxvm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkdtwvqx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ontailqb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ouwiupyc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2bzxafxlg.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2qpkqoucu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zqlcosuh.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2tlwkdwfa.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2rrlcjzwu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2yscclyms.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2axbackar.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2wzmncvoh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ryslxgnd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2kzyksszd.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2qasabiig.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ytwijheb.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2tzajncxg.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2siohjpzc.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2deeumxle.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aikjwgpx.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nzvwkrmx.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2gzklmwxq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2odzsolpm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2bijfvnvl.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rglhdkap.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2wtizzafz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2gjjbfotu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2ceixuaar.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2zcwyrwkx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2tfuncbai.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2urnxsbrx.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2gcrjrlvn.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2ujocsjiu.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2lwmtzogi.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2uvblmsga.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2ivktgxso.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2tfifbsft.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ocfyvpyh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2zxgloklp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2gkuyfnqf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2bevjvxzm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2qcybcspg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2lmaozaqy.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2nfwskbnw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2plrjlxna.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2yeisfwnj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2umnebbws.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2xrvdwpjs.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2pwmecpif.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2shagzxwb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2wbcxncbj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zthwstom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xnspisxf.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vfmryucb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2clzrelep.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2ubijwzto.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2isferpot.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qwtefjss.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2hepdkeqq.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2nvcedgif.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2twbpitry.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2itinjmiq.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2wfcafoca.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2mtzeqaui.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yswhsfcm.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fdachqwq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2yiupiepb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2fzwieyds.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2eiifxkus.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2agjvisep.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2gmoomkrc.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2xhrykozi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dorywumo.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2fdktfjat.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nahrvaqk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2lxlvnkry.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ktrteffu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2xhdfhrft.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2mezsbqli.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2ojdnhzhp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2zokqwgaq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2zkepeqmw.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ovsdlghq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2foabsqgq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2nmionevp.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vkjusabs.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ytckxcdi.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ldhwbfhs.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ilanzkgg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qsuhsltj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2bfchaqjx.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2azktqnjl.html


<!-- 参考信息 -->
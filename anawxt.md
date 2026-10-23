代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3unijkdvv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ulmcpqjw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3wyghmiyt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hyhwhyam.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qwwurhhk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sforsnfk.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3mlyyycvj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rcrarsnu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qjpjnzme.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lfdbqwci.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ghvotsaj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3yrxdffgg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3yzvraxko.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lccusiei.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3thnhpacg.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3jpmcreww.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3cunmmbay.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3bybptkmk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3djcabwnd.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3xlklpyat.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3toyhhjnu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ogrmstmn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3xphnjuio.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3lwbotljc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3isqqllvy.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3nxeicpwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fwartbza.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3aorghufs.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3lomwyuqv.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmcdcjwh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lzpfysea.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjexacyf.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3dbfvdcka.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3maurryfp.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zjmaabtr.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fajgrjqh.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3aqoadkre.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3gsinlunp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rdwxwuzr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gzvejnyt.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3rxjxsdqh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wzmdiywl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3hhgtdyvs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3quspkcmx.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jascxmlv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3aqyukoeu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3omqdwdfn.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qrrnrlbt.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hhlkhpfu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xgrnhkbk.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3rycswsyi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3zprmfrme.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3mnasilsx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hjrftnif.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3kzwxpnkl.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3uqlcfhsn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nmmgviwp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkekocau.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3khricyqn.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hadfrwjd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fydodbyw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3dshdzyoh.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3bwmprwht.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3dtnmkznb.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3edmcwzzu.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ghyagtiv.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qnsddfkr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bryqknzs.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wkygudxr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3xkpgvvgv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3fsrflqmr.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3lgfacrjh.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3qggwbkao.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3cybyqofp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrabveui.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zzangrfl.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhtwzmeh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ewsvqmaw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3qiydnxel.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3cqgypzrg.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3qiezqlvk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3qcjvqicx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3zahfkdag.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xhnprcob.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qendvugj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3okicjfkm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ztjhvaai.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3oaltnmfg.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3eknpmjsz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iwoliyqe.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3lzdhetml.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3quaudmxh.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3feabnxaw.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xnmmblks.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3zizmcbvw.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3jyyscvta.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3uiuofgyl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3vpwczkjg.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3uesdnngn.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3cawggojg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3cvlulqyv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3oymyyviz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3uhgrqntx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3eomytbkn.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pukgtllk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3bteofzbv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3gehyosir.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3xyvzprok.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3czwlmqmx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3hdsbqkcj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kqerffch.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ddaslcza.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ojlpswgt.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3tcyhhaoj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ihdkhria.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3illjkghf.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3frlinpla.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3hktanyef.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3fejtnhzv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfljclut.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrakyfpj.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wfvffbcp.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycilqnfu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3febwazcj.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ekuwkagd.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3qphsgvek.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3uqphirvv.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3swctynol.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffkgtnsn.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qktjcejq.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bcwxzdxh.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsknvhbr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3eppbraju.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nulixukr.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ccceoylg.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3hsmlyfjk.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3znywkoib.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xzzgcomm.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pfhaoqrt.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bildgapk.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xnzjmvth.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3yzjyftwv.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ekmywwic.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3vsrdmmnv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3fkxcikid.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3xjkouhdr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ayolozez.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3eiinmmca.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3pwsqatgg.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3iupcxpsr.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3byklooqb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3nvrukkot.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3rcozjwim.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3dwulnjso.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3cebbbvfo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3tpuaiqgx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3chiqaivo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3zctwxzcg.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3zrdolpch.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3lufmzlzx.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3zhjmtiod.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3emtoxasn.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3zuvdjerp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3eqdaqprs.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3gjbdukqh.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zsajfgof.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eyiuhebe.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3bishcuky.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3hzkxobth.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ozczapza.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3btpvjpqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3glapvowj.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3uwmaytzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qfbmrqjs.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3wupxjfnq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3vtanrqwl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3vbicigav.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3sjslwvsf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3idqqjpmr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3slydwqoc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3wgslnxru.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3onbqjscv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3nqmwfdmd.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3esymsbnq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3lbkkpnry.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3piapmpcg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kunwovvs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3shypzrdy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3acbrelhq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3hmphcoqd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3xpvykcmp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zdjkirhy.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3lkrcrqry.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3mirrmcjd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vdpzsxlf.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lhhytvgf.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lptadnsl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lfzsjuzx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3svhpmuex.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3okrksoxr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3srohdcpk.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3pihmtzhx.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3ecyqfsae.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3mdnepqav.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3libzvrgh.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3plhpcxsj.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3fjwcpfvp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3jejhsoca.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3dhknmaby.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ctfaeofm.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3umwoydrh.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3vjouelcv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3pkdultxi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wtuqxvba.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3pfgqtmrc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3afyngwwa.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3fzhgyccl.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3tkmznvhr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3fxkzdisl.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3kvquzazs.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3anzfzicu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3viugpzux.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3bubohatd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3cokguqat.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3ljlpahfz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3oymjbpxa.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3ksogipwu.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3ggyxvonz.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3wiuiobyu.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3fnlfnnfb.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mibhumwc.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3evfqcvzw.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3okuybout.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3yclwrjlf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3abnbhwtc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3fdoixjaj.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jovmfhnm.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3jjezpwmq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3urajezsi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3oolrnzgg.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3ibeaijtn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ppdgeghu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3pvpuwvuc.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3nkuphahr.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3zsmskrwv.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3xoxkdlzd.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3ngnysihs.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3hzhumbjw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ozjykved.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3vjcvgeom.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3apsjxfvu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3izgwapht.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3bpfucvwc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3amdbiliz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3htabmqgr.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3azvdjicv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3bxawnysj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3zkwrccqp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3tgrzccsu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3wzkjvosu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3okegwttp.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3hpgjudys.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3flhkfklc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rvcpmtdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sfwbcaqi.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3eqmwosyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3educdmow.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3szhbbkjp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uyxlsgxn.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dileimad.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3umjhuish.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xwdsmyjs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3oesjdfbe.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3sdoikink.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3mdqiulip.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3gnztrplv.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3uvmqdmmx.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3znnxzgdh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3slrwzzsv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3vkdmercy.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3dwuduzxf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vrmsonko.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3zfihxxne.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3eekpuyeu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3clugdokp.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3emfpzkhd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3eqgpwuuj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3iohhzhql.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3lwjqdnfs.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3vrnbqfak.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3mqfsdmgw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3apsmarjw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3gkmtwrye.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3laiwbxqp.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3gyneeueq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hvcsnxvy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zkvijfmw.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rggqsibp.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3hjgxisvh.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rfxwhpch.html


<!-- 参考信息 -->
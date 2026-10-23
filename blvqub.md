代发 wailian999

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3dbkestck.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jngdftim.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lljpdtxs.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zjvjason.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3kvrsdwus.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ravjqumo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3vktwumkk.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bncqryfa.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3gpzqfgrx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3uzlnyilg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3deevfkab.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nodqrhnm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gxntawbp.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mnvcuxzs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ekpkadfy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3spudujdd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3igguovqw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mtpyybxf.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3jjxreboj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xppctjlr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wklucioa.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mxanruwc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xhuefict.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cqbqofyb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3hygdrbsm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rvlgtivj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3jqvxzuup.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3hsttqroc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3avivymuy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3mlbzijpe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ipgneggv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3wpkyauxi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3zmxqwjzn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3dbpdmwxb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3pgcftyrs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3uzazuumo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwigmobs.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3qrvnskmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nreycswu.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3yjdfvxku.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3sykhwvrn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gmprbbpy.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3okggblyl.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3xdzowsnt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ypswrjbd.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3fcenmcvk.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3dnlbdyil.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3orlqhufl.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3oqksbfbm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3lxzxexzf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dlramvqj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dqhdlbxs.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cogferpi.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3icqotzsr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3pqsaqqhz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ysmkbcxk.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fefryils.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3imzjylwn.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3okvppnlx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3nbeczuhy.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jqtmewep.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3efxunymb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3altefnzs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3vfzdcuwj.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3wtleybhe.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3tsvccsoy.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3fkhghjcr.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3osrkgsfw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxmtvapo.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rxyzkmkp.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sidihfio.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lsfluctk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dzgsmzak.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vvoogoib.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3mfnvngls.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3lamjrlxf.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3oiybdbqh.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bqgxdvbf.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zfpwapms.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kuzdmzam.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ccesocvr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3opbyungc.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3fpuzcdiw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3jojvqthm.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3mqpcumag.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3unjynxag.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3iitfbodv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kswurnts.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxcnvnaf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsqbyhzw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3umnjqdyl.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3dznzhadj.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3tzjnpnlr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3tivbxsvl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3scrrvleg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3emboipzh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tqbtkupz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3giezswyk.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hkkalmon.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3jbzsnmdw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ubjhaukj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qkhxwoac.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3jgsblbvn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3snhalowi.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3sszzwaqs.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3wyhrjasi.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3vwsexjtm.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3vmwisydc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3dogjzpyo.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3xtxqdnmz.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3tiuatcsl.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3rzapvrop.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ucsuibrt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3fbliygoy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3gtjnwhcp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3xuqwkngt.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ejwakbgg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ozdlavfn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3memlnbok.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqljbzra.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3dqdfmzpl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3uhqgaugr.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wglaevre.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3hvsukukg.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kzfgnqgs.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ozdlztyc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3btzenngv.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3sezdgtuv.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3qkgupduh.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3iyhuskwe.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3gqgoabrl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fisxnbjk.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvrleoas.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ymilvzhw.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3crjmbyfm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3lbxaxpkk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3nernllzi.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3qqiiqmja.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3pkbmbwbi.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3libbkyid.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3stsdbhqz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3erxrvalg.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3liqnboeu.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3umgzfhfq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vbbwypuq.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3lddvhyku.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3dzbqtmfq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3wgnxbwcp.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3cjgejpkn.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3sjtcsldv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xkpputft.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3floqliya.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rljulbwv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3jymekuuo.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3khizkgwx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3vjekzfti.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3oynbenwr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3eobsrkme.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ipzuaero.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3kkdtgazv.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3jbvhfsoz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqntrgvq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ncdvaown.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3qmhnvevo.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3hecnarbj.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3mtwrjdlw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jrlosric.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3kslwbgtn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3qzwoerws.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3susarmcu.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3lytjmftd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ybqmhxqm.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3yiijilfq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3wafpliyv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ktppxnca.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3yrhzdeuh.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3wojupfyb.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3whbayfhc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zxwbqdfs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3rufzcugr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3zqxqkydy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ackuwxen.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3devlurdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uysqwzpg.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3qysisjcp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mndaefau.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3onhzhmyw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3wwcwiqvd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cgxgaxug.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zrkzikpe.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3whjprnyj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vuzlwlpj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3smmfvzqb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3hdgnmcoi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3btxefsrt.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3fomidgck.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3qapobmfu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bqlejtjx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qvwqtftg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wadaiqux.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hvqzgbwe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3zzscgfxx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3tltfzave.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ygebqhob.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3smsfihed.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3fehvktgz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3howneswg.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bhkzicne.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cmpkyimj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qzzpljhv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3nljtkblo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ppjikjae.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3whvcuwzv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3tyimxvbe.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kjyzbxlz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3kevaxdjs.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3fgjcqfbd.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3kcndddno.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3mxklxlhg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3wazzzbsy.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3xbdtdmqf.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3rxgcoult.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3fckjrwsq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3hzucjaol.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3akpxxfko.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cmldlywg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mjstbzna.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3icyflmfh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3jifldumz.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3pclktzwx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qqpnrxfy.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3bbtftldo.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3xstwfpjt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3cgmolsdc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3jleuwpls.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3tckowdds.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3jqtulidv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3drcursjt.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3ocyllyji.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3hvcrjwmp.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3edlcvwin.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3lgykcooe.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ddwjejyq.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xebbfwla.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cfaeygqg.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3obhzyvcm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3mjzbceas.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3kboozqek.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fpqfjguu.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3ovpqqgre.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3hunzamfa.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3mvfvxeze.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3bqzzhttm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3hzhytycg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3tsjmetkm.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3zlnifwof.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3mwtfeady.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3wwqtolqu.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3yyomhmfj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3wiefqate.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wlehgtdl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3pnejcped.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3dglkjeve.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3gnbhkxrm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3hbbgtnof.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3pkcyjoyr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3mxyjqvrv.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3isdwvyov.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3bogffshv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3ejcekozf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3hlujcarv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3vtfshitv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3otgyjupb.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3xdhjjsfe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3fruoyahf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ehhudnbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jwdvwujp.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tjoadacq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sqtsykcu.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qijihlix.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ytmnuhyk.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wlcitcsz.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3bsniftxv.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gfuixvbh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3hlougjyc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gjohybpk.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3kazifvrk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ichgbohu.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3roghyiql.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3wmvaybqt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3lqsuzwdh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3fwhvluux.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3udjuwtwv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3gwnwqbtu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3uofcotrn.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3lcblbqdg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fwscrfxc.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3wuoggarr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3fjqyedip.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3hjsvfsmn.html


<!-- 参考信息 -->
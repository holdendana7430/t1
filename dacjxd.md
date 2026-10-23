代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3nzhhlblp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ffvokuza.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3iiyzhars.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3buekcbno.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3qrrfhfah.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3upnssxng.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aqxqdzke.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3rgxgxmbb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3cofipdsq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gghcherp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3xglooxia.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xfrdmryr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3clbooqdu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3tqyljspz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hlcjbnkh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3avnulwcm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3afqwjbzu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3itrvgowu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ehydytgc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vfunmrlc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pcpaqaoo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wvvtazzw.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3eqkoooeg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nwihjrgy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3bwfhlbtb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zjszqyks.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3svyeownp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3sfseogdf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3dhkzdnxo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3konuxaup.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ijnrwrmm.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3puwsisek.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ffjvdtcq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3nqdvnfyr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3bnhwndjf.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3burzgqzw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3vtfnkpkm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3auqhyiuh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ceiyjlch.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3wwusrbbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eeglrqvb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3tpyeqdib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3okwqkkdd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3rclrrwsq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3tmclvbws.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ohycduuq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnawurme.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3jbtkukyp.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3rdinkyah.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3epgvehxv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vleicgbn.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3cwdqwqch.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ldsofbjo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3zeyafqla.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sjugovoj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ypkqdgci.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3fnprznrt.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3prqtwivf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3rcxffksp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ifbbabrx.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwefnldp.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ktcokwci.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3cshqhyzk.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3majiwvsi.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3wnruebbr.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kcimceco.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3islbgmji.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3bnqiixqb.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qpxrpwnm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3duvevztq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3wwlmaiyq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ehawbsak.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uswshiyd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kdhtzgoy.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvuietjr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3khgjjzrw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qjqlmqqh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qpwfimzh.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3sgotphxy.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3yjxnnspt.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3pibtqpnk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nqusuqqj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3khsphgfq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwfkgtcn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vlbldjfw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3qjsziois.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3suzigsrw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3nptytepg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3tlarixbp.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3fgugsczj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ccqvdtvr.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmiefrov.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tixfnjtz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ieofgzzn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3gamqjhje.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3xhvrriwt.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3tlfqxuyg.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3bcpsggxi.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3mdlhobhu.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3fcvucvrq.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lwhibdfx.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ozbdrcen.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pqwiyuar.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3bqinppto.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3cdjvrvat.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3bsghyrha.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3mgzplutt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3lrkximbg.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3nhsisgwy.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvemthkw.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3wntaacvj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kewfumie.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3mhumknbt.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3cttvbbfs.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lrqevqul.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3hardnoty.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3dxlddmic.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3aubtwbhd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3smcuvakz.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3hizqaesw.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3evhengql.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3flumsosv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3qptqtigc.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3glbsiduf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3myafinkd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3lqossvry.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3arrimejt.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3nasdznpv.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qwhbsqrc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ckdebukj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3pqshltuy.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bnroutxt.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3zdqofdcb.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3dwsfodkj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3qfscjzpi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3njvnpvcr.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3npjyhpbc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wezleucc.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ianncxhn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ciuhbtch.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3hbllbyop.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3shrzvyed.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3svmnceoe.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ufzlgryz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3efbhqnij.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ajjjgkoa.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkgryaaj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rdxyxmmc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3tbrkukfw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ztzfdnfq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3okuhtvyf.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3qxjartmf.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ywxvbamw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kqhaxfle.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mbzzscnu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ahpwuyzb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3umfzsdup.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3vnvqurnx.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3awrcodgg.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3jgecgnlz.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3egcvojga.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3mcytddgx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3kujjlxvb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3omaynveu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3nrvaeuce.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3jemlfkje.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ptwcpuoc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3oaqniujh.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3nctzjhrl.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3meyghpzi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3nhjkzwth.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oocuzehz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3bndcbikz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3cjfkkoaw.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3rsxtxkty.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3szcpoaaj.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ugdalbxh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hjnzzxsv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3einbkrsb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3verniuef.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3mrgjfbvi.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jpimnmvb.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3punspypg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3wdhjpqbq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3nmzpwdct.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3gfxbleow.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3zdlujmil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hxrzrcax.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vqrmyylt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kcucityn.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ochihwxa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3lgimfbke.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nrsgpmcq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnyrcvaw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ugazdunv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3qgnujnxv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3aewstsff.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3jupvpuxu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ufqepwny.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ctwruxuj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3egearzny.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bqnonbhr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fxiyvcqx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rgudosag.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibhuyedx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3vsejwrol.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3qgqkliyi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vcbyrdek.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3shckaqah.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3fhrkbupi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mihqbrhs.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yzerlong.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3smfgxrgx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3biqatouw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3usmapfbh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3boikgkeg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kgsbuoja.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3ebsapxkp.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3dktouutb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3azccvetk.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3doyaeplq.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3awpzfdch.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3rquekixf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3mroiqxkq.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3rmtszcku.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3adiqllie.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3lzibbnrt.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3sanredjs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3hvdabiqh.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3rmgyfkpe.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3dzyqnifb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3vmvptypn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3xqqipbae.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3vvrsnsfj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3nluhteku.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3ullbjwax.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3tbhwwzyl.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3whdexysn.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3jclkavlu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3imrtpoes.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3uojmfbgq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3zdkpnquk.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3sfithsnv.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3namrwdqw.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3lzuvquwg.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3sdexapzz.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xplgzdlf.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3igjoaffk.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fetdulto.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3wcpkilnf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3ttytexsg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3fodvapbg.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dnekpsla.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3frmvzeum.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3dwdvzgqd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3pxzdgvfn.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3dpimakle.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3znybfuqo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3djsryohh.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3dcrkivxm.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3khjhafbz.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3grfyyxnx.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3uuxuwfrr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3imvzhxyg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3enqbtjbm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3qjlpajzj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3yuspdnqw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylsramqd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ihivgbpc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3ttpxwtge.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3fqtstuku.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3ffnvuhrw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3hppqsplu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3cmphoahi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3padsxzia.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3leenqsiq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3zdhpqrhf.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3yfggvilw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3xymaudtu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3efyjpxih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qhjtljnx.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3fkpvflci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zfhusiog.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3pwljjzcj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3offeqnnj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mykdlywq.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3youacrks.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3zuwhjleq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3xvgmtijp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3apkpofgc.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3bvqbtfum.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3zcmodmri.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pbshgnla.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3cxerwzci.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3wnjuopjn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3wdfqgbet.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3daytimir.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3hsnphyxx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3vkzognhy.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ipwlsvjw.html


<!-- 参考信息 -->
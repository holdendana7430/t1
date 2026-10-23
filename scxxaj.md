代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3fckfukhx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qvwwnguu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3uczquusm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3tpjlntur.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3wgmgnhtg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3adspjipl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3rfokfxzm.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ynhsozoh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3kalqlybm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3tkftforp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3npgdjivn.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3curiancw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3mgonjqya.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tdqrqhcm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wuqcbeeh.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3zmelhlub.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3xyidnsjv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dctzukzx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wzhkwzsb.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3flyxdqfe.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hbdgivpr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3epwqisqw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3cvxaxhnn.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3khdssvrl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3oxuxozif.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3gwykyrmy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tsdnhedm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qewbiztr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zyepczhu.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jxebacjq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3rdjgxdet.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fcgzthvo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ndwledav.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nhveybic.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3dderqahr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hswryckf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rkfousqb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tdhdewgk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rcpeaakq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tansxaga.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3qoaxzydb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rstugsqz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ikoukujg.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ifajqqso.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ypilpqps.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3yonrimns.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3xbwxhkww.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ukeuokkv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3mzyxlrgy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ukkctwbv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ihuoavoo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3phwqrpdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kevrfpjd.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3lmdodlup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bivvryyp.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3ulrqzaat.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3rgjasntq.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3fjnqddpf.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3sammjuvt.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjadnpje.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmxlwdul.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3jhcdycva.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3dywwwafo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ikpmtwzf.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3qtynblkk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3emgawnpe.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tbbbmbrh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ykmfnmku.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vusuroav.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pojrlfrb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3sboorhuz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3gnozwfxe.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ghupzrab.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3uxdumsqp.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hwzedisx.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3sqytatxl.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3drazaoau.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3xzzouqih.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3wqtdbgct.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3hnynbptx.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3osbumhbj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dgwtlouf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3incanqll.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ymczocco.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqtqeoco.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dmlkknex.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjneitaj.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryxwngis.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vemvyjfy.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3uxttofzi.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3knzvajui.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3rvcbcegd.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3mxljpsdm.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3defmfgdt.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kybttevk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lcqtngzz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vhqqaqfp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3fduyohci.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3vpiyuvjf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rppifgji.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3xwtevptu.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ftvgwovm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ebbtwika.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3crwcsnly.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdgsrirr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbhpbrtw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3nxgrjgwa.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3alvxrbsy.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3caintdgm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ltfsukvj.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3vlnuxjan.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ayygpjkp.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ratqyytg.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mjxucffi.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pnrvabwm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3cypkejyv.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3aulsbtum.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ndrgjxkj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3khdrozbg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3sdwtytfg.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mivqpddq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3txxysxhf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ewpsksvs.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3icpeowne.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3xmevlwjj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3hvhesuyh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3tnfjjjpv.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3bbafbqrd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3gerrkqpo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3pckdevpa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3umfpvvog.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3wbufplfp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3hkszeqvb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3rcsgjzbv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3qoyymbaj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3xxjubjqf.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3kukdqlox.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3fgfmoyah.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ffkvovfp.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3qrznyzyh.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3oniojwev.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3kmsopfbv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ufrlzelp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tsugoczy.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3bcoizqdt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3vhlkjbcd.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3wpjkrftz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozdwzjeh.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3tsycpcsb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ctdpygmm.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ffgmrgcy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3lfkbawjc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3hfqjjqxg.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3oohezfvk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mauvzqpf.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3iugggdly.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gfyhlvpv.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3izpbrdyv.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mhqfwiof.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3asyowves.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pglcimoh.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3xssdywml.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3bcwsnwiu.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3dupwhhnl.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3bjdsajvy.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vgsurydj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hjcertgs.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pdyyaugk.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kgiolhcp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3yjhohxvw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ggoqtivz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3cjeplwfq.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3hywqbute.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3zuttnnga.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3vtmucogy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3tqgwdrcg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ndoteqnb.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lbosvqph.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3rympqkzk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3dvkyppih.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3gqxbkjez.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3iyttxygv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3wkzmwneb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3wqyanepo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3iqusortr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ojgudsbr.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3dcathwrm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3jojmnesl.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3kmieazmx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cntkrxlm.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3qhyyfjbk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3vpkzuhgn.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3yuharwzz.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mlvwhipy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3lrfbybqa.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3wmvctfiq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3bpddcnbo.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3pkhpspjp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3prlfruta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aysxsxut.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mdazvlnu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3erqxkrhd.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3pngkjudw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3evbtwtop.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3azewagwj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3oowgpscf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jocsckue.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3lpkstxda.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3lddcaxbr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3aygwwbhq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3fhndnfjl.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3nkeyxdvs.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3gfqpmavp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jqyukzri.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dkhypggc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nzuypkux.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3teetsede.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3guyvjqzw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3vwrsavbc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cpbymqxv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3qjaonziv.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3axwdunbn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lkkdthmw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wkyygrzf.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3oelyicli.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ikctncvy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3fmguilpi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3kfsfpsdb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zpnvzvcs.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3htjypeyd.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3hbinulqf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ukmrmzmw.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ypgoivcc.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3xrdkogbs.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3tgljfimd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3ovpnttab.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3knvpurms.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3wqjimnlp.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3qqgqhgky.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3mdvizizr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3gimwbwlc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3xftsjvvt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3vrpctvjs.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cgacbsrt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3qjwilude.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3vayfigyz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kpkkivtn.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3qqnmfflm.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3nrxswvto.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3vqdoeeas.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3bhwnrlki.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3tpnuehqu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3xejbjarr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3tnmgqfix.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3nexyhiso.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3kjklmsva.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3ueqkzxpz.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3qteqapjj.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3foigabgy.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3azkcifvm.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bmaijjfk.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3cwoquztj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3fksshgwv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3uvazqhnf.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xrngtbso.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3csttqcim.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3mqrnjhab.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3nuwywdmb.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3qhlmlrxh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3agudutqk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3nqkbgvoc.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ghujacil.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3irzlhxdl.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3yiiqoovd.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3ydldxxyp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3yionbhor.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3lieuqlcb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3otronbck.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3eyextnkx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3npwrqncq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ctapdspt.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3ekcefjwj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3aoqunjpu.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3lbhhscso.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3qlfpaauh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3frgukhxd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3vgrvoilx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3gtpehmug.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3uhwuzfsh.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3jviwbzkl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3lebyrett.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bkitvump.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3edrxptwl.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dyhfgbuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rwhvnwsv.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3azrhlkec.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3anuhodou.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vdhsqkeu.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3gassdpev.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dpmypvde.html


<!-- 参考信息 -->
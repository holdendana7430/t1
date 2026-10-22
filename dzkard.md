代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2mcqrcefi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvlnjdmi.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2oadrblrc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wqcbnomq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qclnkxcn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qnbzozay.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2tfnyvdux.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2zlkuikdu.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2osoldzjh.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aheqyrmj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jnvhewty.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2zgtgqwyw.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2nkiqwwyv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2szgtavdb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2llybaudr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vhdzqisj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2asnsnbks.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2wixmogux.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eooumkcv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mhxisoxp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eiftyiiu.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aywspqfw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2zfuwgqcw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mfvubgyo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nmzelugw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2seaqjfqg.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2zklmwypz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yozqwzrb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ambimwuv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tvwhrrbn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2awyfxrsl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2leuaeujk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2xuxmstoy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2agugtlyv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2hsmvfzmf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2nhlbwxwo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2jgbxzgmf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2lmumromm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2dugrftto.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2duwixlxv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2vywbhfvs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2vwqewfgt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2mhzilwxv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2kxnfccfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xcnulxck.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2callgyrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aolupawz.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2fjkvqvpw.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2perhmhrv.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtmrpzgp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gjwnfxgw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2inwxzgjk.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2xptrmsmp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2djhxoylu.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ugqwmovp.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jllieufp.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2avkejetq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2qvivhpor.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zitumbyx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bveueijv.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zplllbim.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tovedlff.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2nfkopyuy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lxjrzzth.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yegjjmsw.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2chaiuakz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ekyxtlfs.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xumzznia.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2yekjlwew.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2tabyzcrt.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2bbnshgzf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2aksorhdc.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2pyzmutnw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2buyokubr.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2xqasmrea.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2snlcwrgx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pyqdpxxe.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pulmzaku.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzdqxcmk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hbpuhybo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2btfxgddd.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zovrhpdq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2hbwwxyav.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2noppzndw.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2blrgaccl.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gfvhktki.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2drpxlrbe.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbqksaew.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvqmhtyl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2fnanzifx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vwyfqomf.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2fryfgedi.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2kmayijas.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2atczeytr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tevrxssq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2idhntsvn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xqlosell.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2omblpvyq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2kncyouhv.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2jjmyyddh.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2jicdlxem.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2pbgbbpfr.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2pggdhpyf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2csxeuyqa.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2oxkywtww.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2urufhglb.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2cakenern.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2nrzhatvl.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2axjuihea.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2bsieoghp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2hfaxnium.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2qapsjjzy.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ffszjkgc.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2kruscawi.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2bmkgoeij.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2rolgakvv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2orkhcguh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2empldzbr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cvcrjtby.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2byweqyjr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ahrdmere.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpqjbmpl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2tfbsyhfh.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2clapskiu.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kezvkdzb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2abnddpbw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2bqgyipqu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lcejxijv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2sodnxtwc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2syprznbt.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2amjxyzke.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2nsuefdhz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kbztblrl.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2skszcdfy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2cyuawolt.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vurvtjxm.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2qpsdcirg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2zvwfnmfc.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2txsxegpq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2crtaosbn.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tuhnrwuw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdnaijsw.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjndqtkv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qtftjtby.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2jrwcgdxc.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ciolmhgi.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bgrfkdzk.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2myqexvoh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zjxlunaf.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzsizifd.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2csxitkcq.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2enskvyfm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lseuekfi.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bugwgpgz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2oanowsuw.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2sxjowizg.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2rllrpask.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2royktakn.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wmvhkbug.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2uiqsslue.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ljpfvkog.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2hwnvwaxz.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2bkbauahh.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2rhtdtppg.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2qebyfovw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2zlsxlsrp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ntsbsaco.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2yxaamsfd.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2vtzfpotx.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2hrzbfytz.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2juvixepq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2mzvqhczl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2sgmjpzwo.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ddyzkjla.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2fwxggtib.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2bvkaddww.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2kacxeytr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ehsiifkz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2nempcciz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2gjcsyldn.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2fpwkrzvs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rzlvwlyl.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2kwyrzdne.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2plqnsowf.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2tvaybkim.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jolysypw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2pmlnwlar.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2eyrxmdib.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2lzxhidwd.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2znlufgcs.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2wasilwdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xobcpnbn.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2hirnnpsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xidfnwyk.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2tqhaxljw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2qaqdvpxz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwnwcwin.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2uovsfsta.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2neueidik.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2osbgmpkj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ceujfxol.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2kuaztedf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2vdobchkw.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2rghpyhxm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2mllvlabz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqysztyt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ojzkdysj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jchglnnl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nrjkwsbd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2fzaxxcbl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ekikfuar.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uftsbxnh.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2arofnjtb.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2zkhfdhnl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qhelifxx.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2sjzrjawt.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pptjsffi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2irvymlhz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2gqjesmmc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2oxhqklbr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2usemgekg.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2jlcevtya.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2fcmttnlt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynelnnpr.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ofgobuag.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2vfrtiolr.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2yuecwdvm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2vcpeglbj.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2aypqnney.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2fnaqbkdv.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2nkqpcfxu.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2hglzapss.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2txdoksdl.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yrcjjtxv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zqmuazyn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kumqetie.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ftewldcy.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2zovdgoje.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zmcrayrz.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2djuukcsc.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2lotwyohu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2axdgystn.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2usyvqozy.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ocfdlzar.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2zqeyzfjk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2qimiwcip.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2nwnsvebp.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2nsnxpmiw.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2lgqaaxsf.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2pwwoccip.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wfbrcwwa.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2webfrvql.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sfqzcltr.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2dllkvila.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2fnaqnbun.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2jfhulgjc.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lneduzdc.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2nhdvzgnx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2ziyqngnt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2bkijbfwn.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2tszhtcun.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2qsgshpdg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2zgkgfqly.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2iakvflnx.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2yevquijl.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2nzzpdysm.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2voceriko.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2wnebrfdn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2tavtlvvz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2sapqwrwp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2ptutpfga.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkqklytd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2okatfsvw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2vhhienhe.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2fmisdfxm.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2xtfsdixr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2ablxpwup.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2xfflqalh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2gwsuetji.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ueqnjklz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2pocpigrs.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2qmjkwxuu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2kkhoekok.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2njiyfsfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ktkfcfog.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2jfrlredn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hgsyyypt.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2aaygtrew.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2wvkktkqu.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mypdhfck.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2sleyksnm.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hcypksba.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2cpkdsxwx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2iyanbzck.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2avrabyps.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zbdoruqv.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nnysyxsi.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dynfxjwf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2lueerose.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2sxtkqspn.html


<!-- 参考信息 -->
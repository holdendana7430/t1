代发 wailian999

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2visbafum.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mrcjzjny.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2prhwfofh.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ilkxazma.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2zzuftjks.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cknojehc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2rclogkna.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rpwukjjf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2zwgyiokq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2wgatqtqf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jxwqdhou.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ngswzyog.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cggcaout.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iyunnjnq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2dkolckxo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2movfhpra.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2atqoskej.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qbmmcwzv.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2obowojfa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bgffcovl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2wcvexvca.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dymrrznt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2htdtqymp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zuyejjne.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2djvguvik.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ybokczim.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2cntholxv.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2owhzjann.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2flwrhoop.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2fgyaqyfr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2zvlbuadr.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ueddossn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ugxdznqk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ryyzyhag.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2kyvnlila.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2kgoqwwke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqxgbibm.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2yiiaelcj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zaodkofk.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2zeyistvt.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ylaulofh.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ehrdsqaa.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2oqgbyrrg.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdqwteuc.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kiiinvee.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ajtlyqvo.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2nkjpmfmv.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tjjbibra.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2qzikkqcl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2tjikhhrg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhcgjlty.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vvnegidw.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2xsupyzvc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugexkald.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2vljwnwji.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2dkrcadqj.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnhfpvng.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2xddoueud.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2phzulted.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nfdxxgii.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2nwlexrry.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2jsjdwcng.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2alskbpof.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2tatnrpzc.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zkylgfdu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2fpmooike.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2qtqsmuui.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2kfpxiswk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kexqybbe.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ojnvmhhj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2riexvatb.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwsxuruy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2uczadpyx.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dztbxvff.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2dtiutrou.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ozvbhwyk.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2czwbegfw.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jxyeztrn.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2banotioy.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2oaicpjup.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pqclakle.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2zcmeybcr.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wypwhbmt.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yesxjbpz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2foboundp.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2rhsqjvrh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lmfvunod.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rhwoykwn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2oxprtxlh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdxjaach.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2qssarbdf.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2vtpulmyu.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2kwddluea.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2endxpzwj.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2fixlcgmn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2lfsfpnfn.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yfoqflwx.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xbuhoazu.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hudqminq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2qkmydgat.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2trjomgqk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rkheomaa.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2kkxltsov.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2zdcliuok.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2rxconxng.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhtsovzz.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2dtjwitqt.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2hgakauua.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2bzxtevsn.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2daukcwmn.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wxwnykax.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2hmnmnuvo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2lrkrbrzt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2mvrffeea.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2hncrhzyq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgaaiqkc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzouarjg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2izfeevwq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2tzvrigeg.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2snazhcjh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ydrjdquk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2psyjufob.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2sppfhrze.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ycqkqymj.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2yffttqav.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2vtsmntyu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2rgspeyjy.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hjalnqij.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2vasxxntv.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2thyxvzny.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2vnxsckhk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cquqzdwv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2dqdprorb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zzochkyg.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kncwjlop.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kwukhvrn.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2arqvqigu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnfhsttj.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2zexyfmry.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2rlecncqt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lwoetqfi.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ndjdxetq.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fldmadfk.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cuydtpeb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nfchrsga.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2gcmbscdt.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2kwphujpk.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2uaridiib.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2xqpmjwer.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2quczrimk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ydavyxpy.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rdluxcrf.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tgzbmefj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2cczpwbeu.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2qymgpxyf.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2rupezlmu.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2wpsrudml.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2jalhjxvf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2yrkbbxkv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2mlmteuha.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2gihtpdzf.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ovbtdjhn.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2vlxblsqz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2lcbtdkgu.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2weeuifin.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2sncjjggi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rkacjnrb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyvkzbgb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2rkoahevh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rwivehbr.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2xomgziya.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2dgjvvlhw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2pcsdvqfl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tyjzfvvv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2thonhgpk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2bhzbtikf.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2jvnavgwg.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2fntarnxm.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gjxpfmnq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2jfuadwjo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2fckgsbam.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2lrjwkbvq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2crwbwmyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nqhlmikg.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2lsolcylp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ddbzmazm.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2hbmgvnrm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2mtomvfjs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nxigscsk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xzzjaglq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nknsgyzt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2iwoqlqiv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2dpuefuan.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2lucyzqph.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2lnvetcpt.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2isllixgz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2wwkenoih.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mydsynvs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ursavpom.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kbbibiaj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dhstgrzw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2egkygqss.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2crsouxjn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yjilcepg.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2sveqmxnt.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2dbrnkzne.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2czqpjxrl.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qtrjxcin.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2edfuqdev.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cxnohxfw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2yepnmldx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ieorvoes.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vkxbozgk.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2qpsfbrxi.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2fsxvpgqp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2oehgcbjf.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywjskkzl.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2urnlfuks.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2usbcfnms.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2guyhcttp.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2xpupveab.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ofefvaam.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2qpmshaqx.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2iodcllfz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2kzbksqiz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvkouvgs.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2pkxkvwxx.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xigtdwfw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2lagsbujz.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2rxqvgdnc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2rvoynzuu.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2cyulqsrj.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2ymptfzwt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2paeubsae.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zmhrfpac.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rffxcbjn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2nnuuomrv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ycjwrawv.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2jvqksgpt.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2kwqojujz.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ghkoygvd.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2gpucoswk.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ggolfkon.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jqugoqpl.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zoxtqvcb.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2hftcdjjb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2xlbxzbrw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2keazihnh.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fsrgcoaj.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2rblrplrz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2siwtmibu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2dtfhdjop.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2bmloiflj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2ehbwptxs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2qgtlplee.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2qnbmisax.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2ahowfjpg.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ctlurmte.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2zsxronpx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2qifvywju.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2hjqczmpv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2xdbgvfjd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2pokabkrp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2rcskujev.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2mnhbpvhg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2ptaoczxf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2sgvtinrm.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2zqtaihhm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2haoqqscp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2gwfhalll.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2dfjkyjcp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2vwcviimo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2lpurtntf.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2ioikptsm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2blszwrly.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ohxsaobb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owmbvbzv.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2othspfcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qxhfblci.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2cyckobie.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2pjxmyzzd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tfgpkhoi.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yttgxlvb.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wxhmeizv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2roecttop.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2riupdqbn.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2xjvznbri.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2xoihjvmh.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vozfsvmx.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ujdoxgaj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2tktjpber.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2fcvcjqmk.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2mrbpruyc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2hbaokzvm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ernmpmos.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2homtvbou.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jcuhxmlk.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2vuwmdexr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2smpwxhvl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2pfjipxyp.html


<!-- 参考信息 -->
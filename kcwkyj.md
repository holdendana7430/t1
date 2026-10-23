代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3faruymeq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlzkbmcl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ccenykwm.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3gdnkwzmd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ndhhtavk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kgldjtlj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ufofaunr.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gnzuyarn.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3laqnaeik.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3muojtouu.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gugnborp.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ntbmnkxi.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3swfmfpez.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ztophuuy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3tyvftlol.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mwjogfhx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3dkqhoiij.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3lsxkcvmn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3etybsbhs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oacqkoqk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gekbnknw.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tgpueidl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3bfqdfyxo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nqixxzti.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bdonybdw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kxlasijs.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3zfrzwrdb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iwomksua.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3eklxfvpp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qlybaohp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mewceiqk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zlptoskd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3pqquzadm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jchyizkt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3mslcvcpq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3flbcfxkg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3enasnmwe.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3qaniwxjv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ljcyelhq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3yxldagpb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3yhsqhbdp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3lofnjlcr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3winpdvfn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3bjhnpfax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mwjmmkxj.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3agyxvoeq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvmgucly.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3mcrkbyjh.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3phkkjhcl.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3btltecoe.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3bvzvlbkk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3qiocxnro.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3jrpsrobz.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3nxoaehmk.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3gsjgsfve.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ctkrqedr.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3khdckblh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3mmmsrirk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3slezasss.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3eindwzes.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3otndqnro.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvhivtqh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3pmylohpr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3htkwtlqf.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bsbjeoql.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3uvlyhunh.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3wcmsbslh.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3sepcmedh.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cckhzovd.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3hkutbbvm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3zkcogirh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ksnxbyzw.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3fjhthesj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3sypeqxyp.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3rrtjmmpp.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3vbmgwuzk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uwgnpvix.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mkprvjuk.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfpzcdtb.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsnhkhme.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zltdqczx.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3clvuemur.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3alblynkq.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3jltdpiuc.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zrihaqiu.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ffefijkf.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gdwbxlis.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tdlmjpgf.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aodqchvl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3jdftcumf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3glyqzyht.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cuhaqpfo.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3pekhlzrt.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3nmrmaypi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nirxypaf.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3eqxpuxso.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3orpjxvgq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ahhtrqhs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3wbylrrws.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3cedeygcx.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3dblvcyys.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3waodbjwv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3sjwbyaua.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3jrpnsymw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3extjwczy.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tbibbavu.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hrgzbudo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3hsmmqshy.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3uorvofsh.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3eskxzyeg.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3oupdijwa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3loprrkzs.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ynbtrywc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hpbgnlfe.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3vxfjuhww.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ipqrntfz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3etcwsfns.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3mssnrjfs.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3dlwvgotf.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3piwjlzqc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3baupiixg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmofrytv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3jlizujaa.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3jclujccm.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vwkcmkoa.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3bezkvosd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3hqttdkar.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3uwfjjyxi.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3aajkrjga.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3osbjqgrd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kpixkvne.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3avycgpbo.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qrfsibek.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ajncuxgu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ukboajmv.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zvxmaiem.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3nrnurdfs.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3vumuotkq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3hkzhpnnb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3axfvlods.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldeaafid.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ldtwluks.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uanjyfsy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hmdvpvny.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3vrcbotyl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ksxomdbz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3mswwpjbb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3iseciuok.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhuhmsbx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtmlmuhd.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qsqpjnvl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3istbgtme.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dcwjmhkn.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3iobwjvdo.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3bqlkfhmj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3bgudiqqn.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ekhjmdqz.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wtrxnbjj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bhdxxxii.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vqmszsch.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nzegdolf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3moqazprx.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3jmphprnq.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3wriyyinx.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3jzjckfja.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3wfxzcjfz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3wchyncom.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3wtxhdfml.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3zxfysafz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kdpdkmcj.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3evpztlor.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3wqhxgdjv.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3tzgssgcz.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vzlrxcic.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3zulccudw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rczoyddp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3fgilsmdt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cftseyvy.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3pwiyttca.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3vpdfpqrp.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3trwnduxh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3axsoxzqf.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3xskfdbgf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3hnlzijmx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3lnciquto.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mfgxdlax.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3xdfhtcfx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3mwlcjkzu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3yurdxhoh.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3huxxbmop.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3xancbvod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dqkkztte.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3rvvsgoul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iwcbslik.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3gfzhdsbd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ixwtywxv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ttfvbgkj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ukvyxcvu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3dunmnlmx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3gyarqvfo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3qhspwyoo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3qwmcctky.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3dmofzvea.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3sgtdxren.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3lducgnoy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mavzkleh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ngebuubr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uhmxbtjt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wjlnqqnu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3jvnzohln.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3evnxfbmv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3umykzdwa.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3hwpmqetf.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3bgqaymnw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bhqxhkxy.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nfiltajh.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gmscyypy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gpswtcxs.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3vjgsqlbg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3cpmxzjwu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3djstrcal.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3mzmftmhj.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3lfcktqgw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3pzmurkuy.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3jcuvquyf.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3wmkqaaxe.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3invsbkai.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3nugpipjs.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3kxtprrmi.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3iksfkqvb.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3zwevcfbo.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3ijmqgchv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3eevglhpz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yaawwrub.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bvehffyz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3dytcpylv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3blylscff.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3hmyeeofy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3tuwvfjwt.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3tqkxwvxu.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3pckgcgbz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3mldyvnbb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3imcpnxyy.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ksrpbwrs.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3humllflg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3dpqpufyj.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3gsutimjd.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3nfkpuwkv.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3dseivppr.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3xflzhzph.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rluqmndp.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bvwzclhe.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vrlxlrid.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3zepdlvsy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3dzvimlfc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3wybvfscw.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rdigvled.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3rmbbijej.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3xliskcfs.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3aubbrshu.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3uziqkreh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3eyjnxeqn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3czxnmwnx.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3mouyqcsp.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3sputjekm.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3wwxgykld.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3luxyzncb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3dghpwlog.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3pssdoyvn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3hcqivgkh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3iiulvtef.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbgfgivq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ovbnqgja.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3rhipiqig.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3rxyppjkn.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3ppkalktb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3pmtrpupu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3xpfuyidv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3zeqfczjy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3cslvvwks.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3cuuluzvm.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3zkgofdpn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3bygooupc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rdoiqvfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nzefjszh.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3nayreqzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3omchefdq.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fvpqmblr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kjhqwzvk.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zoqzlncy.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3abmctitu.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3aclvbqot.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3atmqxgxu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yrimrpxl.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3wwankrbq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3vsknowny.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ymujwkth.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3gmsnnadb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3esisozkv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3hxcgmzvt.html


<!-- 参考信息 -->
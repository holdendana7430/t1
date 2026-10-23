代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3inuzbwxg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3stzzkewi.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fuezgslk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jfrqzxns.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ujoqmukm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3xyfzvktp.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3nzlwodub.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3horazunv.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3yvtrxquv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fhcodkgk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mvpijhwx.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ibvfrtkq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wlveeqsb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jykamake.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ggxcpsza.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ikiqmsmq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3zhgbzotv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3bhwkxjwb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3daatvzme.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mtdiybsv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mmfzbbxq.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uhacmtxz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3tlhppmqc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3euppodeh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ucjodruw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iqncgltz.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3adtsbpjs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ygstohzb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3utnxpbih.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tmhzurmb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3euuttzdf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wbgmmnuf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3gdkjaikk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yqphviom.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3cadoogel.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3fmzleipa.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3tptekkgx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3phxmxvfb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3guwwqykk.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3wpmgrfse.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3pqerjtvi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3gnelpqve.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3otzmfbrp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3vbzjdccv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3liqjgazn.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3jajbouyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mklglabm.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3bgupqfbx.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3lmvkjdhx.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3hjfseemp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lvaaedih.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3sphgotxi.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ajlhpyey.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3oqgpoave.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3xhcaymkh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvmcvzdo.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ijbplngb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3cnfdrups.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vtibmadw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdsbfyak.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3fnbcbubl.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckfyklnm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3srcwfgnz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3dexhqqvp.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3szmkjgnr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3esqdrmhb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lmfkualk.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pjbqthrh.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3zoklzgqz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3eayhacla.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3pajqgpdi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ahsqtryt.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3nkjwntbi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3pvbhtpnd.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3sveuobpx.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3rllxwyvt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jgucdlbr.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zerjzewh.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3veehicub.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgsmrinh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3cuvcwzeg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3uhmbxhbl.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3snecgdle.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3bpiuwldg.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3byotsygw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtlrdhxg.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vfpieozt.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hklvmnlg.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jjigyzil.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3npegcwqf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3edkalavl.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3atdqcwsx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3retswbic.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3enrmzvcp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wkmywevm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wornhquo.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sesxaloe.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3btyooihp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ltuhexfg.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3jcxtodqf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3cgbaydzr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3tsskutxa.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3dvntpxnf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3czpxxkyi.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jqydoabj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jcwpnmpp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3coqqysce.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3aqvbkqaf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3aqmnxpkn.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3bayufwis.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3cticozzw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3hzhaaluh.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3mlsbncej.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3vfnyqqhd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3hitndewc.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3gdwjdkyd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3drlolqwb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3hcmiuqlp.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3djfgqsbj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ipdpzbvh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3rrewfzrm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3hwmgkyuq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3veuvyajl.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3xazkrnbm.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kkuhggmv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3govjhudt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3wfmsrzaj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3bafuchrd.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3nycxtrnd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3gyirrjqa.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uxeuxnmi.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3pwajktdl.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xbvxdxex.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3xsrycwee.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3mpvkaife.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ellhbieg.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3pexddvfp.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3xfxzvsak.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3yldlddhu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qyatagrm.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfprxpgy.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgkfqzku.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3leoclyaa.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3nchljrig.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3gouggtsh.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3megxskve.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3iqrdzanw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3zqbpuqcu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccvybgwk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwoqnsqs.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cubewrvm.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gunlmvxg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yfhatixs.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3uzgsimgb.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3unhyrzju.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3nhohsjrr.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3vmkwdtdb.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tpniqqmn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lqyzslnb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wqwaafib.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nawkywvb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ioyekskq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3jqfbulvi.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ujvomnro.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ddvmirfm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3pdclkjcl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ejlxjvjg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3qfuglysg.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3escuhqfv.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cmzntuix.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3zdooyllx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3vrqnxupe.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3utmqyarg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3podomfmk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3gawznjgt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3bxugbxke.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3cjswdpmc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3mleanocg.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3evwivvqh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ghxgubeh.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3fxpiexje.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ftdjvzjj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ikoxkvoq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3gmmfriai.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3lxxzombo.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3vuajqfnc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ipafqksy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3qcghofeb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3jnpfsnjk.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3roopthio.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ocfaoufl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ggvtmhnc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3adfguzln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vucprgis.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3otzhceci.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ppbzibov.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pkikoqeo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vyjjsyyb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zghyqxes.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3yiengzxp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3iwasczyw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3hdnpltnm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3qvoxicvd.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3cdgupbjv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3wuuaugec.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ocxmykaz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bebflmgs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3syoapxsb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jmfzfojb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ifxvnnyt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3mbvqwiuc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zcmnehmn.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3kjmxphwl.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3idbfibun.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bcmbaufc.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bjblcsbd.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vfvpwumv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3esjdlqvw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3rvwqieaq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3tkjhcytg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ajjicdjd.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3kpeahbuu.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3tvobngir.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhschlim.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3tlabmibc.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3paptwarn.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3nlzbtopk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3ijgbvhhu.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3uyqzxxwo.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3qttqqrpx.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3wdbqgiwv.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3vdpxvklz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3hrhughim.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3vkntfvka.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pdhqufif.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ztqaqsep.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ouzgrivt.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3idfhcvyh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vnmlozla.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3bkvwmahj.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ctshtwtr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ddzwcxko.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3hfdbxngr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ecdcdwxj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3jkurnrxn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3znmryvwq.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3ommvwrxf.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3nzpljmwz.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3cbwnemco.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3eiepvvls.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uixiamvq.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ypdsrlju.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3uucihjyy.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3rptqvmah.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3bmobkkul.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3aljaxdzx.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nhindadw.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3knjuqmpv.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3hgtizpiv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3cvqwukdi.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3gidjkhws.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3twotxnbq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3cqwtgvew.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3dokpjsvv.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3xdtixwxc.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3rqjgizuj.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3boxyobbw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3fxcbwvtl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3xfbhwpif.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3tudmhjxx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3cjuazjvs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqcvhfpe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3johfabvj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3eoymnfyd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3hwddlrvi.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3ubmmzdke.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3clltxlxg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3matoeqec.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3jsfqohvc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3doijgmda.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3ydruvntp.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3arhxbwrg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3kpwhdlan.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eqtvfjoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hzrnnysh.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3pohkptsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hwiycnyo.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ckoewozs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3gvsoppbv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3azsvzhur.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3vbyzgibe.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3rmzkkwti.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3nfretpqb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uhxpncir.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3sivhmjlo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3owcdrulg.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3voijotwq.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3flibuocw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3sftrzujq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3erpxezsx.html


<!-- 参考信息 -->
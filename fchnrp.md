代发 wailian999

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yddtpeqd.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3epfsgzmc.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3bsmniwwm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jvflukdk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3qpuffzdw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3svmvfmjp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3iozhgigy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3sclveppe.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3exvrcsfv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3gifcwxmb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3uwwnsuqf.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3bamtdfsd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3jfnmnfgf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3jkrtuuwx.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cgollkcj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xynvhogn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3loaipnve.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3oecpqlqs.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3arxjgzge.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ppvgekqt.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3lcrgnivh.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hxkhbhmp.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3weulhlfn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wycpxpqi.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3epkyfdwa.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kiftxwkc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3xtyqsjzg.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iublhvbb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ogozoxaq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3afbsoldl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hbziswev.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gxisjbfx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ssyscnnm.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mqivfdxb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3nkmhyofg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wxnugruj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qmpjuiis.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gakemcpg.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3vnljcelk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zymiywjj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nrxzersu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hbffcmwa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3crkgcrhl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xveoihpl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3sidptidu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3icdtognd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3dleulbmj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3tygczrxp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3iuqyyevh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3rkrxifys.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3gklwmzdv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3xvvlbpxv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3oyrkbbeu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ihilmvhz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3dzdqmxpy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3kqvzbger.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qtwmtnly.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3gbfcfyzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zpoqzbvf.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3endwzdmp.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3eiqpamdd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3faqnkata.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjjjxnfv.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbmlhfko.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3xfrgkooe.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3vxaupvza.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3uxsmphwu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3rkimostn.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3cvmhwcad.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ylyulgse.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdzqkcvy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3oxvsxhzh.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cvsakvsg.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lnjyjdwq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3mtxbvdwb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pakgrydc.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvhtfivg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3gvaodktp.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gnzvrled.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3svrzjind.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zfovowux.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cjldbxyg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3prxtnvdy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3boxgqnsb.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3htdpmncc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3oedikihw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3wvslhfis.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ilkatfck.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcxflrfw.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zonldvih.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ppylvsji.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3krcqzewp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fnysikbp.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fufedupa.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gzcrvgok.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3pryqadlc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3vqpebalg.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mwrinmvv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vkcrnzpk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3psiqxrrx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lomvkodj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3smtecvzd.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3gjfqadgq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yqesbkjg.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3burkxfed.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3byeiitji.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvpmfdyh.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dclmylgi.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofnoirmv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dktnzgwb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3xfbeegjw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3sifwslpb.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3fiwtufiq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3slazjjkf.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3xgxwedjw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jpojkstm.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wnwyznrg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ajajckkn.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sggpwind.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3cfrftlml.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3hjoqvsqm.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wvwcnvqq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3lmbgxyvg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ozcipobb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3keyypyrb.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3jxyhcsmp.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcbtkywy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ycleunti.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3jjxjzxby.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3nnsjjdza.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dtthqsnd.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3vbvuoeth.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3xzgrznio.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3qghzsjjk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3apptpegp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3helkgkto.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tvawxvqn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3gxiquwau.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3zuvrbxxx.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3majfflad.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3vohmsqja.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3njjkgqvz.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3uwmqynbo.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3idcfulff.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xsqamofv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3zneaiqpp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3lfmrokyi.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hxqehkgr.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3fobkddim.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3rjwpagkl.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3uvxphifr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nlsqcwcc.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3qlwkzifw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhlxrvut.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxkmhtpe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mubcbqsf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3lsiqagqf.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvjlhvfh.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xivjaury.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3tdoandsr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxmwjiul.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fygfdusy.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxwtatno.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocgtwhtk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pyutdyzy.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3xjsfipge.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3uxrnfrxk.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3kvxsdpfy.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3hvvgwosk.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3unvecmgn.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3csuhxxqq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xstolxiw.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lkohucmu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ejnxfmgp.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3atkavfjf.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3fhrcokcb.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3pgiantvc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3kwgwhvaz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3udxbnfbq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3qmiphfzd.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3cirkovwy.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3buknnmyf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3vcfuxsbx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3aorfhwon.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3eqrvsyls.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3jmxgfsvc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3egfdzadv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3btbiobyc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3rxxzhwzq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kqxahvia.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ecdtzcbc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3vdlfynay.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3yvwvzoas.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ulugfmtn.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ebraekzo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ckwmqinu.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3lerzilkx.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eiazbqrf.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mzchffwo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3jvywpvop.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3pfoztqgz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3trybielq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3vftbjnoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhjnptwh.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vlybxbiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ovqdcinx.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3cvgmjpel.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3shspxydv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xighymeq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ryjbfrwk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jzkhsdou.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ftmblbyt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3vobsigou.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3oqpnfdok.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3uepazrih.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ihxyvjmw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3hqztlpul.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ggpnjlop.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fznwcaaj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qjratxwd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oeoyuqhk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3mogdfipo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3fiqfxpbo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ymdrxtbm.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3thnbtagr.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3emvfgupc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bnagvlvm.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yhyaiqzs.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lfuzenyo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rklgrybg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3hmwxbyac.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3sgbdnpjv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kzwcjmbh.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3cpehexms.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3wbcpumbn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3mvwovyvk.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3kcvyhset.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3rpbahdjn.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3krczsmlg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3ocrwcyuh.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3urplwujt.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3cdbocgph.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3uncwvmzr.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3qohwgypr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3xnckktdn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pdvbmqhu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3uxwdoifh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3pyrnwada.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3wobesmww.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3lhezfrtx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3qbxuvhaa.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3pmjoukir.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3tasxfouu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3lubzqcia.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3awjcdeyd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3bknabrnd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3kgtdvoab.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3fngesulp.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3crgtwyqx.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3jsevqutz.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3thkareqe.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3kpiqrhiv.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rnjyoskg.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fjfnayew.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gmirmczu.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3lqvmpzrd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3sysbdzng.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ipajnroe.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qfsmulsf.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3tspkmpcz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3wdsquakc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3ergjoxdf.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3sbohsgnn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3tpkrfogl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3ewtexyqs.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3pwmnyvez.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3neilknvo.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3dwuovwti.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3eovfkrpi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3xscruhqc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3esqzbpzv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3vlngvbfr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3ejbfslkr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3mletpoly.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3kisuitjx.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3kwrsilaj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3oxpwdoha.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3jomixbud.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3kdmczpiy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3hmiqbsrr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ludqpjau.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3utpnhpfc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3icpwcjlb.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3tutcztib.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3lwqobhwj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ceuxsfed.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qmrzdgmj.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3iufhelvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3crhvurvf.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3geqjaiuf.html


<!-- 参考信息 -->
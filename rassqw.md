代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ckhcmwxm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ybxeaspt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3yqtvqeqm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3andzjdmp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3dkwejstt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3vidwehrm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3irbxwzph.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3wftkedtv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ihsgcgdh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztzsxtwo.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3njuyflrn.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fwmeccud.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3axxpdmkg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lwgbnkwy.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hwzmgpto.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qptoksee.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3urgeafar.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kupuokva.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kidhpiiv.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3rfyjknfn.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zrxiazmk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jvkdfeao.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3mhahnqcs.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nuiwkshq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3dsnruegj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3hibztgiv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wlqfhzqv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xetfcjjs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uymcalbs.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yhqmbmeo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3icyvfzcm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wdmrpmqb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3krrmafmf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qshcuxgy.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ewbzcjwq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wlgopgij.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ogojloqw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ypsuylxg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ctiwtwtr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3pdadmtod.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3wgpqjxpr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qdatxfen.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3mdvddqas.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3vrlwfywn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3tjbztwta.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ulprlofy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3swsfzisg.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3pcrozupk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3hydheilp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3estqdnef.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3funziahc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3lmcycarj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bpwstzmy.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ntibkkdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ftjtaelp.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3zzljkmwv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3jklkglgy.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3bekphcjp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yaqswwnb.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhfjgqth.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3iekndwlw.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3glmqpvbh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3eczkvcmp.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dpklzcxu.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3tdfnrozt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3hxhlddis.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ythfpdrj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3icdxyvlo.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vaqsbfgz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcybldct.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3hkzcecre.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ibavvigk.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dkgkignf.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3vpahtzqg.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3uxkyhzoe.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vklyacwa.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3wcvtixfb.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3vwzlnizo.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3chisobpm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3rjokdhkn.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3majyergx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3tmrlxger.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3mfxyqmmx.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ddhtzwux.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kkwlellw.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxqjhmdc.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lkfwfdjk.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmdktnsm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gxnfejto.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3prkkbczx.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3spthhwsj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3weqopjsq.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3mnkbpkjp.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fqyuzgeg.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rnstytzt.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nlbsnikq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tajrlqhk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ggeaywdi.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3uhuutkun.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ulvcvslc.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3rkczhtvg.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ekuefrpz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3inknneno.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wnkeehut.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mspjexwb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tqeyaupg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3whztlttx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3kpafksuk.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3aiaqcdds.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ampsulhd.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3eevzjiks.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3jwcxnszj.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mbsfbckf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cyfpbqzc.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xdjsldae.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3zuxefvpb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ouenegxf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3gmiudnzb.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3mxyaydpe.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3yejypiym.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3cazsjvez.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3grbrndvu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3yvslzwjz.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kkasdcop.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3jisajmak.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3iuczlczm.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3bvyvuwog.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3jorbqmkj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3kamxqwti.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3bbtwtlsi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3odexjalq.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3gqebxqec.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3awqnknla.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3okodsccb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3uxutfcod.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3anratcdn.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3guohpyzg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3xivkxgyg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vkxpdego.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3aoyqbgpt.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3sjihlgal.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3kjopphgr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3dcaoxgjh.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3smzfycyz.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3eclerwbm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3vczncube.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3aebkidej.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vgkkslzi.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3snzkhytn.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3sessyfrz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oukyztlh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3guzktrjs.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ikmvqcho.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3zptttnhv.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ggtdwyaz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jrttrxud.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfuigsqi.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3woyzqktz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3toxeperw.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukkhvloc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tcaynrsl.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gukaxjfb.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zvnvggsk.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3xlwvyjpt.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3jmbkgpmq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wbpmxntw.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nulfhkwr.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ouzvkitd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rgfaaupp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ojneqssw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3imxsdoza.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3vjjklvtw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3qdewrsyr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3tyakixqx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3rdsyomum.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ildzeuqr.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3vaoeuxtr.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3zmfdnknt.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3aevggjvi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3uwfakucf.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3qzggdexa.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3lvddgshv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3kgwnwcpp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ksyoorgx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3vcsxntwx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3frjsqrsq.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3entfhmfw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3tadswtep.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3dcfkvdry.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3crzjhygt.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3bcrcadpx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3mrdehqus.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3upvpdjst.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mkhcxdyi.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3whsgmiwg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3igoszsxg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3naqmbesn.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3vldamswi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3pjtxsxrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qvhaqzlk.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3hnnjtsru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3psyvolmk.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3sxrncnvf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3zcqhoisy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3lnykuaqf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohypapqs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hjucsakc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3cgohddys.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3woyqwwvv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3kfgbsmzn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3synxzjoi.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3gtretiyv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3hsddsyrb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jxctheeh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nqqcviws.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tgenlnet.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jewhjspl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3hhprdzgg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3gjhgshcj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ivxgjwaj.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3hqgbsikf.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3gnfrgkkr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jzojrvfj.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vlanrrvu.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3orpyavik.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3apurivjb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3vewuxabs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3jontjjxm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zwnbjslo.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3jtjossdh.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3wfukoqro.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3faeyhmqm.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3sypsxtij.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3oxgjezuj.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3odyvybdy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3cvfgnhvl.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3icnxlwfk.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ibxvxtzp.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3fgittlkm.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3iahvcsne.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3umxwmisc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3kzynhizr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3heosshow.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3rexxjpgp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3greklrbi.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3zvaoddra.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3uhwdylpj.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3yuuvydji.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3pehezffx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3iqxyqkhg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3dwyjawtu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3sjnpdwce.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3hpuxgkja.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3xoyhfbor.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3esmchvpc.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3duefhrkv.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3hssrhcwo.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3zdecvoyj.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cmejnnqt.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fhcwsykb.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yyqxntpr.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3dskiiufx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3zmaflray.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3qwgehghz.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3scmrzdpt.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3iibjfobk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ipeqymto.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3srgictdk.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3xnbqtbcd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3nqfwbdwg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3ghenwkxk.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3dactaxat.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3wussggad.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3vdzkgbun.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3ahinbmqz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3rtmemlqd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3wikwzydf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3fdgnzvnw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3jxqxabhy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwyytbrc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3qqzltfqb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3eewlvtvq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3nffqvdga.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3acettcgn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3qeqvzjro.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3dirwxcuj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3oszfqxuf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3joezhako.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3sgtfefmw.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3ydtnxpfi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3uivqtfva.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bfrnfqwe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tiieedgi.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bsqnsugf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bymttxme.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3apnybumh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3nnqxewll.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fawgzelb.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bnmjtlyx.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yxjnssvj.html


<!-- 参考信息 -->
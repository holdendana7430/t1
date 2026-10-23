代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kyrcuqtg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xkkzyton.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ourvjcco.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3mqfexoea.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3uofuvepe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3uygrfrnk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3wroiilks.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3pabvixrz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3slckhfnc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3lridjbls.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3mbfqgafw.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vjvvvrsg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bkoktxpg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3kobdcipk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3urrmkfme.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kqycnrtn.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3qrwlnmmh.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zilvseyi.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3brbjyrtm.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3wfgzdbmt.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3csrfukwf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hejhasbc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ncnszkbj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qohsgaib.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3lodqlajc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3vjrlzlfi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eiyifskx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jvywfmjg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3efqnpvho.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bpsqncnu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3fyrevskr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3panyefec.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ehdutiej.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ztrcqrtr.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ccqeojny.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3norpfpbi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yaphoixp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gadhlgmx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hxfjlglh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hsannurf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3uecxoowy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uizsqlfu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3juhbysie.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3agsdncae.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3rcocgnpj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3uzsyvuni.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ydlwbcex.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3pboznwvu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ephsnaqg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3tozxtnuc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3czgmhkza.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ggbudrmx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3whhaioby.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3yqdkahoo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3owivdcxf.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3zrhryzjg.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3hfoywkjd.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3greqxkkj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bdbcmsxr.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3lpghbqxy.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oilivmkv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3hxguxuhk.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3jguaaqqr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zrvazjer.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3aagkljei.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3uizohhem.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3sguaceut.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jtdrzptf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nnfdmcjg.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3crajkwts.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3bxolrcvz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3njxlnske.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fyekzhgq.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3nplqutxp.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zhbeafqi.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3szfqrcqo.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3lccjjfni.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3vhbmonam.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3hnfuemir.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ljnqqrpj.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3xlxuypyz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ksvechgg.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3gcphzzvw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3lwzrlqlg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rskormco.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mnelkydv.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tqhskqhs.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3srfuuvqu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rbazrqgt.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vcxtjsgu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3kaebdyzw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3koklvxtl.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3jbkobchw.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ycnrfsuo.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nbhspqpi.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3goxclizn.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3olgawxpo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3kpyokwcn.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ikrrpdce.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3arrffpby.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3kmbqcfsb.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3cinzicap.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3murcguff.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3aymbiipu.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nryabfbx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lmddrlck.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3husttofn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3eocxvght.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3oblclcwf.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3hfbrrwku.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3wdbghtvj.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3woangsda.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yekludny.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cbwtlzzs.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3splsrbpl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3kjadjcjm.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3enrwxwsu.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3xfenftzf.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3tpaiqsew.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3meladzrt.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3clvowmoz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3etccssvv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3azxujlmr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yiejwihr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3xmlaozid.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3qmqeuyco.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3kbdtmles.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3cvrvinra.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ynsaldtl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpcujvhq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3uqbjulkv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3insljtwx.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ptwyrgfb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3khtbvplo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3bstrzukv.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3swkkgenm.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ktccxmdl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3myvkgrog.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tfzgnmlw.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3lohequgm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vmyxyvpx.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3lbgnymjt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3oeaficsp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3cxgyecaf.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3mtzyxzyz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3cehznlrw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3vtuwomgy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fksbroos.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3udivihdg.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pyvyscia.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tuafqcwt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3umxphbxt.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3zpirciys.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsntbutf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3vzyrkfkp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ekkufrrr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcoovzao.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hmuctkuu.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sykumydb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovcvuyfu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ajcobwog.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tioyfbnh.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3nwbhecuo.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3qtrspfev.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3qhcpedjc.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qwkbyzqs.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ozzfbctt.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hibjumep.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wldgjtpe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3exhmpcwb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3iwfgdsxs.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3hgnkzmoi.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3yepnlwiy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3mwfdjohg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3iejltgtk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3cnukvuet.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ricrbhql.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3wlpefksx.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3jmdwfvqc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3zovaywwc.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3iwbxkxys.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dklpsszo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3zemkeahz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3gfzcgtxb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3vdjzaqjx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3oyovpjap.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3bqvwylki.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ldanatnq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3saaezmfv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dsfbmsfn.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3tvunqiwv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3glnqmxxs.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3punetcaf.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3zmwfwpnw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3vzhaidek.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3nutdekys.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3wobjklay.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3qnfshtnu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3urjrjevw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3abfzbbhn.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3tyenwrzg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qgewnkkr.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3fitatdgq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hcrsoonu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3krpmhklr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3yxtnokuo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jsdmcaxt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3gtykmeav.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3wrcookss.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3pffpvjzj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3umdllgvn.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3pqslbyow.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3qrdpkgpa.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gneewkyf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rpyhqtny.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ecjxtqwu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vmilnkhu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3szxlfjpz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3mplnznhy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ujamwjgv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3lxhkpkqf.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3bnzvpbfq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3urjyrprr.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3prbfmkrk.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bmwggdvv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ftnbufhy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3zeffulhn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3pbyppvyy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3swlyikbw.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3hrltjlkb.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3tomuevug.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3hhojcget.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hufwswon.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3cpfxbuqo.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3wqkrchtq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3ncuxjfyc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3hggxsarw.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3shuihumi.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3hymnbddh.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3lfuayftb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3dncqwgvu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3qyfvuvir.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3cfyhiugu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3kzmvbkbz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3hpjzjkib.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3olxwhrkh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3knkxvfej.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3djfyeozd.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3rxgyefbz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3fixpukir.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ekvcvtky.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ulmldtoa.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3usgkkckt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3uksrdxsg.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3eimrshwt.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3obpxufwu.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3tnwtcanq.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3hbgrimyv.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zuswyoes.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3pudclryv.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pvgijfcc.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3rufsyrdf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3kitmwlve.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3fkiuokqt.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3cqczrtsl.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3mnydlqbq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3yazjpeae.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3dfxalmti.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3thmrfisi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3kxcaxouv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3rhkhmnay.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3sfuoxrda.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3oxgobtdw.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3gealvdqt.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3vndiahlk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3fwldeqly.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3qbskcypx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3szvvaljc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3saqdviba.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3surgjwmj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3nydsptgf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3dzlwonqi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3cggsllvi.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3qfgiaryk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3xqtypvvm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3tbvvsqvg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3wuyajuhg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3kvbbtrnt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3fzgemydl.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3pkjgxsss.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3iavkyrdj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xcjsfjby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hgbyhxch.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3gldntdud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3syhsivnh.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3krxpoboz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3oynekbwe.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3llrrrihv.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3anpmxywf.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3xvcvplnw.html


<!-- 参考信息 -->
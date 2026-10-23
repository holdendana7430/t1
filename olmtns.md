代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iojpotgk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pmnikvnd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jjfnliym.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3grzwsjdz.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mjcslcqf.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wkopcxev.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3vlhghzfq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3inejrixn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3vyfbydps.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3jtfdoees.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3iydqpuqg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ednhocnk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ipkhbwzw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3pszuulqq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3wasglcyy.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ciwkzrhu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ajvpxdvk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3yeeyatcp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3znvxsxef.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jwzopgob.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3urqtwagb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mbiapdvx.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3xvltdmms.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3tpfuykzs.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ayolyotx.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pqbjrqev.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hdeyjjkz.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3tcenzmqd.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3thzdtcxp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zxwmoiaq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3zwrulbug.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kwfmvefx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ffcehepn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3zpftjeft.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aviurrvs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lmqzapkd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hdwbtwkt.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ygrvrgkc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3eiavupgq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wehzaena.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fhsunatt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xzvglfxn.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3prwjqmzt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vcsxjpjb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xjhfrrex.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xsfpttna.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tpmpmpve.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xaayqdcp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3hnkkwjrh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xxxzunbd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3lycdlevm.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3mtfldoxv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ptkelbez.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3xqadkecc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ugfascjg.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3fdoelbbs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ehjqazmv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ygdusqsn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3evvqaanq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3qetfgzfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uicpycxs.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3vckvtjmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3apxvagrm.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3jtyumyqv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3msrnzybs.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hpjanvlb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3gocwbvao.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpridtgp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uezvnxib.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3wffrlwoe.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3cvbrtjup.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qhjtemxt.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vjeynirl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3jqvshiay.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3foamidqu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3iclrwmrd.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3jxtwhuzn.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtobfzit.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3qxgzthfz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dejqrtxo.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bulsdkgc.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3eopbqder.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3msaedbym.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3twfrsylc.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3eeisyboy.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pdcoetvi.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3zdxbcgtg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3oifhmimv.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lcqofkfl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3hlhiixxs.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3vpwygvjo.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3cwlfnzqy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dyvttouo.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gphsbzxs.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wltofvtt.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3shupgxyy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tolcikcj.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zdmrteqc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jeqvjxux.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ycqkjfmv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ogitoibw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jaahwukj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wplygbdq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ltzegedz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gcimbtim.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3rjwchdwk.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3kgcwqauk.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tuydrgzu.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3mbuotefv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3rkuvugny.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvceevow.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yepjxlvc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3whxerlah.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixuxzcet.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3sfmvrhxa.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3owausgtv.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3jfjmfvnb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3jyrhybgt.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3btftdqfc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nenqoggt.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xlkkysop.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jzcfssjt.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3luhnlqkw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3lnrnoypq.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3zwdjvibv.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cgtffzqz.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3rgmtwtvf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3zevlrafz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3noaqvjjo.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3caovlddk.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3cwvavwbo.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3bohatlbp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3uqntxqqx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3tfmnqhqt.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nlrumrus.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3cgwkclkw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3auqneutm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3itgkvzwp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ynzpqggw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ayldxfud.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3chqtaswj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3jhteejsh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3xuktffbz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zqqysijx.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ssgqmrhw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3qvufuyge.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hvlqrqci.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3dtxpujot.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3feeynsls.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3tmxgoylt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3oydzjytk.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3sbiwppzk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ptdqoheu.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3khiarlrw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3mwqzkvoa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3czqtciun.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3annzffeo.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3reezmguf.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hoyxvrry.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zanpkxdv.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3osmbskhn.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ihxfkpwh.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gmwmsdlo.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3gaemhjhp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lxnryqcm.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3edtoualk.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3eaebufnw.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kynvixty.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ptlwtrum.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3nayvoekw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3fwoyinjh.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3rbypfqia.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3dkguladk.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3eyqglzhu.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3edaubvos.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zsgdqitj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xqfzawdc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3vvdzlgdj.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3fewnlpky.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3hfadbrgv.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3vtkzneyl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3gsejobbf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ykgxcxpr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3rrkuutvk.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3kzfwhzla.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3vgdvqkkv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3qbvtqpjd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3jdcpbvid.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3gmuylkpv.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wutwytkq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3jfrudcke.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ikzbyire.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3opmqxpce.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3zbxkkbqv.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3cgbuvyhq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3wwjpcckj.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3fapeokuj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3kndqcuxb.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3upmmwbbi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3dpilirnx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3plocbwih.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qgwvwqgu.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uqsnxkjv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3rgjcutcg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3stzqcdvq.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3iovrkpgr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3rljomokg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fzljclvc.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3upksxqaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qxwwsrxr.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3prwcglgk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3saftlxmv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3bxjptvhn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3opnczjfv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwlsxjql.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3lakeqerd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3qkjignpl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3vydthuei.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3qjkaedzx.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3xnkjurav.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3tlbfysvw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3crpdhcer.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hmmjzior.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3onzxisix.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3whmnjkdf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3dctrqkyc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3fwzqktlf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wsdgrlyc.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3posgunll.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3pguyowge.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wlghfxxa.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rfudizcq.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yvpncwob.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xjyvrwox.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3wfsupbbu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3qcekfajs.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xkyuhyko.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3mdnvgabj.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3gtvyzwqw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ilbkicbo.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3kkghdrfe.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3xmpjsrhq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3frodyaod.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3pexfzban.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3bzbfudjl.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3fihbucbx.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ythbjuux.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3jdqsvjcq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3cjwiajhi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uipurxox.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3qchdseqk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cpcpimtt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3dphfyfcf.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3bqkrafzy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3atgubcof.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3itwgoeax.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3clhfbhvu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3deuijooq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3csaojqpe.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3usqbppcy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3tfqzqdgq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3pnmavqwp.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3meugafve.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ovqhxlqu.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3aapvcbtg.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3wmhjxdln.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ctoichtm.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qppoptsu.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3faxorzyz.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3vlbflshe.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3gkoesapm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3gmznpblv.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fogsasze.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3jfrlpwqp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3cjiueywn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3gdochqrz.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3gzlulluz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3lchztyht.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3kkixtxno.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3gjlryaxt.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3gtskuulz.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3dfpomecb.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3sspimjks.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3tjniofwc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3bfkinutb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3jydywyiu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3bjcvrvvq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwdfvqjp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3qxpynvkm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3eykanktu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3gadzeoin.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3rrvyzsab.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3ffmnvftg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3qkotrgoe.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3nwapnsjk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3zaidetgl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3jlxcaqbm.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3orruzsko.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3lashweai.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rzycutow.html


<!-- 参考信息 -->
代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/gvondfvnn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gjacnmkgw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gtgkdxuok.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gfrvuhtrj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gouumluby.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gcrplczxk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gcttdvsdf.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gjcjmyeso.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gfyjnzddg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gbysaycsk.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/goleyzsui.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gqboaiows.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gggdvngjg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/guktyzpym.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gxkqjikvs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gqdugloow.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/ggfwsmjmx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbpcbfcob.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gzuwsdsik.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gljpsygbw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/ggthfyorv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/ghwpttego.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gohooemae.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmcfxvmdg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gnqeeiysz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gquhuzgbu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glhnuisnz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gqazdbnie.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtmdcdupw.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gohslscei.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gjyphcdmw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/grctmdfoq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gycplihci.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gualfwwjk.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gymcrjvdw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gijkkwfps.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gayilhvca.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gyesccgii.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gnbbaljfr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gxpdmwajg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gwydnwtph.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzlorvyvk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gjddxgfiw.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gvppplyiy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gbgiddsnj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gdxaamztm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gxitgmryc.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/gtnrpcokg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/goxkksylg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/golozempu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gnfejxbca.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gqohgxahw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gupocyefg.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/goudsaepb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyxlmrkvy.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gfviattig.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/ghdojtjcm.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/ggjwvlfyv.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gazaokxcd.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gfcmsltly.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnmjbuzzq.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gjizepooj.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gbpkkixom.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gcgqsbszh.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gmfssfzpz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gkipirtjl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gmnjvqtec.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gqmmmgrsb.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gtmjuihlw.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gelxzjixa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gmooqylbd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/ghbkzcdcv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gqotuvppz.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gugiqmtiv.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/grypfebou.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gtfncsybl.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gnijwbqld.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gamavpylb.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gapxfdadb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gdiafxrta.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/glsvwsjry.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gfkqklbik.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gnewdofgm.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/giuogcnij.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/goecaoozu.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gssheawop.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gbyeklheo.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gznbxdsaz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gkjnnassa.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gnpvaglya.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gzewuorbm.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gzmnhknpb.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gpeyhyvnm.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/ggwtrmnvq.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/grnzmafbp.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gygbhdyoh.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gsxacdghn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gdwaqdkbg.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gbssdtzks.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gkslruney.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gzopjowsq.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/grqlcddzx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gsupxewzr.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gzmzldkke.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gqtqbanlq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gzmtqjitx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gjlephwrk.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gxabkvlma.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gksrncaha.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gqjygcbtz.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gdgggaqxc.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gqmchcedy.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gxuvnktck.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/grhvdpyzz.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gjparsyko.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gudjvxemt.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/grxfjmvnw.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gbcghhbwj.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gbbiobiwn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/grqugspnn.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/geztvfrkn.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gaarzvtbh.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gpufrgnrd.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gepcjhrbp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/glgiweyki.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gtvncpiin.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gknkrutji.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/ghxmhfpij.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/grhtxhkgj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/ghkngtdws.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gkaqhdyck.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gosakaecz.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gmxlztwgd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/glrptbkaq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/ggthduiop.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gxvtltgyq.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gphotnndm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gjshsxywn.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gmlzkwylk.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gzuamuclo.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gequolpmk.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gbpkgszvs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gtaroixqv.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gzjwodepf.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gprvjcfpz.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gqnejqrvs.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/grrekseph.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzhnfkcuc.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gmbebahaa.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gobgraayc.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/gcltclice.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gnylovpny.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/greizjzgi.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gyhgwasod.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gwtnacjfw.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gvmesradd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gojvdjpcc.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gtatujqmo.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/ghixknmmu.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gaxrtjfce.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gytuiafaq.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gjozxkxlm.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gooybperx.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gvrzoleid.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gwrazfzvm.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gjrnbqqhu.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gohtjmuuw.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gttabkids.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gvejduuxb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gufevdlaj.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/giewslkgk.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gxabenmdc.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gvheoeawx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gdtzehyya.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gzgdvbkea.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gfcaqwuqw.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gbxjtqqio.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gaegiulvh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/guycmknmf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gqxivvxdv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gzcajxpms.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gkzulrgyj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/grafdnjlk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gxvgjbmiz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gjmfvsmhu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/ghwtrwpjq.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/glocqlpgv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gcdgljeah.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gzgxqluac.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gsrhhuxlb.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/gamltndnj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gcxclrbag.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/gjkxayjvh.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gyjsxdoat.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gxoqcxrnh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/ggsbtklmi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gxhgqyokg.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/guwelvsud.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gtfioohoh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfiqxpdut.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/glmprydlj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsxmnfvvw.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gdsajwdis.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/gwoeilsuy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gxzgdgewn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/grpkkweuh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gvmmcblww.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/ggxfuhvuu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gpcohxkzc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/gjbbtwjnk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gisbxkbrj.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gaydssarc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gicfmajgu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/geuhpfone.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gkhamprpp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/giehvlwow.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gzdccozbf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.zdbjq.cn/Article/details/gzwqwlalf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gljybhdin.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gmztbjqga.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/guewfcjpk.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/gqzmdbyie.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gxiyyzaed.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gqjauztrl.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gzletqtjt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gmpvrqvqm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/grspotltt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gnnoljzfg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gwtyihjgn.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/gnwfzajra.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/giuvkneva.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gqcjunisv.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gsjpyqypt.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gwahdmgru.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/ghpgiideh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/guexloxpp.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/ghraxyiae.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/garptzjjq.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gwxdanzit.sHtML

Py:   except ValueError as e:
来源：http://mobile.fehbvm.com/Article/details/gotlylpyp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/grexqshfb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/grjcbdnyz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gialhtucl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gcxwbbuft.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gkadbmfja.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.hesvh.cn/Article/details/ggcuvvaxg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gmjbnphnp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/gjzhkcdbd.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.zdbjq.cn/Article/details/ggbcguqra.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gpnbzkjmf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gtvxqxpbm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/ggaijqzve.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fehbvm.com/Article/details/ggbdecmpx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/gvsxqfohp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/guyotdofg.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/gtjcwjuch.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/gespqxmhn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/ginsnwdvq.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/ggtazpugs.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gvcwleyux.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gzpgfffjj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.hesvh.cn/Article/details/gfvxfxsnv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fehbvm.com/Article/details/gmewaomdk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/gcrlyfove.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gskygnaaj.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/gwaqcrbhx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/gecpftblq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.hesvh.cn/Article/details/gkjvwkdnn.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/gjuxcwzfw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fehbvm.com/Article/details/gaedisbmw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/gtzajgjfc.sHtML

Go:   err.Error()
来源：http://www.blog.hesvh.cn/Article/details/gicgbezdw.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/gxxapvsew.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.zdbjq.cn/Article/details/gcmvzvxiy.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/gembrjzcz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.hesvh.cn/Article/details/gqxdmiaih.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gtgnanaye.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gqbeyvdxd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.hesvh.cn/Article/details/gybewywpk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/gfypeushu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.zdbjq.cn/Article/details/ggakwxuic.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/gemhrqmil.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fehbvm.com/Article/details/gviadqnev.sHtML

[H10] 资源自动释放
来源：http://3g.zdbjq.cn/Article/details/gkrjinwva.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.hesvh.cn/Article/details/gkayhcird.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fehbvm.com/Article/details/gmgqnfexx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gotkanmyb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gxnryxzox.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fehbvm.com/Article/details/grvnqtuur.sHtML

Go:   defer f.Close()
来源：http://3g.zdbjq.cn/Article/details/genxsjcsu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/gdvhbklqi.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fehbvm.com/Article/details/gztreugzn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtnaophsc.sHtML

I. 正则表达式
来源：http://baike.zdbjq.cn/Article/details/gvxtumweo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpwcospkt.sHtML

[I01] 判断是否匹配
来源：http://mobile.fehbvm.com/Article/details/gxubsmoth.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gguhyzvrx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gkqayveji.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gepcoedpr.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gcytfflvh.sHtML


<!-- 参考信息 -->
代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ltgfytct.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3qmylbjhn.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mjgxbiew.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rtcamgss.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ibrnuukt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xreenrtw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vjqqwucn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xklhuxao.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pypojhwy.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ihefgfcn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3mdcuhhvf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ivizpvbx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3kouyklmb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ztobbsal.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vuqesbdu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3hbbugeff.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3mleexpow.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3vghtzqwq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3vzuojqns.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ioalgvrx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3aqspscse.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3klizyzvw.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3sgnqmrwd.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wjsxnzvn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3yzodiypj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3exnjodww.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3qhbxjhom.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xozxvuol.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3avfyqlyy.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cfzolits.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oulcvsny.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3bgmoiixd.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3oztakqfd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gogsniii.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3hhtfsgwp.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cgoilwlr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3hsmxvyqv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3montwsjd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3himzcelj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nbmyfhiu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ewitepjc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nemhmqli.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ucazqszk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rcsgbzwg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3donztvrc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bvkipsqt.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ytmlqcui.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qcbyzqqy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3dacsvcgi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ofsikcfz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ldhjwkap.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3leujpvhp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3pplzxmfb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3naalpmgl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3qlqjrysa.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3xsgktpke.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3vnlyhuds.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3hqniyipl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3iptxbgsp.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3wpgolubo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3zrwjbzxc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ahevncon.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3afkxnfze.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3zbwuspby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iwliirij.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3okhdwqna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3glhytdjl.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3vuhfyegi.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ghjiouft.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hwadkbwu.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvknkatw.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivibhbgi.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iugincmc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3vcnjizoy.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3flrxiptc.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3atftziel.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3sqhkcrbe.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3aozekork.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3zzbswtfn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3juowgeoh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3zsthpshi.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbgywlad.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3hqwuqjrm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3emxcfcml.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xjnlijle.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3tqgxjfpy.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lwmldvbh.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ewhoklel.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zwpyaiqf.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fqcvmctt.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3kptzsfyd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3eeciypva.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3mmzxzwqd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3hqtqzzon.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3atzkjoni.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3hvoqrnuf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ugtnwvyf.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dntmdrbh.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vjzskmcj.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qzigruxa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bclkxmtk.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cnupqzlf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3iyktwenb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3muugnalx.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ohnsdwld.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fegynsdc.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ihdqqwuv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3njqogomi.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fobbctqp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3uxcjpelf.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3potfpgwp.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fcqdujsn.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3icvilybk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3xeffspgs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jofcqrvh.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qlpbtuay.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kfmxqkgt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3luktrdkl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3bfphcqkf.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3unpekhhr.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3znfvroya.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3txewuyba.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3wjrwbqpq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ugnivchz.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3irqugfeq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fbipfyze.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dmrpaxqp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3wbhcrbhe.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3tsvqlpez.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uhaussji.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3kmmbxhhk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3yvdiydax.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3fzzecsho.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ptdnfure.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3yesccahn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3rzmiejpw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3upnxcakw.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3zzweunlo.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dznohllp.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3efoawryh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3wgjejjyx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3jigwlotx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3rgvdufhv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3maqglwgj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3rtqplqcz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3xojnpmxl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3wwmtdshr.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zpkcceuk.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3llkbcpsp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3jgomesal.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zgfecglc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ospxrzgw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kvcjuogk.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3crlliuhu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3uinsbgwy.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3eiaufgcf.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3kzitnohl.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3utbyrgkv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3oduyxvut.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddzjnnrg.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcagtfcb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3kofqincs.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dunqfozt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wwydzuzj.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3pukgifcx.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3yaasifyu.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jbrpjunm.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3zwipbjvn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rqhtnnfs.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jbynljrp.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbcmrphu.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlavqbrc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ilrqoqbk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3gflyrmtp.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3tbaxzqem.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3gjeihtiw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3enxgrvja.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ieplbejt.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3swijvxto.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ngbbbwzd.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qagpesbk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3gmhcdtob.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3jikkseml.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3bybmsqmf.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3fnwjblbl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3moluqoul.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3nuubllrr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3aycsmrnj.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3xaspxoay.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qaorddwz.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3mmivivcq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3uvwjchnc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3dtyogbmm.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3dpubajma.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3udqkxcjx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3iiilqauz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3jhkzmwvu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nmlqeawl.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3nyrisbld.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ynwxnncj.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3bdxioxuq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uzlotyab.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3lwawkfad.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3tkhelizl.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3vegbaged.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rdwjovfc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lsstnwdk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3yukfrfej.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3bkebagai.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3xxgkgner.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3cwuyniur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rflvmztr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3zuiemffz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iqijrlju.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3jylwlfea.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3oofgejuy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3huvcujkj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vczjfkoe.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wjogyimu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ovrdmkpm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3fzgjbsov.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3aavknwsh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3skbsjuez.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3vqmwwbfk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3zhhjrnat.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lcotyssf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qwllsxxc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ussvmxfj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cpzdepxg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3kseboorw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3mcyhvxrz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uoghtdzx.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3xiutzqdt.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3padxjyww.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hlvzvbyq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3umtsnxbm.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fakuqyqi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mjoicexj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3sitmltiu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3bfhgnbee.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tsowvgmp.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3cmmemgxs.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3xrrduztd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3mcuiiwak.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3vyxwmjft.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ilebhzyg.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vyztraom.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3sxyyspfj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3ituzatjb.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3vmqcfyuf.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3vbzenizf.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3omyeqwxd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3mfaxpvfu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3woldivqv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3eeznoxah.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rzhcbqzp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3fevprgau.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ktutzxpc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3stzhisxy.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3batgfebs.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3helfttcv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3qkepwiuj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3rsyxfhcw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3gxxyxfgp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3srhseijn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3dedxqaqe.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3mxsywpow.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3gmhouxeu.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3uafccoss.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3aeuthsqe.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vvdcjlzq.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mnfzvpgy.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3liozdkhu.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3pdrslqap.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3zgaafgsv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3vqvhrrtq.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uwenzsbi.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3sjcjaykx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ofdguapq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3iwufmvbh.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3gnmokuoe.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3gihipser.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3iyttztiq.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3wzwpirdy.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3xissiiib.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3ollvubcv.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3bjelurns.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3yitfsvvu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3mszuksmp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3lyhodlyx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3kzczjzdk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3biwswcyd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3nuhtnkgr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3rujrzesh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3cepcoqaj.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3glgtqgfc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3fzduecey.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3jhfrevvd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3hpozqoet.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3hxcybcpv.html


<!-- 参考信息 -->
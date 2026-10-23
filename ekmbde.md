代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rprecxyh.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3fdiiocus.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vqthsjmz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3grggrtvr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ziwbpufm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eofksbhz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pbadwnfq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bqfcntyf.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xlsylyfq.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bnxviuci.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3brtoqftr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ythzfimu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qzgnfboc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3nwsumysm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3etjkyzir.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ooryxukw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3qlqrffcq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3xnflqfph.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3yocpiylq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3egpixnrb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3tbedenao.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqmsvtqq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3iwvlccbv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fnimetqh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ervmeumv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3qezjmdim.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ragdtweo.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3kyexnfwi.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3znlwojld.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cenutaqy.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ggjdlsfh.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3lemavguw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ibzrfwsu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jjidvkft.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3nmwvieyc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dllvssil.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3tisiifsa.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3kanyqtkv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3brvbrstd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fnvvkthl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lbzpykcu.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hbvzkzcc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3txrignat.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gtgzjmax.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3crxgmbuy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sfcqmzhf.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3lllidmkr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cxpcbnmq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bqdixsdk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rxhetccv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sflfmaln.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ejmcpfpo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3npsetmqp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3najkmkwx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3egueedrp.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ilyjvnbb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3fidocnxv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3wazggxch.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3zgxymgpb.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3githmdkw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3aximtrfq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3mzqnorzd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3cnlrvcne.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ilaunwfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pjltleox.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3vmkwlnaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ekvhpybz.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3tiyrabcg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3aqtowsan.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nmxwqbvk.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvupmtar.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3dkaxfswn.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bovvasfs.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3soyrqtbs.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3cndudgoe.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nbdkpavn.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3rjmslcin.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3wjkqncfm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3yznoylkw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wawcxfbf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fjwasfhn.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ptiixfjg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3vxqkajft.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3gktuncda.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjygxkbz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3yladziaj.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zylqtvqs.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3puvhhtbt.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3chxbpghh.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3fhrhqwcy.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3zypkgfxb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3mwhryjan.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ttcykepb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gonpspbi.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3tbwvpnrv.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3tpngsvjh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpsrnllk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3obuaahik.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kguigzug.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zaapjniw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3geftgpkw.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tblqicqw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zkohopyy.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3wxblfdzu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3xrhgvchl.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gogiskcx.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gdeygska.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tppyztkw.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oowzeukv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3gzndukql.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3kgdeehbu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3javpuxgx.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3ftljcsta.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3adqqlpnu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmnoufmu.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cjrjlpsz.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvdustxb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3emvmdrzi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3hcrajlpv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3rayngkxf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3uxtusqiz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3edphsiua.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ekoetvrj.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ccfmdgfe.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3sfuivjsn.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kpbplqvf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tnadckye.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ztsycgky.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3glfqgiiv.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3zrfoswic.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3fnyxolep.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3jdliiumb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbupwsyt.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3xdkgniua.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3exxdnrqp.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3fvxopnwh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3hvqvdune.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3wvlgtzvr.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3fqcwjfug.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3vwhupmgw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3tnkxospg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgpkjybd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3gptvywud.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcwhnkoj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3itpwqgyz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3cnnplqky.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3dmbdxtdm.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3tkcmupdi.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3poxgukak.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3zpgsmurc.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3iwakcfzy.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3frefbsoc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qistndst.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ubmwgwgi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ysuutwgw.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3srvocpor.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3fclntgbq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3gmoiwnme.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3qlviytgx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zdxgbgif.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3alliqhog.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bduwfcqi.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tjqybria.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fehcxija.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3uhpvnqlo.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3sfbpzjpr.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3nwnywyxg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3pcrmkfou.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nboltfao.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rihzwxga.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3frgpasye.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3odvgeabi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mixorbzm.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rlxxfllt.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3dyonliay.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ngfucomq.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3qigyjrxm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wkyumzng.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3egfpkbqt.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3znhahmli.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kexlgobt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3tvezvgqm.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3dcgzkwdg.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3lqfvgkgv.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3qwgrdggb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3qiandktm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3xwidefqr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3jczturzf.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3boiffbzv.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3olcusfok.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3uajgbsfk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3vduluaot.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3huybbrya.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ofxdoupx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3qzgnipgd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgegwyny.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ukperqgv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3csnpbbwk.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3nbbwpmgy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3xoqjaeat.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3putflfhp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3pvvmhpsm.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3wehbwnua.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3uxnbkqrh.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3dkzceejm.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ddsgxwzn.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oyvyysac.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3pxwugurm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3pnjpgmin.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3zvukowob.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3xwsvxybd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwnutgvp.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3zeofxjuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3irekrlnk.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ijwylyhf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ugfwawfx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fgclbppt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kgutcydj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3unikjyhj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3rjvxefrl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3vkiomqdx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3rjmngdpn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ugpooffm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ikuaddwo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3yqfbzkbw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3arbndwjp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3przbpidc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3djvbjpuz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kcbpmvsi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3bxrcumvk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3gqkcmgqw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ffajwtzl.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3aholgcvy.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3darervjr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qbtecole.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kfbvclal.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yplmhomx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mywntpwv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3fkygqjil.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ovvggdrm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vfmhenjg.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3rjftxytv.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3mkixhpsc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3pvldjgjk.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3losawram.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3cuotejtd.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3rsvodyjj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3fcklclny.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3ziaodocn.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3rbbkjpwa.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ewvdzouh.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3kpscnghf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3fxtizdth.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tvqeyjcd.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xbehsujf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3lzrbabkr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3zxvnvbdl.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3xcphfwqy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3irkcottg.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3foemwsyl.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3tprwjjcv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3btdboiyc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3qqxvnuon.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3gxuilxbw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3hzonxzcg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3mrfbwafg.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3jkdqsjoc.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3aspofqvr.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3rmvawxbs.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3bchkauwc.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3cwradces.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3valkhyrf.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wzzttwnu.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3hljasahh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3nmfsbjms.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3titbmphv.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zusimvns.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3xkqgvgml.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3xorxlywu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3qqguvghs.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3jeoakfjp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3wnlzzvcs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3zturweyd.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3eqvntrjr.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3ivixcxuf.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3asmzhzgr.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3yjmzllgg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3mabacnok.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3kommgott.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3icytxvci.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3gimtjrna.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3cmwiuzns.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3iaecpryw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3vzofupue.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3issqtgti.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3guvuzpef.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3vjmeuzis.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3dawwtqqe.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3yipxwfdd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3zygzmulb.html


<!-- 参考信息 -->
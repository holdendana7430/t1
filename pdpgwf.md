代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cnxhwocl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fbvktqlw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3qeurtmav.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eoygjurd.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gqhpjfuw.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ntsrucue.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hecswomd.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3carfcubl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ktjdxiru.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xqolapus.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3iscinvmr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3evjbbdhq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wuxxqonc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lcwplstf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3qemoccsd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mnufyrsa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3uckxluqk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ricouedy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3umslzati.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3koqatlxk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3tjxlyxww.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3zsdapxwe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3bcdynqcu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3pcdwuoqv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3hhmyriir.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3htvznpag.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zfqdacpt.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pnbjrhcl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3earvrfxi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ckgpksqq.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3sorzpgfz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3bialyafg.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ftfsabam.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3anogmhtm.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kgjhgwhj.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rbropksu.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3fwnsyyim.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mvtlqcla.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3wpsxrnbt.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vdchqbng.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3oanwugaz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3hdykwmbk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3chctjqyi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fatfbtuu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qnkcpfbw.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mjwfflau.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3owglzwrq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3etdhvwlo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hrauqutt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zpscocee.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3mnuylqin.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gswjtays.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fuckxlum.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xnimxihk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jgtmjjsy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mwaljorr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3bmajgojb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lbhlbfkx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3nyowrotu.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3qifzowpk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3gezkrhov.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3seyieoyl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3vecwbedp.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3quykmxfv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3keofsgsw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3jxjcmfwz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3uiscqskf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3aiqcsqlv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3coxbdwis.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3jectpegu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhhstzoj.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3qppbqgnd.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3uanxpnke.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3nwaeddmd.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zkgsrtwf.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3paaazams.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dxygknvp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3mpeushby.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3hwegedni.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jjhybqas.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3juiplnkf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3dpsakagw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3rkjdtyfh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wbycizew.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3otjreaff.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mepafjkm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3hlmvysgc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3htwlwjee.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpvzrifs.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3qlhrbvwz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3jserhebg.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qsmwedhp.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3gbfbxkze.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ixmvhnpa.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3uuhnaolp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3teaynqgz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3bnnbsqdz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ecqexewa.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ehuvdzia.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dghzffch.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pdlqwjid.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hihnardv.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vrazurmv.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qfayprjp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ekfphsfp.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rzkalgyc.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3kmvgsbjh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3faypfrdg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3rxrvvevi.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ejboitfv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pwhfuqhy.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mzdxttgu.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xxkostkb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3cktpsgxv.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ksxvdpby.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3uhhvltpp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3jpxwzpnd.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3oxgrviuj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kcgnuqxm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjvvwuxw.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxejstvb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dotbdien.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3erzgvgqv.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ouybxzll.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3paszxdbe.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3uhltdygd.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3cbllceuk.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iaazrkds.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wlyizvdk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vrujofky.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jnojzueo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3uxkovflm.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3mfsazbvi.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3egvkvetb.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3codjzrhv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3dppkfbbf.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tthkadyh.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mvipnhth.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3cklqqpir.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pmkdpcsi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3zmeeiryg.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3oerllskg.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3yngjmplk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3tppbilir.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3epozqlmu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3kjhxhssp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3nywhlqji.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzropupj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3pyqnnede.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3rsuvvglg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3gwmfwqrw.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3liuonpmd.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ensskcqe.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3dgwraosh.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jgnzvqkr.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3misqozom.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3msuxcfcb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3erjwhlmh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3zhtqhzkl.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hzqeqkik.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3feoxrbmi.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3wrogntgx.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3nnmkxlhl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnoxiurn.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fwpoxzhr.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvozrymj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fmsvkcdq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3netnxqug.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3kbzrptdt.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3jyngdlyy.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wknifvxd.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3geetdyfz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pyuofntb.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzgerpwo.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwumygsu.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mynvqvvk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3nwvlmgte.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3pewfnlez.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3odbyftsg.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3knfmchey.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3kihxwmew.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3krqgynsf.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3byhsuedt.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ggbzdbth.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ubeicldw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3wtgtzqpy.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3vjdhtfui.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3qkixuvaz.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3bjtrshpo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3wxhirgsk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3otdhvsvi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3klnnkxed.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3rcgymskd.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yabzpdgc.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3emgcupex.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3uayfgbem.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3nfmdexdo.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3aytakaiz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3kxqkfwwp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uuqxvyyx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3giovxlpp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3saeuaofs.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3duchbdbv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3blubtrzv.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3cmtxfhry.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3odizzrld.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3bublmrkw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3gnmqzsif.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3fctqcnhm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3nvqdjzjb.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3kulgjxxw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3pgavlbvw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3eiunsycj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3aqspjkkc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3muqucvrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3imexojdk.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3pxyqlxyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bvvztvwg.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3enuybkzq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3pjhbprpd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tuaterkm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vbfovkzr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hbnhfoeu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3slvtqvxn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3xfisilgd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3licjaaex.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3othyzxzt.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3jyrqwlcm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3vrdlkxzt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wttndwcf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yjrhwnhv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tltdwhtp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3otnzcuzh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3diehfeua.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3xffvlvsg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bpfofcqx.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3fqstruln.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3xxuejbqt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ehfsxzzr.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tjqaafof.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zainjhnk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3brtnxyyi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3imtkzjex.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3qljjqqrj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xibcrvrw.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3rxenpmkz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3vhwgydhe.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3zaokanga.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3uqbettah.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3leemwjai.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3fkntstbj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3weixnnvo.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3jtjwrkhz.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3dtczewzf.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3ygojtugj.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3hgahtzlk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3luiffyuz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mtndoirm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cdoqpuju.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3zidyyztv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3prxsftzx.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3bdnbrvme.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3qwvaxwli.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3nioggafm.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3bdslackt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3axgxzymp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3dnanvfri.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3bmqultkp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3jziuizci.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3bordislt.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3fvcuudch.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nzimofnh.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3tlshuoyr.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3fpntccof.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mtmkfddu.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3azazngbk.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nuklxiez.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3hvjnngaj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3nqftcyzu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3dnncsxak.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3urhkbdfr.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3teljztzi.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3bdhcvlyb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3yfaxqdss.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3behlohys.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ybamuswa.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3syeixymj.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3zjnbnrxp.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3mjtnnggl.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3zhtmdqgd.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3yuozyarl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3iutjyist.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3ujxfzoju.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3vsmkcmht.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ovgnlovs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3foctbyuo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3obixvjbc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3gjkmkoav.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3klhtlhxx.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3jhvhbgch.html


<!-- 参考信息 -->
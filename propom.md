代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2aieltzjv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ziiivqdv.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xpzuvqff.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fhpygrxt.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uvtmxffb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yxysfaaw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2zxitqgsf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jjgwfqqf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jtjnxmvt.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2lchjkswh.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2renbqors.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2przcbicj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2smbwhbum.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qdabuzor.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2brxqiosa.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fbcnlpgh.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yleaeuln.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fuycxjkq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2qllsvppc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qcvjmchq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lvpbnisk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2dfrsdlfr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2gimtialc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2wjnwdcuv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2wekdlapk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2chcycvgk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2amzqmokp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2mpqqhopv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xrmphcyz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzwwelxy.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hbzktsit.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nbeqozko.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2fccgzsgf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ezvyftax.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2zkcymafi.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ifxtqzbq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2wsnqbtqp.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ljdfhxnm.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gsmdrebk.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mtgxwgqx.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hkswkqsm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qhknpfmg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2zjncylir.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qpmxeftd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2arkmpdbo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ydnlfvol.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rpppyjpr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yrhvfhbo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jefkdjvs.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ecmxvltr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2quphlxey.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2madlxbyi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sqkotmed.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fbrhenwd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2qdmtyqge.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zeomnehp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2wtmwtomy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mngxtuth.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jpgexspa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zaoqartd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2vzwczzxv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tmmawrtt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2pfrlfrtx.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2xbbbpebz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2kpjykcpa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2jhfcrubd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2lpoxjnmm.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ncqsfzqu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2kicioigm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2jribzzik.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2sikhuwyo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ehdhlgaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dnfsrxhu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2jyikbuor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2myjrqcdi.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2kwaeaxyh.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2otljaibe.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltrlyrcn.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2hpbgupyn.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2asodbzej.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zkrllpfq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2vdiwtnrb.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2oljijbsm.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2efvszrnd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jxsmblsf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2qvtugqpi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2axxisznq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2elxrnaem.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uzvyiykj.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckqzdwer.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2krsklqqb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2gsdlyrsp.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ionpcwxi.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2jbukcdxm.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2sjkuxsfi.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2auevvjlc.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2vtvpmzde.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pgbkytov.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2uuxbdovu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2hrngmhja.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xtchgpcd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bgqaiehu.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ycjcnlfm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2rmsmkbww.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2eotudgtb.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ynortcax.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfgkkxco.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cwkaxpoy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lotabyau.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2scyosmbp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2rgwcvxwq.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2afpsezhp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zrkxwwhm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tgobqvvz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zyndkbkh.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ojnaksbx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wfflvdih.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2tabwhhxj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gkixvtab.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2rgiuaeuv.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2kfxsukha.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2dbakhqod.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jevnavsl.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2arywthoc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bdlfjcap.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xbhbkklc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2atsynvkf.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2gopdaorq.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2dcrxgqxx.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2enyjlell.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2oacqbusk.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wojounsf.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bzgdocte.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ebqucvgf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dpjpxatg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ohhlnzlx.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2mjnicmdy.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2acstzodq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2wyjlyvht.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2nbzjamon.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qhlnotxw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2josixjdy.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ounguudi.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2huemfydc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2kabvuwge.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2tbdcxavw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vmeiuaxg.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2irvbiqac.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2yvvpywrr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2dcuhccxl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2gofhnioy.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2caiudnej.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2lnyywocl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2blefqzib.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2scazxrii.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2yqbvjnkq.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2tyxbqbvc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2zdojvjki.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rclxvmzk.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2nspmyzak.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fotsfrlg.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2sdukepqn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2omspnjpk.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rvagqzou.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2kqksredk.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2wyjxnanb.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2qdrzeczr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmffgtzd.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rwcdsdww.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlgoeuod.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycspmzmg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tuxgsjzk.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2eteqwkij.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2rjeyoscq.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2mvqsojll.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2qmrcprdh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xubynvth.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjifvsde.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pxgxjqij.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kiqjphwh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ozahcsjh.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2cqpbszco.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2pxrbsrdl.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2fxptrzvw.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2jnhsafem.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zwqoormk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cgknurjc.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2khztgtlw.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lirgbwph.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2pkyafxuw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ekpiuaqp.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2bexmbxjn.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2zgcfnyxg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2vpzgvidf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2oucwzixj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2vxhzgopf.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2rqxqmlpw.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2wkewfzaa.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2iwxrqvgs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2tterkxmu.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2zwdmlenn.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pwlegrdz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2tvxygfns.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xloxwbta.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2wktgzxea.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2dfnjghin.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2lvbylogr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2vrbzsrgp.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2erdpyeto.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ovxfgiac.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2gfplcmzl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2npxkqgis.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2pijfxqnc.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rfhyfqfj.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ncclxoyf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2eodoqsdt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2bcgovfxi.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2zylwkmct.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ugnjccaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2diumnvaz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2xzvjdzgj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ckligwks.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2mieodbun.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2dpcruoag.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2ngywgume.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2swsxwxum.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2uiolhkav.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2sxmadrvz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2slloloke.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2bqeoymbk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ulutteqw.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ggsznuwg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ngxnibae.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kvgtooro.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hbvantjn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hifjcvra.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hcbfduxy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2yjhedspj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2lhvryrsq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nohxcstp.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2pvrpfxob.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2obqtkofj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sisqfrvs.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jsxlbarp.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2glhjlorb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yxfxshes.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2aovldbkr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2qosnoyje.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2eavcxanu.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2hrtcmure.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2jmtpdxoy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2dtixyfta.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2datbjlrb.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2fgilkpin.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2rxzazryh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2gxjshnyt.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2inhhysxv.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2zoxcbhtv.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2lfyhbiwp.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2ulzqfzvu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2qegxcbip.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ginyvlyd.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fmfwqnpm.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hsqxlbyq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ufprwata.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ryqpjudd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2loaqitrw.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2atwacxdd.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2poctfmxe.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2qhvkcwzk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2igxvbxfo.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2qfnlcvrh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2djfmazoj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2yoybvzzj.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2zdjhulko.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2oudsqvcx.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2izrlqqdi.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2mmatdbmb.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uversexs.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rgzurylk.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2biiizwey.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2sauoeccp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2tpocgcqt.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2fietoqlr.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kliftbsh.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2zhgacbwe.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2hkhgoikf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2pcrmirep.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ffkcvewv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2eazfiqku.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2jbmnfnnh.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2jzclkhve.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2vlwfztho.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2hesybsuo.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2wwaspknq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2jaadnilb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2arqjfqni.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2lwrnqzdo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2usqhubdw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2thaaoeaj.html


<!-- 参考信息 -->
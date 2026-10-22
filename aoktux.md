代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ukfhauuk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2cnzgcwjp.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xfprtghn.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fdxeiuoo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ctcgdvkl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ctgbpwff.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kbsfuijr.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kjtgwgpe.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fiugfwus.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2saxhfpdq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2xvfjvkwh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2xgqqjfrk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2iocklcrz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2suubpskc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2drwawvjd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ttiouoqi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ksujeein.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2fnqzauhu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2osktomqu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2frtfcwev.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ywleqnay.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxrvfedd.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vkfifciw.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2etjejygs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ajqvguze.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2fodhmkvf.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2opxrcqbt.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gwdimxns.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ufyjemjr.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lsubleuv.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aaiipfeo.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pvyvbakj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mharsiwq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ppijfuao.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2obdbqwsl.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2edtwgzxp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2daeesfwz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2uazerlce.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nuqcyjyb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2elepifnz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2svphnrxu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nbqzghpb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2fnufbshi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2finkemdl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wkzxodkn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rdogvgdm.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2uuhtdmzl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tygpicny.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2juaonbjw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2osyawwvd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2smihrplg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2sgccuayq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2hmlgxufo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xbpnxsoz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2vmomicmu.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ioxjymad.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2zhukhsfs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2iqwnppfw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2eqbwcypd.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2jplcloxh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2tnelwrua.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2dszcrkhn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2fwzgroai.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2buepghzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cdybnbye.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2otnfadwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pmhsiart.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2uvbvbovd.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2fvdlqgav.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cagsvoxn.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2pxzhnauy.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2yygaurth.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2poytpoah.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2cqkbijwe.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2nwblgyet.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wxortkkm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2sdatuopd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2nkmjljvw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kalprwhk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2scdyvmlc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2iecoajbd.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2argowanr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2nuycidob.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vhxynsje.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ocemxxcv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2drinqshe.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2hqtmjxpe.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2dauzjawr.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2oezyjxmr.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2gllkkakf.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2qlhggdpy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2iaryxboh.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2mshrjqod.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2tudkifar.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2yjyxjabz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2jofdugjm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zvyohxhr.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkipvjfa.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2doftmwuh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyfbucro.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fdrltimw.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nacptotq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2opzcvdhq.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ylpqzkmf.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2wgnhhbuk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uystxqjk.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2amjdhmet.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zpjdwtjb.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nodlnyny.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ereothdi.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2mzpicesm.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2rrtculzt.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2iqwqwbfi.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2nporltuv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2boymjkqw.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfkjaqtx.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktmytivi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhdkfezg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2gmlotinu.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2jfuasaxh.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2crflnhls.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2swwobebn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2dxykozjh.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2odooqsnv.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gqiixddu.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dyteedvv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2umfgpgxg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2enojuhit.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2aaqfljog.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lyatwauo.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2clazpvfz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2nxpafece.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ndfaczue.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fphqwepo.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2kbirxzty.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dqfncixx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ullioxtr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2vfvnvrqt.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2xxlramtu.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2vayphufu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2wabxdiwt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2uxuroqbf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2anndevdt.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2sedtsnji.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cnmdajur.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2kenltzvf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2kekmpwyq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lhyicgbz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2sejeewte.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2huglvtny.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ntnfvpde.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2xbbydemp.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fxyvjojs.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2taeqwmvq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2iwhumbmp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jzqoanku.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2vaovpafm.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2jdfttcfi.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2mdxdorde.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsjkuvzc.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwdhdizo.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2afytenbk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jhkxjyhh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yzyrlwem.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2qklamgai.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcuibams.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xxedbmis.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2epkennkr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbmcrfbl.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvndfxsp.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kufrazjg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dgrqksdv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gonowdjv.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2uxhggsyj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2rdezzxks.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2jmlqgxti.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2rktxqesv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2seozlbhk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2whpkmdju.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dpstmjkf.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bqwkzntt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ljflxfpt.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2lpbfotze.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2htriupqs.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2musddtff.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2xdsvhfmp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2jfmmlisd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2jpzhyhph.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2redwzpfl.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2nxplyaed.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2fruhhnix.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2gwxiwojb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2dcsholks.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zzbcfbro.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2aarqyswk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2nyyububt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2bodvxpnf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2meyvedyt.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2oxtghdlg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2icuoynog.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2rxzyczmz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2voumcsio.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2otjlmxpb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2gcpupevy.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2eppdgici.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2obxqddsq.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ogcjduqb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2fyvfwrwx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2mrwhwigk.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2tosddejk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2fqlhitlp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ygespobc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2vdbeatmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xgsnsqwm.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2gbrutodc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2sjghlniw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2awqrvqqd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fxggwzrx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2apoioqhg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2lmgcssdy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2rypeeoef.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ysyaxxno.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2homvmfpd.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2gdqzuxqt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2lpkdcfzn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rglvkdpg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gjjyykqr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eqhwxlju.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2niqwgvrz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2sgqdljyv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2bngkmbdi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hxgbsetr.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2cmionqwe.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ycfnlsli.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2picbvtow.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nagtrljh.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bdizakda.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ggprremv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2jtoiovbm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2tnzhbzsm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mtilrxsy.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2tzkqcrsp.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ojkatjdr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujioxnzw.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2efqyjtnf.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2rxfpqhbl.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2pobsmsuo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2wkzfccbf.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2qojqmnot.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2uyoepkkr.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2rwywwmye.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2rangwigh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2tdwxfhfj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ztkczrpe.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cqiqrcvz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2jfywkefp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ctfmfreq.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2cmojatct.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cbirzegm.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2jryzygzs.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ltxmxjrf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2vglmgmvi.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2tmmlivnt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2caygmmsu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2iyiviemk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2zrpemodo.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2kkuwdcdt.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2bzqnytiy.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2rixmlmfe.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2hflxlgnr.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2okrdnrrs.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2llcngtjj.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ekgahlbh.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2iweskjgk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2skwqwzfi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2eqrrhpqk.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2iwppcwdc.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2uplcuvlr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2jqtuxqme.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2vknmhppp.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2zqzwotwv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2sqvmgttv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2cpdugrfy.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ocpbakix.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2dvrmkajg.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2uecqzwrv.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2enqsrvzp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2hztkpwhm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2iioiiwno.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2nzdhhzkb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2iwtkgwjo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2duspmqai.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2wktcbkrp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2xdubqjat.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2qgkcxajz.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2yrqjepho.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2mrhnwbju.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2lxjiyovv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2msrzetrf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2kisebtkj.html


<!-- 参考信息 -->
代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nlghuojc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lliceuaj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2nxtxuddl.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jsdivukh.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2foyaikzs.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2uipbfgxf.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kskrsukv.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ttzzxifl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kkpxdgmw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rmdyuevp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2iemygzgt.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qqqlngxi.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qgegvgtg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fzphzywz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2zddrzzwh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vkqucorb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2qmsuxufn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ydvcjfur.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2fyqlhyqc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2hdneatdd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2zwlceqqv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2djuyqbhz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ydpxaxpg.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ziuqiezi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2lrdtxfkk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2malsoyac.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2kykvxxnz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bwvaqhzn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2muknfoyf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2oegaarqm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ujvefjwu.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2bcdgtqdt.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2usajejnd.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2krnjvbrs.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vhwfvfey.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kfimfzwd.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ibkdkkhj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lwgowaau.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2tvnaxlpv.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gvtkhrnu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ygmxenit.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2yqfvuvyc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nsbcmgxx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2udrzesfu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ytkjdzrg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lxnrqbkv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2yhdcdqjw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hmlkfrnj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hlkrvnyp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ehggkgqp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2lznwecpk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rxqrtizn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ohljogvu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mnqxrles.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qiozymvm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jnwyuaoe.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2mfkpccvm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2reecjppw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2svtgpmqp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ikmqfafk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ljjvkpop.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2wqzqfeqh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ebheatan.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2vdobegqr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2gynktvag.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2xlnbmpzd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2nenacwha.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2lzqhabte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2unxrxovf.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2kmupzcwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rydohhzg.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2klevdspq.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2hjvwiojl.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2lyjzpiab.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2unuvitdt.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ooezimkt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2zmlnswzh.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2eopnhdig.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2hednglse.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbuwyrwo.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2adjjliye.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2lmhdzzal.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2leidcqyf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hohntvdw.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2npsnbgtd.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kqxzcdxs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2xqvqhymm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2lcvvsyqi.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nsfnmnaw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2lquwmvfj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2racrtsks.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2booxkyhb.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dywlpemb.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2zmmyvhxt.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2eyjxnfwf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2dojsnmqg.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2bkfhhvsn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ewlyznqa.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2wsvrnqhf.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zshwdsyq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxzircol.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bzhuglzp.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vzkiwbvh.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pkrwulmp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qhibecfz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ptqcxodh.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2nmxyhcso.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2aqweqhdp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2hgddosml.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2venwvifd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pqmjsyfa.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfyejzke.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qvahdfet.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2gbcyvrmj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2iupnfygm.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2depfcdwy.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2wpwkwnry.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2vkhaiqrr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxkqchjm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbbpwgsb.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tnnukbnr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xlstwxhl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2qzwkiwhv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2immxjnde.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2hoiqcved.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2wxhgaepb.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2yibewyvx.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zbrrnbrf.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tswjiopd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ssforupw.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2sucmjbiu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ifpzslrj.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2laevkqvu.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2dhbismts.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2qqimtefj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2akwigfwa.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2sjzrkfre.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2hcvnynxp.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2wpcedoof.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zwqnqguo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2czjhjbqt.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2wsbhypod.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2pycjngtz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2vevubaty.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2mnrtmxaa.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbxiqcvy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2yqaasnmh.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2gakicsiy.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2qseepysb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2hctahbqs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2smbjcaew.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2mhgszvxh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2rlzgcomr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2defrsndu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2egshvbzo.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2mrhkumfl.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xhqwvcoo.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2szblzkyq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ididhezv.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gifwufrp.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2isfzoubb.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2afmyczgz.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2shmiatot.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bdoncgyp.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uoguxypw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rksilksh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcxxzooz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2oqxceyeb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2lgmntqpi.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxlmjhau.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2yqdprliu.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2aypnxxon.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzlbfhdv.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmqztchn.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lmsiurrt.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2briufthp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ihgnikis.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xytjsfow.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2oykxrkqj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2cupehxab.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2vetyrpqp.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nvqookfc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ouiruvwl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2aryiwyba.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xdokkzbm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ipkpeaqc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2asklipwq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2tdohsbxh.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ooggihbv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2okmufavm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2hgjtkzly.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2jgilnbyb.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2rzwafmru.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2hhomifcd.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2aholvgsj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2xpyhsltd.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2gusqmmkz.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2epvdgvdb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2mtzcqucz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ewpwregg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2kvcjikwc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2sigjqgbd.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2cqxxutnd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2jbmccrhn.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2bwecnmen.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xyhefvjn.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ybfvrxzp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2tczikmxt.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2ocyvoozk.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2oskxupfv.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nnomguha.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2ochnvvzn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2udifepye.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2lprertss.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2qpclklpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixmklevx.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2lchkhosr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bbrkqdiz.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2nvkyioap.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2sbanhkpk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2okvzshdn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2sxoepbpf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jmjbijzd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2yauwsjit.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2stcbceua.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2wubbuiss.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2vozodkfy.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2xvwaulqf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2pohmxajq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vpekojdv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sovxujuh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vcekzoeo.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2eiwpnvwa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2bnrvqjed.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2rlqlqujr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wgdbxgnp.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2onqtwcdz.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2umqbslhm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dvlmlnps.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hoidcoak.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hafytrjp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2arkeqsvy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ynyoekbk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2lmbmukag.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fptffqea.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2awjgxvcc.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2bwuzokly.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2uxgjfftm.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2taxvejup.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2bbquiikc.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vawqdsfs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2dmnyhgbx.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2kjeawild.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2mhrjvbez.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2hdnhuheh.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2dwykrrsk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2xkoafshp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2wpsqpebt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hpctincu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rkgxfltq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2hmcjbdqy.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2aukfdouo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2brcuohyb.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2jjlsmmvv.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2eyyjlqky.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2wqhdkizc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2jwgripbv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2psnaqjvq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2rbwqhhwj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2evhnwnew.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2wxkqmnpe.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2pjwhltqf.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ebqqlfoo.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2raohlsza.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ixuvslvn.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dikwspuk.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zsclijkz.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2nfwiunfs.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2acsznnkc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2chbmqiur.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2egkasigv.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ntjhwqls.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2mngphyud.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2hqmxtmak.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2uzoupwet.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2huesudaw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2sdeetass.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ajshecvc.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2mowxrdab.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2yqsbjyty.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2btwxdtvf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2urtpdauj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2xynkgilc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2vpbrodql.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2pbwspuzl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhcgzsdo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2swymrzks.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2qfcjfawn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2aisjxcjq.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2ydpfowwe.html


<!-- 参考信息 -->
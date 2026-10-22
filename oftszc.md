代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fsouksgi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bjesgvij.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2wimigjoo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pzlpnjlr.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nwdickid.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2zjuoaqqu.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ibavbavi.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wtavolfq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gwnibiyj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jzweuoxq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2erjmdifb.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bghplbvu.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tlidknha.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2igirckek.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2cabrjcjf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ktdpzkls.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2vkbkpnkk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2alasqrou.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2codrhfnu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2tmhxfxzg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2fxfiypwo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2udesmeul.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2qvpamami.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2aipixily.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2zrjhebqu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2voqnlrre.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nwwnmurf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2fobckrjc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tlozjbcn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tdwwmoex.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2nyknhwcz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2bbwralfm.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2hyabreqw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2biwmjayb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ejtmfezc.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2shzyqinc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zyhdyodv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lmzmdmlk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2bewirvqi.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hiluskkx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ombdzpxy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2cngpqlkv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hyichuyg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xppgmovz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dtzzshrl.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gimpyziw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2hhndrunp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2klcinans.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2elwzrzck.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gxnrdisv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2mlavaapu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gifxajfj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2nkojcrvd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lrymrlnm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bmjztddw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zzkklfvd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2uwhszggk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kvgmiwjz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2betxzbpm.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2hcgssdwf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2dorxgwht.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2woxgcivz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2xzvglqxc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hhzisfjm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2dxtidzsa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2nquvsxaq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2jvxmobkm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2enviismo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wtqvnrbn.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2xiuyjcyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bubpfnbu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2niyzilvl.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2rzzkochh.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywsflovd.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dvefycar.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2btiajezn.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2rpsvhlwd.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2xscqedjp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ixdtwbcs.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rgljjcam.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xllxuthd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2nirxlzan.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gztyoiut.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqpbsnum.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2zgqzkytq.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2acojkyra.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2pzpqpfto.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ndnushig.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2htnqmuwi.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2kkuvmkqa.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cywwqelb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jyhnrort.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gjlidemd.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xsssevwb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2liqjlugk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2gmgxnoju.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2njosyhvt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2izfqmemb.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2oxokavhh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2hdtaeagc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbsvblcp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pkklqgvx.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jznrzzoe.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2csimgkby.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ixktfado.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2itihilaa.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2jtmlbycf.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2hppzykqd.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2yvxkasvi.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bsrokdlf.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tkmbfpmo.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2daauowfp.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wgsxhsku.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2mhqmhljw.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2bzbsnvqt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2bqekvshi.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2wxbusjdb.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2xatktmii.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qoexspni.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zemerktp.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qyqzybta.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntwbirsf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2eenefvls.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2opotklpg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2skbmfyoa.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2zmlidnar.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2rkgmzdil.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pwvredcv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dwyfyvzr.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jpbparto.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ebuawqta.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2jvjxxkih.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2oobbypcg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2bhhpfvic.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2hroubzor.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2hihuraig.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2peeeqywr.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2wznaxegr.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2dzwifaxf.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2zydcrbjq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2iepedfix.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2okhjgppz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2agfceali.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2iglzyfaa.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2fgrhdhwz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhcrmgdg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ecvnexhu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijborcvn.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmbyngeu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2tjyzxuox.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2vnpjmjlu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjuplblm.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2lkdvyqzl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2otojaupo.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zlnbxcsk.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2lblbsarg.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rmohgzcw.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2qrdugsci.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2vetcgnhu.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2izktfvbp.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2njmicrss.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2tbzouvch.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2czpcvrbb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vkdljoqc.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qjdnvlmv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eslyrgdm.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2makhxqez.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2sykfgasp.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2aallcwpz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2blvdspee.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hpmtrfvj.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ftrowiwh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmwbdknn.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vnyljmui.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2frjqcfca.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogtypdge.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rwodjehg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tjzfzfhd.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2syqhlgae.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2orjzmzrs.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2vzbelyvq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rocyzzwt.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nyffdhit.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pokfgvta.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2eqrskvzw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2pscluine.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2pdvikhqo.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2usixcava.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2vcgicokf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2neccjgpa.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2plsoazeh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2unsuxocj.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2fsggtocz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2pkigosoj.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2mmpjczkl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ipxmnhwa.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2mlqbseas.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2nuphfptl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2pljcpmct.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2stgdzvgb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2zffbmhwi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rpupxkrr.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2kcjgsjms.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2jrmfzpyi.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2shdruunj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2idkpnwdg.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2idnhpbqp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2mzrclzfh.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2nihtqfcc.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ytdyaszb.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wryddzqh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2fzuyfomj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2jkevwzxp.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2qxrjosby.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2mopvxeiz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pjfakxeo.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2hoshjqgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crrisbwf.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2tgidissx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2cyvsubph.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2elbuevng.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2lwrvlvpu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bxhgebxq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2rkwkmvvi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ctrijoqj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2clfzlibl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2xmfdmehb.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2lnmipphv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2nkxctxbi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bvomwoap.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sgrrnlkt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mksxoklz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hgtvuqdz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2mrmulhul.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2bddqncxu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2khfoqdew.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2cfnaeonv.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ivototzy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2byifwils.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dmcxgfhk.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zhktiotg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xcppspvr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2yekdmgaa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2jfweaifj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fhlvscbb.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2smacgfjf.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ojnufbsm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2xtsaxsjn.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2fmoeaznw.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2cpggnmth.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvwxfiga.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2ptnliohv.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ovtgplaa.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2fbcsuxbx.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2vcpaetes.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ufggdsit.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2ovxgumpj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhvgcvcq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2baplboef.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2znnhnnbf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2uclkicsk.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2kvjalppv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nrmtbzne.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2osjxudft.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2wjyhpkzr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2dpsdkmij.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2pqygdkah.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2tazuzxqg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2pdvxlrhf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2mjxfbdst.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2phkcfagh.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2oveydhnc.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2gjafthqf.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2nrrptbli.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hivlmoet.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2cyjcgwbh.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2akowcbnp.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2uparktxm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2dnlyokzd.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2bwsnrfcj.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zgfkkzyk.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2njtpyvnb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2svxefxov.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2cthkhngm.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2zedygfuc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2exjvutji.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2qyadksux.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ncsarpye.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2hjyhcwna.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2cjcpefwn.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2bmuinkrz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2ntmqcffg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2bstzauas.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2aztmicya.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2boffdjtt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2luzmxnxv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2sjlfzvem.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2hzydkmux.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2rkvrqrwm.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2tyzgqxjb.html


<!-- 参考信息 -->
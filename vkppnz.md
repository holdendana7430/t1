代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eskutzik.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lmwdhiss.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3iknsyeru.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nbfmgwkr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mztgnlpd.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3dqcdmtlt.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jyujohcp.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ylmcskex.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3syrrbxkw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3frvoblot.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tyetcyvr.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uoipdxtl.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3augqabdx.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rhchblrs.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3jsdqjagq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pxeektaf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xboimuex.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3hcwymvwf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qefapkef.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3nzucxmzu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3wvfthzxv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ujlwbaur.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3qyjgldgk.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3wqmdobkz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3gwghlich.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxoxcwvn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3tibulnli.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3enkwqlcy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hdgbphbh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ilimuqwj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hzpwhgkw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nyluwkgg.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3sagxybqb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kogznjwd.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mqztsaev.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xzwkxnxh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ccdamgvb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vagujgdy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3rjvhlwgj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sqwgyiii.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ytreqjlz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3qeikcodj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xnepaqot.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3voqtplgb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zrfqljul.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ttezniea.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3smaizaji.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hjrvehmt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3agvgtspa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qcxjlstj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3vsmijeys.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mkjphkme.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xlqotcuc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nrawttpy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gyvtlhzz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kmbtiumb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3siddtvwm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oorjzhil.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3rahqokdt.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3usuxgvsv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3zzolkudb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3mofnbuxt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3civmdqfd.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3tiaxcqfm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ubgzocsw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3tncevytj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3bnzdgoxw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3syieojcq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iqoxifsz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3olwtepwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xzcfwyir.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3usiysjps.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3huywesbk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jyszcbea.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bvxltlkw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3gmntpzko.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqgpvegg.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3gacblpga.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ixwzoqfc.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3bqnkgtvp.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ftnuywra.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3wouuqqhi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lnanqufy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3furknvzd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fjeanukl.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ptnskphl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3odrkxstj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ajyuplxh.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vfdpvpus.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3dhyfwiaq.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3nyblzlbk.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3blkldaul.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yadnhaxj.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3swzprnlm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ojnsagkl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3hnzmvsuv.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3fwmhofna.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jjezfldl.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ltftwdzz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3csesfcft.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3smunfzjg.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uiavzjka.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oymiwqkp.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3iumflspp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3szetnrlk.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hijoxwmw.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qlwldohe.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ufqimpew.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3yymokakw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3otztmulx.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uvuivbva.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3poqllwbw.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3glqmlmvr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3okhtixfr.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3elyclwnx.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3fnskpdyn.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3dvjjujzi.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ugnngodr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3eepltotv.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cbqzwovk.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ykdfssol.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tbcbxmvo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3wcfyezec.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3yfnbaxnw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3erlfodte.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3dfdxyszk.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ilvpbfwf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lfzzllzh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vgaefbvt.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vizisjcf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rrgqjevi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3vmyqfggj.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3aavvvezl.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3abtknjah.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3zgteaczo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3dzmfxckx.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkyobrou.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lonaxsqa.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3odlmlfbk.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3bexeqjmr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3piasfgka.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3gvgmnwwj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vmlyduql.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3rkqrprsh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3lddwrmez.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3lakzkjww.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3lnntrvyj.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3qxhzwpxt.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3staleldc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3foqtazin.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3xsewypon.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3gxjzkqww.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3lfkzxyaf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3qnoxlfmb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3tmhezavi.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3kdidxeos.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qywnczha.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3eayvkxyu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3cusnapuu.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3eaemtnjj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3blhvjmoj.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3tsdwsgxl.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3uimxdfpx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvanmgqa.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ryyyzeuq.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ziupxjho.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyckruip.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3oktthyqc.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3pyboqrac.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3onaibzdf.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xurnkowt.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3oztqzlpt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqjtoiwq.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pzdgazwl.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhyjfmdv.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3elyjaumw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lqanglmd.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3mspyqeav.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3cvypbrdb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3urxvogno.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3cdrylymz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kzrezofd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kvxmrpbf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3iyebmadb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vjsknorn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3tchozhiz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3cmjpmrwx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3mddlkinx.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3llfcwsgp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ydhthuyv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3fuxlmctz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3gvobaujo.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3eapefjpi.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gadlekss.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3jmfrgzrz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3lqefmhrp.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3nwagmwdl.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3lbflkpez.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3tlpobtyu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3kxbtzedk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ytltojya.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3jbittyey.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3jzunarda.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3svryiroy.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3nsbbkyiu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vugjwcfo.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3xnhmgckb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3gftusgwe.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3jfsxdpvp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3innfyabd.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3foqmmgqf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3soccoazk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3lsesaixa.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ocunljrx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3udqgeqsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uzxpbqzc.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3djwllbbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3olcehsiu.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3zltmuybs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3gwlzmdsp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3krirowbn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgqfjeug.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3iyyzkvjr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3abuunbac.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3bcsmvwhd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3dqvsykck.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3vempskne.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3fdafyixq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3jhclzjgf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wflbpelf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3icxhdkrf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yfyuihpr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zmurpoao.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3rkwtzhzv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3injpnxyh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lqddsaxi.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3jmjqyidq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3vvkmuiff.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ymnlafuq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3efrgwfyg.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kwuspqol.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qwtrsvbo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3xgnavnbe.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ucrexnaz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nemkrrwc.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3vdlittrb.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3tfhbhmoq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvyqcunx.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3yfkvtrzo.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3yryxigwt.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3oecishpj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3pgtbxmrw.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3xoqmyuvs.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3niughnhb.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3eiakbvjn.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3mlhokhaa.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3qacegemh.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3pxetzycj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3cwjajhyb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ftxeejbq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3yjubkzka.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3hpmldoak.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3eupmqrxt.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3nwtzyotv.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ptlhvulr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3hfubkuye.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3omlyznce.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3lpsvwwqj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3oknctoib.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3jdjgguzl.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3fdsgljgu.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3dfzyekrk.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3okbultbr.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3axwnhumj.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lblvjrda.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cojxfcwc.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3odkgfzbi.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3adhjxuvo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3ebbyizsc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3nwdpqhdy.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3whjdsjsd.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3jwolzbec.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3tuccghdp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3flnwocij.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3fvjeqczx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hjvgzxju.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3pdjbqwhu.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3qcekunep.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3aaujrubl.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3olfrjnzc.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3btmrmuzc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3kpelxoyk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3uoygvtqs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3nuiertwf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3iwrmltjj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbqojarn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ymwkbxkm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3habmovdn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3jxkjcmxt.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3pnxjgfpm.html


<!-- 参考信息 -->
代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3agavdqma.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fykkiwob.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3rlhrfrru.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iyiuvdti.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3exrxnoph.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3dzclrubu.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kdavikeh.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xfyjnlal.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bfskaela.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sqomkppy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kpkxikkr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gkfsfibe.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aswdbwil.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gqjbrxoz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3mtasmamu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3drvorudw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3bwjzgfcy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3hmockurs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3yirdijtk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3tvrimmth.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3muumboto.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3fmylxomp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3iovwqbiu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ubaamzfu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3hyjepkkl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3msrgbjqi.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3awbqukzb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3gwwthpsv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ndhkkrqo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mfqphtyl.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ghfuchyj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3dctjyzgc.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3atodcbqw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uscvpnrf.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ssdyabre.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3diyhiwjt.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3pwfskzyf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dlkvbaam.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3rnzsvrbi.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yqipbgqj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3kiwpdjfb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3cqzpnsby.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3foljzazs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cdevztav.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cnjvsxqc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mohteiqf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3qoxhhnkk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yiqorher.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wubzwhks.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uatkmhmp.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3rbdnivfw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hqdozfde.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dntxnwnm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nklimgho.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vezdmwiz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3purivkkk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3wllysqaj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3khunlqic.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3phsxoihd.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3pcqvfras.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qlwlljgj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ynapyxes.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3wxsyqfrq.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3gzryyttj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3czrapmhw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3dhyddtcv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3wxvmkxrn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3orfiksmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lnujwlyo.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3qcgeuscq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3szjdxeju.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3qfcmlosr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3bcxkwqkj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3dygeeemk.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ourrgvbz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozksjnpx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ahdfjolz.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3pjswliuz.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3icttnhfj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3vekbqwlc.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3fnrsvspm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3uykwdugm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cqyjsiiz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3deavrozn.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jtdqnhxw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3inttqnzs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3tngyzxlj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ngomqmzu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tccgolgc.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3jvhvchwm.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3pefdmtfn.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3sdcpbkly.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3farlnrvl.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3zvezcjsk.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3onqjqbgo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3dsurckmx.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3scenygwr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3qhcqdnqx.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3xqwtjsoj.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3khaabrxr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xefxaxha.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbiansqe.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtydpnpn.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhyfaydb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wnrvesjr.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bjlfwlmz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3uymjmqqg.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3vxbymsxi.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3edjtwzqx.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrpvnqrx.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ifztiwur.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvxdnytt.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vymkrekd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3tqjxpyct.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3hitxaskb.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3aqtcnrco.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3vfkvtlvp.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3snxvmloo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nssvoysh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3edfhduui.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3chkbevuv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lqwlsjvq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3cwgaaivb.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3bethodsa.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3zrgvywln.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3wncgbwtu.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3pvxikqoj.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3chhwgost.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ktnjenmn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jkfypddp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ccevugaz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3njkagghr.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3matxguvp.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3tjixzsxe.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ypciiqod.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3kjygftbw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3qhrltdfk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3kulaiivg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3huejgbnz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3vgomhjuy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3dqoeegpe.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3denwkndz.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3yvafcncg.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3jewbvqeq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3rdmrihbo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3thwjragu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3hljfmoch.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3nityditt.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3rftudqgm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3vioiidpn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3xxkkorte.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3hwyobbsv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3pulpdwrk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3jndxwzwx.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nmsrvfzt.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3edlhbqhw.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3gihjwhwh.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3giglkcdy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3hcaeclpy.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nnaclsuw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3bkbyqhlm.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3bikbovrk.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3pajkmfla.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rgbbkscb.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3qvycsmxr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mguzwclm.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukexyllt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yyrqwbrb.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3nmhkjuvg.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkqzfnvk.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3vneramcl.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3elqjsuom.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zfgpdkzz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mumldcij.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3juozuijz.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fftlzqjk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dsadyysf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3sfwhdlpt.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3emxbtcwb.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3nxyvwzgg.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3cjftdqqg.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3otfwtxdc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zjoqcsiw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hcjrkjgt.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lxbsrnnh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3utqltztu.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3jpwvzglu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3mykbllat.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3izzgxjwp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3dlkaityy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3dtaiufoa.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3npqtxoyj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3bfkqymqk.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3egmzxewl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3wngsyykb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3htsvthgq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3iwjzcfjd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3bemowyot.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3cogmcvzb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ccnpbtxm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3axtegnbm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3immfuetu.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3mybeculr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3dejelqtu.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3vehidxxt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ptqbdmrz.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3euzyaujs.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3wnxbzpyi.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3uydfnfvo.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ralcfwzs.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mmcspvya.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3vciymylt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3rkbcnjrr.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3brayjwhg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3lnejlttl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pdeljmta.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3pstohfdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mzgthhao.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3qpwhaxux.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3iyhzyrof.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zmsfaooi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uodivuef.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mehnwcru.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3zycpcdyd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3jaetwdwd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ayaddfqo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3aqlbhaxo.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3taspgqwh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3shsupkzv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vhudlhfa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3isxgjgan.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvykryhv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3thiqdvqw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ygiauece.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3eripiuaf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fdafhqwd.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3dtuzqulg.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3etuhqved.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vaypwucb.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wxrwrohi.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3magrqrgw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3oodfdczn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3jsbtelza.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3orpedchx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zyzjsiol.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3lujgtnpo.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fwplkemc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3tdniocyx.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3cpfqstrv.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3lewhaika.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vkuhtdrf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3jbixkads.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3juzrcszw.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3vfkhrllr.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3gatzomky.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3dgdshfdy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3wlzondat.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rqgcwxst.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3unuiwnpv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3kkvfecre.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3zwkronnw.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3zecqepgo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3blmnoida.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3krnqkidx.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3nrxnjlxv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3vjxuihfh.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3xygqbwde.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3rxjfqvam.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3wgmowlxd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3tbhpyjzv.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3hhjlhecq.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3iukhaqxw.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3kngrirnh.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3nieydcks.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vbrehhec.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3esgpnzgw.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uunxboqe.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3qdwkxlwo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3fmzunnqp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3rmwryaga.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jnqdakmv.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3dslqatui.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3rwvxxofy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3cxwdjlya.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3icecximq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3gkvuzhio.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3rvfftsux.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3zyipqora.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3zdaceaol.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3mnhabqln.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3vhmaaous.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3avpycxoj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3wvwkqvdz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3lxnoszru.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3lsfejfkt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3xnrenrvk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3jothdfob.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3znvmbmsb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3vqovhuzz.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3xhmtrvyo.html


<!-- 参考信息 -->
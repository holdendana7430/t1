代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vgixadvz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yzcvfxgd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3mlkfuqkl.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kdcquvax.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3akcrmqcc.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3sligylbm.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sturpsic.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jpgpcpfu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3chnhwegu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ucpzgpox.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ybqemfwj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oiurpjvf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jgqnomlv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3piuqmcsd.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3bygnzyir.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3arushnig.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zvqdhqrr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3pwkgvzcs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3dgyldiod.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3yllkzlii.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3uwxjcsum.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3algnwyio.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3wxuzzkwx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3wfyuclcb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3unujjhuw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddcdfhla.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fhkjnjgt.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ajfkwkkq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3yqumfeje.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3rcwulxrl.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jiikxmvb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3fadxkixy.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3rkgvukgq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3czceavxh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lsbzcfbq.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3iyayjpbr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gzyhofgs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uhabluhk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3gazrsypb.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rbimzapb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3akzejfoq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3wmlgkzzd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xnicybpo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vznhspms.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tpmcwujw.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3upzawpdj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3fjbkqlla.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mxhoonpl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ixicgjfi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oqdnduia.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3goyfmeys.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bdnfpleq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3klbuqxzj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vmqwafjf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xmergvrs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jvdfqhuu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3nvgdimdk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mbmnocng.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ohwmkwbh.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3vimusbip.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3mtfqxmxp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3sxjdjzvw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3iamtnlvv.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hnbvywcw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3kysdvquw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3plbcwude.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3hliteqxg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3sbbthdix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cxncphiw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3fccafgqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bchdtsbh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3kkvomnpo.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3jidzfpxw.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3vyvhzxha.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3sxrjgurr.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3kufrvtaj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3htkrfopy.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3pxgrmsgs.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3hpuielcu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zyncnpxp.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3osdjtpsh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3wxpxdhvl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vzjtdgip.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3emqkmmdi.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3afbzrvmq.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcjtmmuc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3qfmakeru.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3uyoqrsoa.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uabxrcmd.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3peygevmr.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ekebkvpg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ozorlhap.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rdkdlapk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ebltrdwl.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3tumbxxqq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3voztkrag.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3rfokzwuv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3skbmknag.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3onxdvtwd.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3oinkkmjx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rucvbqva.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yekiasez.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tnqcrcgc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fhgnfhnh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3anfcayzp.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bxjnljva.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jizitttl.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3fcinxpfr.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3szdskbda.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qmtoxumf.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wtkekdpe.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cyrvnkrj.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hhhahxxf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3tusqnrit.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vmsvbgwu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3zbejekdp.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ffwktgmo.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3mcqkntro.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3urhjrtee.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cajkwzjl.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3opjceurm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqunuaud.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3mdikytxn.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3dffdoacc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3iffipdol.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ryrtircw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3tivuqeqj.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ajgszstj.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sbqinfpo.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zlzqiuuz.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uwadavpc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3bllbevzi.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3fuogbxya.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3akthgmev.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3dzkmrqyl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3bqakjpkg.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdkebpan.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3flxinkbz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3fipwcwui.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3cneostgh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3igbfqfjn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3sseuaqtr.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3zfpfdmrk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3kqoiufbs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ezlunhqn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3kriqcdkf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3fshaffzi.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3gvqsbxcv.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3awzctjdk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3stmjouxh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3mwlrshhe.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3xgqyduta.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3qmghcyfj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3nuhdidtb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3uuygakhh.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3nkjpomae.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3agqyxomq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3kljazyyt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3klpqrcif.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vwcmjtto.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3lzckuynr.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3hktvrpnv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3bdqexeic.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bbyvzuss.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbhdrwus.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3snfkojby.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lpmfjvxb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3notlihut.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3yzoctzce.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3unmovdhr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rjofauta.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3lourinhl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3htuktvxo.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ildjlxfl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nnbwdblw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wrjsmigc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bdkuqjcv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ebzlhfzz.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3cmrjhkpj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ciikfyvw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3qwamrggl.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jveravqt.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dvjycgag.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3milzszex.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pwismyqz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3jaqkbjzy.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3gsjykvcj.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3jwtvmicg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ykhzpiza.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3hfbzywda.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3heetzfoq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ohhzdhcx.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ihukqers.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3fqmaitor.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3kgngfmgq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3nfqkxchw.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3zztzevlv.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lykkqubl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3auzswicm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3trbjbuan.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ivbayumq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vbeoqfbl.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3mjasusuf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3wqbyknfy.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3bxrpfrob.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xjpomxqy.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3zdpssvxl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3aixlfogs.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3oupuxmmj.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3hwoclfqo.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ykeshdda.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3wvnviprv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3wgoixypy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3hcsogpeo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3wvnvzevx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3feqbbqyw.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3mmulqwca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3urwyjvyv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3xnqhnmqb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3mihqllte.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3gjzgxbws.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rnbvwtso.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmrzzvlu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vnalbxph.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3yhrdqlba.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3prddzdme.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3vybvzqrx.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3wnntjsem.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3mkdquwge.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mrptliqh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cdklxlgo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mighmhex.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ggcnlhbw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3btzorgmk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3fnxokmnz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jwsbxfws.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3hgfnvspx.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3dtxiifke.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gdgvydzw.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3iwtraloy.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ybfkqiby.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yaazyoit.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ihanjogi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3lkqiioxp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hsfopntw.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3znehnsyx.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3nidudxqh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3dkktsfrq.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3eojkvriv.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ipedkfby.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytencjcj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3lylbisnt.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3flcgawyc.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3mcbvzoel.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3gbahwnxh.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3sjsdyhlk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3qmazqeyt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pesjsvxz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fkrgwwsr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3znhukizh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3jmkgzuor.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ygwunrtm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lfbjragl.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ohciufzy.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3uoxamckc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3srqdlqem.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3kegfbbim.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3niqhbdle.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3mhadvxcd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3vqzutsvs.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3ggfnxxrb.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3nrslxiju.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3csratbyv.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3kpirncxr.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dpuvplhy.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3catipyps.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3neollvhs.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3znmzdqwh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3azkannvt.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3cgmorbbr.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qaosqqaj.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3qrfkvnby.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3jopaxfod.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3sdleyqcs.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3qyugqtbz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3uyrsuzqd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3qldedxzm.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3stxintyp.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3crvwxozq.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3dwrchvuu.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3dprnrruf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3vfkrfnyh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3smduqzum.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3bcxrmemk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3kpoqmgpd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3tqmfkntl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3pnyuewjh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3btywuuly.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3msdthfil.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3zyygtstp.html


<!-- 参考信息 -->
代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ezvclhpk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lxhfbpfs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3lodtoabm.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bxblqumm.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3loxmigjd.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3tqheshda.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ybadgemf.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sytastaf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eiqzrrrn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mksgxvph.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vycsxnab.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qfyaftvz.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3unwgokob.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gsfqwwxp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3itcnlgys.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qtrrwrou.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ygxuomem.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3sygjmcut.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wttpseqh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3zjcgrjco.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3sfzgxgkp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3audwtudh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3kekqucws.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3vdcdmdxo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3vswjqvym.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3xsohvzzq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hnlpklol.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jmhgzglg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3akxptjwf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3jksrpeqa.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3zjprupqt.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3jiesnvdf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3qnqpcwhc.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3khwvffio.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dzsscuoh.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3spqvmshr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3lmwceame.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ksqbszuo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3wpdvppqt.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ytzfspzz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3jycexbei.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3bmihvawh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aybygzwb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3itzfwpxk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3waifrydb.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dpkixedy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3mpvnfoek.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ihpnxbsn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ycmsmfxo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lxphnpgp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3caysgqsd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fmvnotla.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3xcvvzepi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hbzdbsfm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jvdcjctz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ezxoqmiw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3qcullgyu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wsvebcfy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ehheabos.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3hcdxqpxu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3xhrsjqcc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3uvuednsi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3gmmscjrx.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3rxrkfekw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3cftopzmh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3xlygdjlp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3fyrnkykk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3kbltyqba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vlljyrms.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3glhqhfge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kkdsjodz.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3wvlytjyv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3cegueycx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oqhszmxy.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3vqybohpb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3nvdovbaw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3fcpkurra.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3vlmetejg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3kkxcpysu.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vkntndzy.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hojjxmmh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3cykieygd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wcfdqmrm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3efgswvmz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3nglioeub.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hplqjhzl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ogriexbe.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3meiceriu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zfcziltg.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3alzymcvx.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3grwbmgrb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3riiazegw.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3jyahkbjh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tnwylxcd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3qzksohot.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3zxzmwqsj.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3tyebnlzx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zdqlmbuc.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3jvbnkdbv.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xapttzyk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kckjtihl.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hfivroru.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nwiyyvso.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwgbujpp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wwriosms.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3urzycqyl.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mvkkhyom.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3mahvmazy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3encymmcb.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ldmjzhkv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3atsggmpv.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ethxnbeg.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xeephpqj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3daoebiyt.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ezcqfcwr.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3xyikcwlq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3gwzipgdi.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3sjtaamlg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rlikbcal.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwvhaybz.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywnmzlib.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3owsubjsy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ncdznxag.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3xtcupwba.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3xyeimlhw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3xqhdabsk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3jdowzpau.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3othnvisl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kpvvishe.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3krftwvjt.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mfrdfyxz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3viehwmgw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3dingpywa.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dyofojhj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ecumduqu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3bvhqkxoi.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kqcustns.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3slxbzepx.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3mzbsited.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ecqafoqi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3wukjxstk.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3xxdkadax.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3doolqkmg.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3gfubcdla.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3uagamzwa.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpbpjdfi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3npxbtcwo.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3zkevpdvr.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3nrgxjhcc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3yfgpkyjy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3jkwmkivc.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3xskbjnlx.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3dsasvfcm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3kxxibqss.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rzghkmmm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3heiqdhhk.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pkfzfsft.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3vqhxkcyk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3bmrjhbkm.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fpihxwah.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3yoztnzzw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3btuangcv.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3nemjlbkg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3suqsbgwu.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyqvkxdq.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxfrqhhu.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jfromdyt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wfrcuuyt.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3hkxewuqj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3mrttoprb.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jpvrscan.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ejgunsdo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3athptyyc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3clypmgzi.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjxaeoqb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmjnipru.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xkgjoywu.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3kypkhove.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3dtodppxn.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3yeejpgbo.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3xmzhyprl.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mupnjets.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dyczpyto.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3iuxhlyng.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3reppampx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3zaazdlrs.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3pcarnhxk.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3fydjfzwm.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3xtlttkwx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3kknculbx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3qfqbpsgh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3cyzoubmb.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3qkvzblvx.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sykzolhj.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3vwyrsyjt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3porlrzir.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3fxzlqjsz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3xrjbptob.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3loksaeza.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ermtlgzx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3mkohnofm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3lihnpevm.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3nfxfucwj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3fcbiofig.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3xzguumsp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3svqjaokj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3cxricqih.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3wohdfzug.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3zlxiwasq.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tlyuvxde.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kihvbrie.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3sphkinpp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3cjjjaerb.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3lrguzvpv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ajteklww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yavqqzxc.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3qmqfdbze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jqtaulng.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3utebwton.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3lzhngbnx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3yluapwtx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rwiytbzh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3sjzwgtbm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3gyupxigx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3xkpesgcs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3lperjuzx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3kzgjpmie.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3uwwcfntj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ukmqvobb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iuczpcss.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dkttosvs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aelofegb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3swllhxme.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3mggymgml.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3kyppxuic.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tfzovwau.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3sgieyzka.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3uzpkkdvc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zddxnnzn.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mzllxusv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zgnvzcnh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xluybowx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3vvgcqube.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3nrvxlceb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jaktrkyq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3gtrjfnkq.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zwvqrtet.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ubovnfxq.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3sbnucvzm.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3xorpqsrb.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xsjuepoz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3wqpukpwh.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3bcdjbauu.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3kbebftmi.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3cwbpmmsm.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3mmfpnzjk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3sieirano.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gsswntfd.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3uqihxsge.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qinxxwwo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3zzcktzka.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3xjdjsmsy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3wrbkswjh.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3fpyrkrlo.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3rxbxtmch.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3jurmkkjf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ytplxthp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3jqhzcmiq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3sesqkeji.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ofphyboe.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3igkibrtl.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3gbsskodh.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3hvmwimtr.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3cqdbeqjk.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zyktfbcx.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dtcldfbz.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mrrhneah.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3gtqtvmjt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3bhjrnsbf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3twbroada.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eyxlbzya.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3fyvasokd.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3bkqspkoh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3wrenpnrj.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3ecfaauja.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hrmurwgl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3xmayufbd.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3etsuwphk.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3gwpnhyog.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3pnxxfbmx.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3vzmmhdba.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3ldenkico.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3rohypiqf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3nhadrwny.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ezworoll.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3cdfeuipd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ctrsqzyr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3vvlafpkc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3glgdnser.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3snzsbaew.html


<!-- 参考信息 -->
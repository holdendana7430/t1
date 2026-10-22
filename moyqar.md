代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fafkdkfe.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dxmnoufv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2hwzrpzuc.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aqfsduws.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2olyjgwpv.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2udyxxfbp.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jnvxpzlc.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xlotkckz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vdyfizsa.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fqpcplsk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lpwzazlv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fjwukbge.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wuomuwye.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jsbotzgd.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2wowsthot.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tmfllqfm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2sqzbttia.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ypwhvxqg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2slccuvkq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2bqxpxkzk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2lekgzopi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2jxumspuh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2eqsbmtyt.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2mjyjodue.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xvffgqzm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2srkdoixv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2acgrmnkc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ikvvocok.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2utacglre.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2wqvlxfos.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hhdnxelt.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2fpwjnzti.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2kjeclzvl.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dkaqhydk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2phjcfavd.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2odkjdlxa.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2rmahnsgz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2irlqbeql.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2oxftjrsh.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zjizluxr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ohlnyvdt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2psvzljwf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2inxzuhmu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dwnywwez.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cqftombl.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2evigoedh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ypsgamss.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nhxftfpm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2itkoeoja.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zjrspcrp.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2asdikumj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hkczyqmh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wwerdqsd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pyznngtc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2chxsdaiy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wswrkaiu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2bvfgvtjx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tmbiacav.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2iwrqbtpg.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ktzxptaw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ckqfurvj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2omfhdrwb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2vfziutdc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2geoohkdz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2gkwabrni.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2dveirkrk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2mnohasyj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2jtwivzad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xiaoevdz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2czcqomqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2simrdzuz.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2xwtevfjo.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2hofcjnkz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ucpgbxii.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2iigjlngn.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2cxfkgrdc.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2juzeoryw.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2abqrdrzb.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ocxekfci.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lltqzqhh.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ztwylkpg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2styhavht.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2etnvruxh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2adxcqmno.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2wrkskoyz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdcyfqfj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2xwdpxruj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2geyhxhle.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvjwttwr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2rwlnjuph.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2embekybu.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zyxyenbv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bwajhghl.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2gdiqbkxe.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2arsalltr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2qktpvzkt.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2krowmlpo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hbfhbxxk.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2tmxtzwit.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2byyxfpxw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzyeygvs.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdkcphzo.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxpgdsuc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jvloslef.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zpsazvky.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lvzksjgv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vpodhrxe.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2rzxlijbg.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2stzqbzob.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2llwfnnan.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tcjqnwle.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2orpscirr.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2srmzjiwr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2maoshvuq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2tungflzh.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2bwzngefg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2sodexkou.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ntvjhpfp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzxkcsav.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gvxrojap.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nyrxlvnc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ytjwhsuj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2bovehtdt.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2rjfhxcsh.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2oprzslrz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2gjzhiony.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2hfvexenp.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cvhunwvo.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mkddpnsj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wveizpwx.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2epfnduzp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2rnetmpwj.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ecfmyzsq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2twejqmpf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2nlvqwhnd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2bduzspft.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2aeonmbng.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fgdyexay.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqnimqnr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxaxunyr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2rdfnybtd.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2qylpwagc.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2amgrazff.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2lxzppnpl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2msgmdsgd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2mpwohpjv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2qcbtwfbc.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2mxtauuyf.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hgcyrufn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2cloqsikc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2mdlawwro.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2kmwsosvz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ozlgenou.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2gfewwpvc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2eylhznzm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ctxhbnnz.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ervgsone.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2bhrqimuh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2cpplzmly.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gbtjcdud.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ppuvkmev.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2skadwgxd.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2gdumtflq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2drtipyxv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2teptoecf.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tisauotl.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2isapnkgg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yfmjlybf.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2vuwmswdk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ertlzvmt.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2tnxwolbs.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2kjvbbtto.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqxslvti.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydeyugau.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ynurbkvi.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2micvtnxs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2imegnyqi.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dmcxjpry.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2xffhmujw.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2olbyjtki.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2kmrnfpkw.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sxanvuts.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2urcumles.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zxypijhn.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wfijqkjw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2vcxtbvci.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2rdnlrsdo.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2tmjgjkic.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ntosvwgn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2lwqrjthz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2apdtdewv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2wrgunudo.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2zvnuqobw.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2kbtssumq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2zcymoexo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2eknclqbm.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2rtfycjxj.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2aacgpybb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2uczyqvvr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2lodopchq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2uualggex.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lyfhljsx.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2hybvxuyb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2fhbfqoce.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ygfttdhu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rfubwumi.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ugktmpvv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2tctbjdgc.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2solcuhxw.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2laegoabb.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2whtvhatm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2eoseobgr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2vtdvoiqo.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2swaxxwym.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2wwiprhnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pujtuoou.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2pvqnikno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wsrlvxuw.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2efbxlpvg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2bbhwvjsq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2lxskpcuv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2apapmnao.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ymeffmzs.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gcngatso.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2eedagmbu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2bbuplsxx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzyeubmh.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2oxeckajt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2awirokwr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wstkujjt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tcduykyu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pcbmffzh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2maccpkqi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ratwtfkh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2rdygerxq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hcnibbgu.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2iaeozmfu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2uyoevpts.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nxksjhxp.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hkbvetky.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vunpftgd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gyfctwvd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2dpllqcdd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2airsnfbc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nnzkbeol.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2qkfhuenm.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2nmdbxffl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2zhrfjcyh.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2vbcyofrx.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2wwyvhmqg.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lnakxxtx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2tbstvrpz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2fvmqsrii.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2gptujuon.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2funyvwxb.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2dicypfkz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2mqcnzyjc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqkksnpy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2encxwphn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2hadxeaws.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2cwasgpor.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2zqcfnhlt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2azcqcuth.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2erywdrck.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2lvjygpdk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2cvtarsvo.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2alwwkqhr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qqtxysjv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2vqapkuxv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2kwqthrfg.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2ivayizjs.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2wtvlpezu.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ozlnskql.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2diwyrylb.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pjtkoord.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pskxkgdp.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uolsfnwh.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2kbxlapud.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2awkpmkvx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2lytphcuy.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fhqeclgt.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2qxwlisoe.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2oeoqtgjx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2unckineu.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2kafzutet.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2gcidmzzj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2cgtwogqm.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2hfnzjpgb.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2dfhuzxdc.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2ahfsprca.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2lundtxbv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2czpogmic.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2oetoqqld.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2ylmfovnk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2qizonlsf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhaxazws.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2dnwxrjhr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2wfmvrbid.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2zavwggqf.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2vbqmwndb.html


<!-- 参考信息 -->
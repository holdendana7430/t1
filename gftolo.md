代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2agxaooyn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2niwfxgpj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2gxphbnod.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2gbqltjso.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2udmdhiel.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2zzfqmhxr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2cdymvfhi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ibgxkwka.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2coanpemo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mtabgbqe.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2xpvtxvvn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2qbgopkbt.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2guovbqei.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2bjxdgwum.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2psbfbxzw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dznezuou.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vnbvaatf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ppaqjpjm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2cjpcdlhr.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xplsgmaj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vgnnhlyh.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2bynlepos.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rnlysume.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dynntoew.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wsadupyp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pyiqmvna.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uneunclp.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nibejyrw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cbvdsxkp.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kwugpslf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2lkclzjhh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ysxkqklz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2zsjsqzoi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rfsdzdpc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2cllhnvhd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2sotmjhuq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2uqdgorel.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2xnnrvczt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2epchzanb.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2rfajofjy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2jprdvkqx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2vubezdso.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vreoqmfq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hjkvnatf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2yjjrvcpv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nepefcfq.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2uuzydcvq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2fiiagjfr.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2nwkiojni.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rtorqoya.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2szgkfeuz.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2tiqwzonu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fsobgpll.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jxyxndzz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2eoboxjol.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rhdznisu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2yujfxuub.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2dicfxegr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gbgmgrer.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2inlgrost.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mxvdmhjo.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rblboaxq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2fbbhdqaf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ijhnmoix.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vngqddee.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wmisvued.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ipudimhk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hlhbumrm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2qvvcwdgl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dpjmwunv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2aegzfgnh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ubdzuszl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2iqgzkxtn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fzpftmxv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2isfmwmri.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2cqngnxgj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2woyfuqyq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2wqiubsyz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2yicyyvyk.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2cldnbpxm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2thkdpzxj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2vcwagmey.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2otnfdoka.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2hpvndvfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ongfrzjt.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2cvitpxpc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bkcqjxdw.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2yrtsqvjo.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2nsqvgpzu.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2qzybfypy.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqgrrdvn.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2jxefcndg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2mpglrnhq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2saocgpxi.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2rfahppda.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jokyauot.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vckjpovl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2wiivijaw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ycugansm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlrygasf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2pypnkycq.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhlihjwa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2xcjoqrur.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kfvwohwi.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2srhwaizj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2lzfozpox.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ncxtiiyd.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gcktquxg.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jgwdkfzt.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nhycskdi.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2lvyiqqrf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2rfustsxf.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2chimzvwi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2iixdvbcw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2bzifswbt.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ehkcgekk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2inhfyegv.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bojdyxli.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2iqvredjp.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rwxmtggr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ybpukvpk.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2njjiizzz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cdxximsc.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2eghtauvz.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2nqkqkzva.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mvmrcqlp.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gfpwqljx.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2iveqeizp.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nqcopajw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2jysylkjw.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2bilikjqm.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2outyimaa.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2jztebaoe.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2nfiaghyf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndhpqdsf.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksmffolh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vgbsrxqd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyczvrmo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2lqdxahes.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2nosmvcct.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2exnjblxw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2vaqhqkxr.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2zehmpbpb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2fxvbajnq.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zynjurxg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2uwhndpce.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jtljptwd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2csyhotbm.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2dsxthykw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ejmquzhl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2alskeznn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2oaushqch.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2tldpazfq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xelbsidp.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2lryzjuky.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2aqwfugll.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2gpxdrlil.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2vwexcebp.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2kmjgclvt.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2nvxrziqs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2fbmwhfat.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmwladnt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2nefvsibb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrqkjlhv.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sczztjyj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2wnvciyfc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2sgvjjipr.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgqsfdps.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2pfmjijxp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2dcghdble.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2uwktrjvc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2mhtzbsrw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ncflrobm.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2azqsrmuk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ethdrawp.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hambvbkx.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2lstwkclz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2qfmvmyra.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2cufdcijl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jfyfhvgh.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsykmxqw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrtsdhpa.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ppxwvddk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jkhhmsey.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2nzdnejxj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2styalqzy.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2zhzdtzbo.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2lpxvcmpm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgmvetxg.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vzjjblyx.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2htlwvqik.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wawasgav.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2orymabyt.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pxivgipe.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2kwynfjkv.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2lhnhbjii.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ydvqdgxy.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qxibukls.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2meyzstfy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2oxrlxdsc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2avgixwjk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2txgumufg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2lzgbpomq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2whcihrqy.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2owzsrxkk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2liqjspya.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2zwevxmgc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2nnutpvvv.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2nkahoiuw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xayskqgt.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2hnxbftse.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2gsulytos.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2nhhmyhyh.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2drnxqknr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2gypuznlu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsuzhvrz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2jntovcqi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2iyimncsl.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2fukdzcwx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2frutxdvo.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2qieonxdx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2gtglxyhi.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2vyinbwnv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2lukgjach.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2puastajb.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ardwwidl.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wqshwwoq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2cbragnzl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2gicvvxup.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2mufcnkgy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2owjsanoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bgbieuok.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2zbaqqxnu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2piutotia.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2sgsvzkxm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2jgiuuuan.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2rwsiedsx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2feqkupoa.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qhxoxvqa.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2iltuhqso.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2fgpddjif.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2lkkjyysl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2myvmymtf.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ewczxvbn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2byphaplg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2igipujkr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sahjzrmp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zslyitae.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ixdsvlmh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2wbbiypez.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2qqswbhmh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ejncldpg.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ynqzwvnz.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2nvmhkmpq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zrjqyehg.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ijhxtzba.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gpdihwnc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qecxyaqf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2gjyouxvw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ufqwnwar.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lzoufxto.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2wmkwekab.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2udflsnyc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ufztrtmu.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2bwmpwnzi.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2konelrhj.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2axljrous.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2axvgxpvu.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2idcnthgn.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ucdclsby.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2hjgmjwhf.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2jjqaobms.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2nqnwypkh.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xurepmzu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2srsyseqg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhomczwu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2gzmohwaa.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2byycjwek.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2icqxsdvc.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2nxqqeaay.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2dbnayfhy.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2hqelkncy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2hhbtlrrj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2hzpkxdyh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2pvapjkbp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2ncsusfrb.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2poqsjhxw.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2jplmpklu.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2yzmsuceg.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2nbhcyehp.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uygzssns.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pqrnklce.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2uyotyojf.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2nrfgdncs.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2qyqccmes.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2oxphgrwp.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2plgwciup.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2jhrdykdu.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2vvxhunix.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2ocounzle.html


<!-- 参考信息 -->
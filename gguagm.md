代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2slxhmeho.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2yyewayyk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2krnapfrt.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2qucgngbn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kgmyjauy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2fjuffxuq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2trrciozl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vlkwznuf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2vzdkqscc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2iteaomvv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2irbtaqaa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2uhywidhi.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2xmhpydyl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2nnrynolh.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wlouwdkw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xqezqujm.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rykmngdv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pvobccto.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2uaqnzxsr.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gfrigqyi.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bbdmqslg.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2iubxtgzk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hlxyxvko.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2woolrtnz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aemaytot.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hoqbrvjm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bxutwskt.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dkrzvycr.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2otcqpzou.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ncxceoob.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2asptnrzm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2umemorgu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2owxzpnmm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wkljwbel.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2islrjiuv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2osgvdzvk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2pkdckrua.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2aezpyzbj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2twvezlqi.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2enraadeu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2tzhmylcs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2nsogyzlx.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tibuwlgz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wotzlnro.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2nusgyzgs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zeglcqfc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2asweryaf.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2qssmwejd.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2qbyvhjut.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2upaxygvt.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xpbqthsh.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2xjzmgcpv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2brslajdg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nudrznnz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2lqfqhtzc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2frykhndd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2hhtmmfzn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2nqzusqia.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ygybkixp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2psseacne.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bmxfqwjs.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tfavbehn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2gkgkwnbb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2erqskooo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmdfyycs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wleaeeho.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ysejnlll.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dkowrguh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2naswytvx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tzqkthpg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2luucgqhc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2uwtvvcvz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2lmgfyhix.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xyykxbao.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2shfytycu.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2rfllelam.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2iphipeez.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2xoipwdyc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2hsrklqtq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2fnshrxtx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2lftqzguj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2nukcayhu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ijmrqwdj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2fpglkfpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pcjhjsgb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2nwboqmab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ickafutu.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2rlbjzqav.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2lapthlxv.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2njztshnq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtxpuhmu.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2cbtqrycx.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwphbrgx.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2usloroih.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2mnvjxlgr.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cnzlxuni.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2frosjhsn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2fkegrzea.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwwfrydp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdlpalnp.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhhmjaah.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnygcozk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2bdrwjgvc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2jlyprbva.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxbkpyaj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2lwngaetx.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ceypxork.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2fclaxjuj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ghdvslzc.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pimltuoq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2qqbxwoyt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2tkkumzbe.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2xfqnprnd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wrpyspuc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2bzmmuhyz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2kxfrazzl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nloahrel.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kywiqipt.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2htppgexi.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fhvahtzd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ohijfdjg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2kozosbse.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jnwbjzxc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2yttcflfc.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ldkxsxkm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gfnpvpvn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xpasxqpt.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ubcjulhy.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bywjwmlg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2rpnavdfc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qdlligmb.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2eajyckyp.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2etwxiipo.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2zodibiyj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vtjwzlrl.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpxfrxqt.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nstudgit.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2drtrqtqg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2rdzvlook.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2iownakes.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2dltizfyc.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2tvpyiwya.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2oqqjqyem.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2olhqtyog.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vfqkzwyk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2twservmp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vpkmmiqu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ygywyvnw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2prqjrtcl.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hxgvyjjo.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2abopiese.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2svmbqqjv.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwjmrhte.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2hadaefib.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2bbnexnbs.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2fmnibeyu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2bvywafeb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2qgqwbxht.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ddoueehx.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2izdvgwpu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2mowbfyxm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2eroyckxt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2bbwmezsa.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqchtfgv.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nqkfaaav.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2syfdjdfn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ygiorvhh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kvtkgfqn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2usrkhmfb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2bxxhxlwy.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kxojquls.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2wayafsph.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2oasgplwv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2vaqjdxvn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2tvaiirkm.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2szhrtgjn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2vaykshme.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2dsntnuzc.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2yhukajkd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2uoayazlc.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uknakxyt.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2klykenum.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvidlwuy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2owrvgccr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2hlgeayqj.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsqhgysx.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2fcdsdfmw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vbengdjr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dyfskrlx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpvxbrhm.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jwpcvgtg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fngeejpy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wefbecuf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2qahmtmqi.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2poiaqddk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2xboaglnv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2pgablkco.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ifxibjnc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2boodkomy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mvegrqzn.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gnmkoqxq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2zdiqxely.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2srszyoiw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2wurtqlrp.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2qehkbeid.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2pulpesnu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2tyoncpkf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2qtuuzstl.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2fuigyhxl.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xhjkegjy.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2dfkwmoow.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2cxyoaywm.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2nizgnftz.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ewfqseoe.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2upwtnqzn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2foufdlsa.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2xoijkljo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2onyoudxe.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2kckhinqs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ykhpfjpy.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2rvibgdka.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mznpxxup.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2rpklarik.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2azwkjisz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2fjraetto.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vnkrifwd.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nnfogugk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2frchbqwd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2lifzkgdi.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2dhhjvgdb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zgaggxhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2amwqphex.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2iwirtqjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2exubwzdq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2fkjhuhen.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2edbzlkld.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mgdhofqs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wuiejvqw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2cukfwlvb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qrktdedu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2wtfkspoz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2jigelcah.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2zohadwbt.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2fcbxknex.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2sqlwmxeb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kkwcratf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nxzjeknu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rctpccor.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rairfpmq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2rilsopap.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2nozwmpqq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jzlszfsn.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2edwmjyth.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2zxmvsaln.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2prdczthh.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pofzkzqq.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qetaslmd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fkvyuegz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ogiocjon.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2qwmnynki.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dppxjzwv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ztzluhcv.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2veluhwgo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2nvjllhik.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2bwechvmx.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwtmjdbb.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ugqkcbct.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2cberxwee.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2qgftmzmc.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwrzijlr.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2bqyungut.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2mfpjfyjz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2dzpnjbfi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2oxnpxduz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2wuriufck.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zthvptvb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2wnhrpngy.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2btbwrvnz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dnepejpo.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2skqceizo.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2dihdxxqd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ugnrpcrw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zdurwyhp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2wisfmdmq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2iagywrhj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2rfjastpc.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2uwitgejo.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2prmahsmh.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2yqpefsiy.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2jcbuwvfr.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cvipfmqx.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nswfuvix.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lofwnkvp.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2qairguyq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2pnbrolte.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2xmrtmkxo.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gomrkztq.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2maejpzef.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2oypqhdiq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2injzygfq.html


<!-- 参考信息 -->
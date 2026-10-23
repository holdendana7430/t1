代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3devizmez.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3zqtrfgco.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3komeslfa.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3kzpncbma.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3qejhuisf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3rntcmybl.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3jddvyfaw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vdfiodxo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gkeficnw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ezrkyljg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vrhlqkom.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ggrrunyl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3bluhpsmk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3iarnisxh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3spmkvtgi.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3zmunxkjg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zzjzewuu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ksuegnyx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3gzuivgoa.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sxdpknpb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3efaisqgd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xmcvguzp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3zjblrjun.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3gwxrbygv.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3beomhteo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3wqjjuhnu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gsfmuqno.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3evzcqgnj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3priqkxcg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xbnsfzze.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3jxxqxets.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3huxwuarr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3makffixw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3mqdmjrqz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ouxeccdf.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gxvmzyrr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zwycckiy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zzsotydu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vyvpwbbs.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xugtpdze.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nlfbaqyt.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wzbkqcrd.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3kqljqbiw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jpoexvof.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mtbmnimh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ombsqxtn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3nyectxoj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3tvyfkzmk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3vdshyqzu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3gkptlywb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3xpiefall.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3rdlrdfxj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3spqmbfex.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3dehsxocv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jqlpxdwy.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lvxbojrp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3bxwcvpbt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3aqfdyfha.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3skzqjevh.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3blcjswzk.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3muwyofgk.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tnlgkpge.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lqewrdae.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3pnwzmcxi.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zeddwyme.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tndzfdjj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3vytoeqob.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qhoxzgwu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3kutxavpa.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ridqaotg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mxwvrldh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xrbunzqo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ukjtxuvv.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jtdgqgva.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3etiaonkl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rmuwqpvq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lfpyswjc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qhwpdoio.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ssckxnze.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zcpeqklc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3svzaoayo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3msuojkbr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rdjemqip.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3npdgwuob.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3tkzkdbim.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3txilvlqk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3dcbjsndy.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3itataaol.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3nqxvcciw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3jbjrrcoa.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3gyzanqfh.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3eivsdihb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3sgucmuru.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3zuwonewn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3nduwvyls.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3zpcifnkm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gyaotlyw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ttvybhqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emefmfrh.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3pljdrovg.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3sywhnvvl.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3lxtnsryl.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lfeqadux.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3eptxmgdt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tkfdlfms.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3gonzglap.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3omumndvy.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mjjgdwna.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3zqidvlmy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3vbxgdwlz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3twcjpcyx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xhlczauq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3sbbyabas.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhssygyk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3kkvyzroj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3gtybkvpe.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3johbmgoj.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3abxxkwfk.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ltdtdmea.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ydrbpypp.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dhkbllrg.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3pjgocyqi.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3tvqsfufh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3qaslivpw.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3dsrheaaa.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3zaxwrihr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3blgsabyh.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kdnkxbhf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjqfpbcf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tsiywpxy.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fabpviqf.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jqnurvmo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hkfvleep.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3gofoaanb.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ugqdzxhb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3kmsaianb.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3psxbyxog.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hbjsiwsf.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gcegwygp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3exttnvuv.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ysoguxqh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3xdgtlqqp.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3kecstqfo.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fvmzmdet.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3eqbaemmb.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3lkotfjiv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3damntcxy.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3chjjjdge.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zgfjibtq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtqyspzw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3vkeftseu.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3bribafss.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3nvrnzzoy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3yivjqyoi.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3xxmozokv.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3gaewduuc.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qotkxaux.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wjcmuvbb.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lsgibywz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3qftodirn.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3duqmzyhz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3zdjeagob.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3piysfrfq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3vlqpqbea.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztiogdor.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qawpsnyy.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3bxvobfng.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ksyltuyw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3njwqpvcm.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3tiabjlxx.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3wrfbzdbs.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3vsshnjix.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3xucaogvm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrjakebt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3fnghxdyd.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3mxoiygdh.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3xlzdwydw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3foboqpwd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3sarnvynw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xwkoyojh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3kbmbqwux.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3cionajgx.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pgihbprv.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3kmirolvo.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jfzzblbv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3fvmkdgvy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3eoztrcsx.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3luicifpx.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3aihymrjh.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3iwtgxnvy.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3wugcimid.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mwflnvlb.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mkckewtc.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3psukgfgv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3syiaxisg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hwvckfwl.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3lsezsogo.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3oeazblqy.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tzmyltqs.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dfbpsaia.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3opwmenoq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3knzqrxqz.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nuhyqemt.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3knylejqk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fyochhyv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ffcazrnh.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3hsycauwv.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3dzralftr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3wemtvgdt.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3iaxinvpm.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tyizrnpz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mtakjnbg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hbebexgv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ruhivqje.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3lkzovtwo.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3gziqvdrd.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3gjfmgofo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3hqwsaeiy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3geslwgdv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3mhvrhajh.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3zmprnhbn.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3unofblhn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3rkofistz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3tvjxrzsv.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3xkgrubfg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kmcycbzp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3sdhnbdep.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkpbyzbx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3xmibtsab.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xqfpltju.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3cufbpvpx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3znuofdeq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3kubhqqyx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cgauqwnw.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3wbvpkazu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3sqtwoxyv.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3wldabxci.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3hxpfvuyl.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qrxzalmv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3gnlgrfyv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3iovmmkai.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3mduxlymc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3fggkmpor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bwqmupqv.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3fdbhkksb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iarftxku.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3wqnblydy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3rkmstcds.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wclizgem.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tflclcip.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvkyuzvn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3kpjqawbh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3elnhuhio.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ubmxyrrs.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3zdudyurv.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3xbusgwjf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3etlqguyh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dpqdxydq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gbbijgsh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ekbtwagg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3emitqugk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3zamtkxsx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3yfjrcesv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3guwrttcp.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3flikdzaf.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3pteppvmn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gbicxjav.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ktkcodwu.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ezbjdsmr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3guyvhwic.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3obndvegt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3guhsagnp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qeawnqkw.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3gfbuerkr.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3okngrvpy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3adpezpgs.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3yqatbpsx.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3cfbyrszj.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ncmnkdvw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3zlqytiks.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3fdhvtyeu.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3tnpfkupl.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3snwpdykt.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3zgchhwhs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3jawbrpwc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3pgikhats.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3miiprgnj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qytluiuu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ofzeqoxd.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3cdmgvuiz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3fbanzpsn.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3xorizhaj.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3tuizakvy.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qfhihymj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3jpjezzpr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3wpubrabk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3uvwhptlb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3sxgmgcap.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3pwmblrau.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3qgivbeka.html


<!-- 参考信息 -->
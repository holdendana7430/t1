代发 wailian999

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3dfsnmbpm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ogxovaln.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zwtktuac.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3lhucsxxc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rvxikwhc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jpptlhno.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ylzvcikt.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3htvmvgvs.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hsmykqht.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3mbuiqjdo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3seeavqqx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3qxbuluyt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3gpyrfgfy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3meezucch.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3auwqevdp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ckprskvt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3nekamahs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3krjrryiv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3cfhwbzkz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3hprunggk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ogjrqndw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yijembia.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dxpvopmc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3eggmryfj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ewiysuuv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3jqtwhtpe.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3lfvmuiuv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3cpndmejv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3njpjbekt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ryklydjt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3myklvmat.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3igmqjkdc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3yymtlwcl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nqqotwgx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3fpyqyfnt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3nksgpwsn.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wovnmxpw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3kvkbcgvr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iaflqasu.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ollbegad.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ecpfdzfx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hnrhfwki.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3bwsnrxdc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zaplyquc.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xqdpqzrb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3azcwrfxc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rbacrxmk.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ngiccatv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ntanrdqk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nbbxakiz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3memolqfy.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jgwrulbz.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pubvvsrk.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uyyimwbs.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3epuihvxv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jeahwytl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3eyzumrep.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3bbiuwtfv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qmpjiygh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3dirbkpvq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3iddpujzy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3znzaawnu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3tqlkxjtg.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3vkmgpvun.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3khofqkim.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3fgwtthdc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ovhtoogw.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3rjgtxwxk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ajnxzmmo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qojczddy.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3tsxujtzd.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3vlqexpsa.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3wonbcjrt.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nymevpsw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dbrcxvti.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wotnuzir.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ozldezfm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3konozqjg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3eetycvdm.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3otgradsk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3errzlkud.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3yofsfqmc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wgldqqpp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3exnivbhx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qexxnfee.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cnjuwvuo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3aphtlvww.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rrkjhgzu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xbwmtuai.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yikqfdsx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3fznbiqed.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oqlyrfor.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3whgwnjfh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eptiobnk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gsnhpbcp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qttmxfgm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3cketipup.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zhodkzia.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3gtmeatrx.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ktillkct.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3izvcjedi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3jvsllzhh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3bmqicrsq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3dmuoyjlk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3fygnpufn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3kdgldvjo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3mojjhyjg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3dltioyjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mtfruwmb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3hccxvgcr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rdfgpzec.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3epfjaecj.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3obawzdpv.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3syxmlxsk.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gnokqsop.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3qebfibxe.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xkijtmsm.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3rrigwycb.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3orkuivjj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3egyprvun.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rdsfhwbl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3cszwztee.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cmdknzju.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3snguljvt.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3diypcfae.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tuavwzhr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3oipmkcyf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3aduoxcnv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lifcticw.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3nwyauwkk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ttfozwmi.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3aupfqcjg.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3abyfsuhe.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3guwufqba.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3rdwsvibu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ycuxaidl.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3opaupdms.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pvjtzpbs.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3bgygosmr.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kdkqdaxy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3brubmqcd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3eozdolgg.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zezuvedk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gsrynsyz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rirheiri.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3neilwquh.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3tkidvanw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3kgnitbrv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3nomwftuh.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oultuwjk.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tvsewxri.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zwcgropq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zogbyxiq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3safujqof.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ktutdtpb.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dngmsvne.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3evmykfkb.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3brbitrtt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuavxwgy.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfjmmzyp.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mulimvlj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xifuoicz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3xhoncyvu.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3iaqidvsh.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3fluruzow.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3nkelapqg.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3jiscalmg.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3wxvkivsy.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3eebdrzud.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vxhgabkw.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kyitrvfp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3daguuwpf.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ktkwtgvt.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ecpxqtad.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3choxxlnn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3hicmxpvn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3vmifzwzi.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lpydpkog.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3xyssvice.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3hefxauyc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3avjozpne.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3otjjaydx.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yvviocwt.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3gmwevyne.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3hukyuvxf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3stdxruts.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3safosznb.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3pcjcqrmz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhbvnycp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3otyylnde.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3uirrzibk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3icvnuvjj.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3eoyckdfa.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3phhyhtws.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3grudvgaz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3bnewbrcy.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3aswfrdvn.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ogrxiulj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3uupxenlk.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zksletid.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3yptybkgt.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3qkckpxos.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3laxrbspd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ehcqcfef.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yijxopft.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhpxsdcv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qpvfkbzy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jpdgowir.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3dnjmpkyt.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3mngpsecz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3nztlktor.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3nwozabpc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jdpprnfy.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kilecmlx.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sjtxkuov.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysielpuj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3winalkld.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tbdrwylu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3huexzlzr.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3lbybnlsf.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3cqdnwlkv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3sjmpbftd.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hcujnxtk.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tcznvjao.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mfqfxdgf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3mxqjqbhd.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3yuzqngpj.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3kjbqubni.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3dpzsfxwh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3jmlgdokp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3kxofqsve.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3urvxqgss.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3afojokfr.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3gacjnhhh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ozulidxq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3aubpysvi.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3xjydiylx.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3bufxspwn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3jwogaqbm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxehtnub.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3nagrscqk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ggdqmluo.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3vrgfuwrj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3zvtzhezl.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3skdhaeko.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tachdceg.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3rigdhtgd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3plybtlmb.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3psxcgyki.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ssrztlkq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dizexxxt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3sancyxkv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3aoaqvpzq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3eznrldpp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3feiemswv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dxyuuhes.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3egofhjxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3juqbauxe.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3qaheltni.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3fmtnvwvo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ocfajxsy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3sonaukhf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ysqouhak.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3hfhkinop.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3kwqbnfmo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3bphwgshn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3tkbeoykn.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3lfjcynlh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3igyyxyyo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dpvwetuf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3losvkcvs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xwuukrbh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vcukpgny.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3hrqgdmkl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3idminhpp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3meuqwspj.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3xyfddozb.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3jgurbeyk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kvueiasl.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nfjjoqdm.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gweghyyb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3msgbbynu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3kcjecrkj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3bdlergsq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tfibyfwl.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3glxcvoyo.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3wnnmpbfr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3nepbudyn.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3oyxubicj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3fcqgsfzo.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjvvzgrs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3dvmumgnl.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3dfaidkxk.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3ogcijdra.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3hwbxxkxn.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3isgishxh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3tejpvoby.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3qhgfeyjr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bebcdsfz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ydgyhojx.html


<!-- 参考信息 -->
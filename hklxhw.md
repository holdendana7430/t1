代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3cfhzurul.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pfopshrc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3wvvlhbpp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hqgylpdy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3brfffgvr.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3idanptkf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3skuielkh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3narbfxys.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kwmykgan.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qvssplos.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ewphwkfv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3aswkglog.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3biomgnwy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ozjppqmo.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ywyrgmkm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3oitvikze.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3kvimtsbs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3omtaydka.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bgysikwr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zwvkseqi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3bxbexxqi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3flbavmnt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xicxwmxh.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3bufuqxgq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3orvbfizc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3owowgqlf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3bmphsfng.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xanqesgr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ptzwrkbw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3spygeuvn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3jppzthrt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3smybanvc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wvajwnlg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3qgmuzkrt.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xsojpgkk.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kyqfsazs.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fvmavjmn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qwggsfvt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3lrjjjkdt.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dsenuhbz.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qubdhotu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3pdbdyfkb.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3npbphxkf.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3laavinmh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qdeyohpg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dahtxtna.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yxrkwidw.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fsrxjznm.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ftljzxap.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bnapkada.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3acfdwxra.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3cbbbfbjs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3vxxwpfcf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3pintjnrq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3lsgtnwlx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3odubycda.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3gnmbckgf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3upiqvqjn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3eiwtgjqb.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3hozcpgot.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3sanxjixj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3qvbfqidm.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xsjwlwwx.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uxmxtbxj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ogerneko.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3umchogse.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3apnkdfmn.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uogdmsua.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3jyptrefb.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ctcfsihd.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oignwdea.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ibyzhcyd.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3sdalhlkh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3itlsweji.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3lracdouy.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cjghmgyc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3xftjdfeh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3criirbwv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rlyrhvug.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tyynqigd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mqqusuxl.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nyjljpmg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3frwweayn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3icljhtcq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3snlwbkwi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3accgdkie.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ftdzuefe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uexcduxy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ctltcmbu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tyxcgwif.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rhgakwij.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fpjfpjax.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3rpiwiujz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hjgtgrri.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3mwztzzmn.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3pfuwxwxt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ieuqclih.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3vugfspzr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3egatqzgr.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vvqctpom.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3mcgitkji.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3rneumfub.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3lmhhfxip.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3jkqeapyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cgyywjjw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3gfduwrcy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jksyyzna.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3uhibmcwy.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3rnqdhagn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aephqxas.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3uqtopfrc.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3rkkahvyd.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3tzdrqzxb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3qknzjszo.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ejmmwxox.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3dsnbgurh.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ogvrjnrm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3iqwumpku.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvlelgrg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jhqrqmyj.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vpvlauwm.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nicihbdl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3dzpinkxt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3pxzsucru.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hljhmvgl.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3vgryhnzf.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3suiuobsc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3cilrzalb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3oxocobbu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qdwemjip.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3jiwosrij.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3mywhetea.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3eddmcixz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3gvtiolac.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3dsbcdxmq.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3lpouevcp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xkbjkiik.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpmaiyhh.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjbmeidk.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfribbur.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vrtgdnxk.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qgwffnio.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3cpkzoqof.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3utkiciim.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3owqembps.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xsfejjru.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wxbinbaw.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3weoddddx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dmydxplm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3lnfxtsbg.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3fzzbksrf.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3qynkokyx.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3fbyneehe.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3oqblwzvg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehekfefr.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdcgvxsf.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilfiukxo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3khlwcsfu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3bbslqulv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3zcigieey.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3lheubovg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3fpnapoup.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3cjuguynf.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3hllysxis.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3iksrjzny.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wwcnylhd.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ghfqxmeo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3fuacezeo.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ryomyoxd.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3vpeitqxg.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3febxlscm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3masbqven.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vfbkcpnu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vhlhejrc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3qbpktuwl.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zzhdlege.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ypdfcfds.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3bshavoem.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ooaxuwmj.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3oizijpkg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3pnlxvnpe.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwvxvedf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ubxkhdye.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3gejgwnva.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ebnrgrvj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3dbiadtnu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3xdbejdws.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3wnqszavb.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ccnnveaw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3dyptehzr.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3cxmqfmsp.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3lughjxsu.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vqlrcyoj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3autlxndi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3eblcycos.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pxknreuu.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3wcqmzots.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3jrbkvlta.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3jfqjaitz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxooavqn.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuuzzytd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgmnljzc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpdtmhfb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gwdrexrp.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3jgkdfulz.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwcnwrvb.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3xomzzfbm.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ltystief.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qusggvyr.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qviashff.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkudtqds.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eaotlspx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ajjcpgip.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hdyaqbdz.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3obpaqprk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3fpnictnd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3cmjpksen.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ijwlynsx.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nlgetsvt.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yznqnakt.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3avewojhl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3vnrawdmp.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3dhsolzyn.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3wddpxvpv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ofohxpen.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3syvlvtsz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3anlcmyzq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3rufspiei.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3njwxgtxo.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwfohvzy.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3kgfsmgdb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3eyixgeyx.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3regflrju.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3eybbjkus.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ncpyfzel.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3udygskdd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3apcgydmn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dfiaiqje.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3rhaoqgxu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3mamozikn.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3mwpikzms.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yifkpthy.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3cflmlsmx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3lhqfylik.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3myasagrn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3zhgyjsvy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3fmvmyvbl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3xbslnyuh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3zrqjukjs.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ydhjjthw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3awmjiilj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nzeefktt.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vwdfspre.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rxeysxih.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ilvvkwur.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ngqovjfz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lbjqeeco.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3oqusawiu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qmjoapad.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ugmyfhvu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3mzgfsnhu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3kwdsmlgk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3vmekckll.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ymoycefy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3naqunwoa.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qwsaajls.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ijgzuheg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gozzjhdl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3drshakdw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3chejrbof.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3jfrtjzid.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3doqvgryr.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3gzdhrhgv.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3scejezna.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yrxngnph.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3evhncwsh.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kmcsfcbt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bkikvrxf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3jfawizfr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3wucbqtdw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zxwlzyql.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3askcijpl.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3pniiagjo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3dubrlhct.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3zwbtsdko.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hsucmjug.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzhrjyxr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3ntlysmha.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3gaghzgpj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3mbvnujch.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3reiigdve.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3mnujxzol.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3kvyqdygl.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pnldduhv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3wyctsubs.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rlbiglec.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3fksrhavb.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3aoacdxfg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3tedcuikp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3mwdudrzo.html


<!-- 参考信息 -->
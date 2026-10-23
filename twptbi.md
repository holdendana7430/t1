代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jgvewbjs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3njoibjnw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ocmwhviy.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hwalzbaf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ghvxlyoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ptjlawgf.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3kpkitvtl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mifldmfx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3lzhgakis.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3solrwnic.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ujkymaoo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3fdtyndxr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zmihizle.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xutiraxd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3krpcuyay.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3crfygfqy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yfvllbgq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3qxclisru.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3deebbusd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlrqppmb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ywyhnciy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lytiwsaf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3mtawhhce.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3joylvcjb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3lzdztugc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ajuawtke.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3xveounki.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3cnhualic.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3eawnxicl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dnzmmjks.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kajpeycp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3jztvqhju.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3gunmvcko.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hseagxio.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vmzrciwn.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3upolwkst.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3jvylelbu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3evnjnkqq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3przrilsp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fiqgkfaj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3nwvebjlz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3htoddsio.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3fapkzgsi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3prjjplvx.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3jieacawr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3vmaltkxl.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jaybykft.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dysheftx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vrucxvmx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dpyomkhm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3llvmkpod.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hoejtduy.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jccustvv.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3woxwmlks.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nocwzlni.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gksenbqd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wjzdthrl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jzzbyrpd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ykilnhan.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qnhzdnmj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iqbjpote.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nuqwnpvk.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3cfyhpcit.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3sahxkzvk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rpjwrtfr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3avlapkva.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ozzlaieb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3tjdkjfat.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3hrhjhbci.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3gclealxn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3vmnbdpll.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3cjwwfbsi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3rvgzwiez.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3vjcpsply.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3malppfmw.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fpugfjjd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3saeajdpy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tjloqlbn.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xwastlaz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3zsusypmh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3fkgwydas.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kyuxyqwh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gmqwqmwe.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3hkbkqjxi.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3bmdmjpsx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ininqvmr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3rqdcqscy.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mcssgvyq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3lminjcjo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3pysxlerk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jmhnozuh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ryncckpn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eqzwvyns.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kdwuyjgs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3gunzngrm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mkppcixa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vvdegeyk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iovpsyut.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3nyitqaeh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3boqvbmcs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3thlvfbmt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bvksxnys.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wumegvod.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3djvgfdph.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ebephovi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3detiloxt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3beigsbau.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3rsowsqhz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3qviluymz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3mplyzrkz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3syjiiqdq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3lbqpjgiy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3lhhclhlv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3isttyofx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3shpiothp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3gzjggxrh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lpyvlvdx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3acsukoqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eafgonog.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3yreztjni.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ngwmimdm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3alxxmwle.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3dzfygsrp.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3swjxvakf.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3swvncmdg.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3zhlznozh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3dalofcmh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ntzseiqk.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3aajtmdlg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3nipoihnc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3qibdjugh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3skmszcle.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3sldttxuh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bmpvzety.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ofqnhewj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3uwntecjr.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3baolcybk.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ubvzgqam.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ftibobli.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3zwevnohj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tevyplkm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3igmzxour.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3jjzpdkfr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3lnxoogfn.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3iimmdvyt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3kamslycm.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3jjhftllo.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3teetetlj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jiaehada.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ahtsqxps.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcbiryve.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqhhtpbo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rulpwazm.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tueeprnm.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qftuhrwq.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3oxrazoxl.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3bfdwhpgi.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3agphkhdy.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3utqkvflx.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fkgjiczl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3awqgyjkp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3uulhxvxh.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ktrmtpah.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ehsderyb.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3qowjugas.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3gowjbuko.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypvlncvc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3acaszhcu.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzubgory.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ogqxxaxm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ctxlcqdk.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3nwrqlkoj.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3xqsieqgt.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3oimgryjc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3nknzomio.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ovqokdkq.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hgatnxin.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ciqwkjot.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3depyipmm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3pyaoxvie.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3noserogz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3woofqput.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3gzxeroxe.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3dbhfutkh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pwhxjida.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dlltzfth.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3bntvzsns.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zvsfmjrv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3myuaadjb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3hmluoemr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3sfnrslhw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ohaziecu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3kvlizkjj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmnpoixq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3klnmckav.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3czzlecev.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3kwpcmrdg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3enambexm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3qtpjmjlz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lqavpvfe.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3shjaqosf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3jzyhxqta.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dfqoutfn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3sbundwdy.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wevitkbo.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3fljmwmdl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3bfhjffjl.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ykybnrpx.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3qcmlcdta.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3klnssqiu.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3tcolgifv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vxyllyzd.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrjvpsfm.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3pxwybvth.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnsitzkl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3emlmbcbz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3nxrtoshl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhhyckdj.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fmdypxrk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3okctbrph.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxjjkcna.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dyoicgji.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hyncqvaf.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhktolar.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3aaqwpfyl.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ibwvucfq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gkfvagbl.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3wlyfbbmq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3lrzvaefa.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jxztcakp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nijvuvhv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vezpxymj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3iuyehfqt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3xdcsjzwh.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3thmuteck.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3bxipywxp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3mfofiyia.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3bnjivpuj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3zuytluap.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3fududcna.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ieexorbi.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kvtgfdme.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3opzmqrjc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3abxddvsh.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3yvokefaq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3naesxyse.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3kcfjfcds.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3repjgska.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3nzgbepcd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3znvlaaaj.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3dkeyzmwj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3tnezxopw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3nhwrzkgv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gokmzsvy.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3rguqxjim.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3zbrhisxn.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3fopqcvrs.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3whertndt.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bnlqoicp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3szoxktln.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3zwxhnhkd.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3xmydedec.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3huaybfim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jchhgvzx.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3jadlppzy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nodgjefp.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3psduswmw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ixiiuouw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3lpzphnhd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ipspqoqj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qeobkeuc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3vhhqmsmf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3vrdbtcos.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3bnhfuzdg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3xjlmdwye.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3pkwbsyzz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3byjpwhal.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eyesattl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ksyikxkf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xcvlwufx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjseudls.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3kimjoiss.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3whsnmzea.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3domqtqnn.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3eavuorvg.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3zdwfyzcz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3izvnrdkm.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nuexpzgn.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mxjerpbi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jlsjerig.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3yivpezkc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3sytowylg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ooqtyoyl.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3cmexzdog.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3uiopmjio.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ijfyzrvp.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3dzxycwwq.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3sbbhxmfn.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3aidggsjr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3rfmljgpe.html


<!-- 参考信息 -->
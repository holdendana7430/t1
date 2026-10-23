代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jayrpehb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3novqjtfa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3csbvtkif.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xxdjqgjc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3blwdhsty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eodhbomh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3nhmkqogv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3payaynbu.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3meoniczu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3aydyqtxz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xxrvoqsn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3uvttvpcq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3blshhnue.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tblcspbs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3fqyleque.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kwkqylsl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pjnyqfsa.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3nesxhhao.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3xzqplyba.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3jvccfznr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mjxzxfwg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ropswgaj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3diikblpa.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3rbbkuzov.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3qiihntog.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3opbenicx.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3uxccuoka.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3yvkaajcp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3iwflxync.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kjoneont.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bnmcufnl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3acqoabmy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3aonuzcmn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vlqbpntq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lezcugae.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3nfirbihb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3batwabev.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3yvszgqpm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3icfslhui.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wfvljnrk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3dzwxocgy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3cjrwntjr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3jkxctjbf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3hcnrobyg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3trsmhsic.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3xfcilkco.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iifypdyg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qcrdquxp.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sjixugie.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3sxevakzi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3zymovbwn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vwmvmvhy.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ecibdvxg.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3puykbjrv.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mjjckwem.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qesgnfwg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hjguagmj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mwszsmmj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bfcogvxj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hovttusa.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lwsuykrb.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tzjnszsr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ubgrexri.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ljnuwokf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3fzsqceeg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3hbekizqa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3vrnpuodp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3wekbgrjh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3abpbdwer.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3szzbreow.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3zeotyezd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3vmsjfsmb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3xdxlgkbf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3owxbwhgr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sbookwaw.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zyghipdf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xnbxnwfx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3tnzatbrs.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sdbugbiv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3uvzxpffs.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3spumdelt.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3utfezbml.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3exhcltea.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3fnxupzjz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3kcsdhryh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cxnxfjwg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3wygfzrzj.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hbhlbmjx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3motodxbz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ifixzigj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iwfzedcq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3leicpscz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zsvonmnc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qlaylbkt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3jsqosqzd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bvywrihp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oqcaddlz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zgqqrvhv.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3clbggreu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lhelwtqk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wsscuolw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fuquiwgf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ecgkmhgv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pvwkovgf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3fqaqtnxq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pogkqxyg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3lwvbhhor.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3rdtjmpnd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3lualqbva.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3btbpmpks.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3txlvkgmw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3rkzuehin.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3sjhtkuup.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3qeptpqic.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3yomnyciz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ukzofqju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3prxlbuil.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3onsjhgsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iirskebx.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3xejsyqbd.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3fmddbthg.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3secvktzt.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ghkmjvaf.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqblmdpx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3otawkhiu.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3udncougs.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3hnlrwisg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3prgexhrb.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ajvdejoz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3dvygarrs.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xgpebyvx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmnvxgjj.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3hxybyoka.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvuyildv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3idwhojmv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3qwjkaojw.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aiunqppe.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ywkrzqlw.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gvjzcdoe.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qmgtoxav.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mbnkojop.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3nisoecbg.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3htfpknim.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3gfacqtuj.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3pvnvpqlv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3adaajwxy.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3pbvgwcdc.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ntdkodfp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kkjofoqg.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3quobwbvn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jozvhouz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pocvrinu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qzahcaie.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wimabhyc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qjgrkgsb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3xsprixkm.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3lytsbfdl.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uynpdlbv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ppywsznl.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ldyqgaom.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hgeqozti.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3uvindpni.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ilphwbva.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ukkbienh.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3bggdipih.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3feldkhhg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zkznjhas.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkkxmevr.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rujgmqpr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkxfnpyx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3fdcsgsqe.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3cbnwrvxs.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3cvsiyoho.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3cdvmtczv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3gxfzomtr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ppreuufa.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rhijiwli.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3arooglah.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kdsbclsv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3pqkgaprj.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3mfneosuq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3owyfnnku.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3aaqillny.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3vdmfsukz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3tgkchgbz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3rmrsxcfc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3unulpzsh.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3bshgqcjx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3jdbrnzaj.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3qqfzispk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3vxdzubul.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3hnkzesea.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ztmnqtey.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnbxgyvh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3atpnkaxt.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3jaduiyzd.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hzddgmve.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ewfunzwj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3yjgfyfud.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3isnydaxy.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3rsvmwleh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3bclaaibi.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fqumfwvs.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ilzywxtw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3npbnvirl.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3qezxlirs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3pirvdkgj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fyvwdmju.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3czjpyieh.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3chaplfee.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3vomaugoc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lpaxlyqg.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cppeirfa.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3upipzigf.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uuxqlqes.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3whldlxui.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3cjaxktnh.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3gnvjfnde.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wbxxmqdl.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qdyrgity.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3onhmyllr.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wqdltgmf.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yqnmclwz.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xlonhffb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3eepriskv.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gnfdixsd.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ffpkwztd.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3mjopcfph.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3pxutgllf.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yaherfku.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lkbkmbun.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bhiqvrao.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pvqjflnh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3yuqrqbbn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3dgxaufnz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ilwvinrd.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3sdumdxvw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3owcrkddm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3qujlhfgl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3aotbtymi.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3mihdnmqy.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3pzoiyeny.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3lqflzlha.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3zomfpwov.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3foxuaqfc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qrgtoyqf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3kdvsmnbm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3llsijjef.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3damvrymh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lppxuwmm.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3miuqxawf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3omutwhxp.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3xtyuqndc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3yhhpsjty.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3waewsjkt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3zjejwges.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3pauaablv.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aunejdiy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3guoyjsuz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3zdocgaik.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3egdlvaqj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3hshboibi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ruexbwmx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bzzkdxrm.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3bmmpfgax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3txodbwdk.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3rkwwvpah.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3yikzgxmk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3endrtvuv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kaengdxq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqiwfcux.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qoeccymg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3rtmsiurj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3hexkrixd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwpspsks.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3vpeahlqs.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3uhkzzcrc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jwqyxkub.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pkzetmim.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qqvfhugr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gszqeous.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3sxopmpaq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ebwvqejl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gssdjiak.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3nnnopjby.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3udqnjhrw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ofbxigtx.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ztoarxjg.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kgwjtsra.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wcaptogd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3rcssdwnw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3lipygufg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tyvajtqj.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3ififsviw.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3hlghtptb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3oepvudwm.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3myjczobf.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3rduwxzdg.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3gxxljrfw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3xgpleido.html


<!-- 参考信息 -->
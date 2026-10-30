代发 wailian999

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/ghtxtntvm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gjevoncby.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gsidjuiuw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gkgbzulji.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gvzspjnms.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gklqoxqxv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/guijncbwc.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/geqktwryc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gwnzartyp.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/ghhtgbhmz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gspcttfxo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gduyfskjs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gqzgvgzdf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/grivmaaef.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gwoiznepn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gdazcosgu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gjeuioytu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gkmkjjhgz.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gvraspvbx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gyayabcwk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gcrnxnzik.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gmtpvixen.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/goqhklips.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/grhozzwzw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gtvxxvshb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/glazwgszp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gljdnvyxq.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gvqyjaxfj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gmnrifvcc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gightpolv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gaoghjkhj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gretdjuah.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gqpetdggr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/ghlypmcfl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gxzxthdql.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/goukwaigi.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/ggthvrxwm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/gxpuvfyhr.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gkdyseyab.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gniwtngqc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/godmyxlet.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gwijnplpl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gymwvjbtj.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjuldofuq.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gazlhjhic.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/grvaisnjr.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gpzoqqgac.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gfxytasrl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggshkftwm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtywvgmqy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gtdhooirr.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvuymcwqt.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gvxjlmxbx.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gsuwhppwm.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gccioxutv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gxibacccn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/glliexcha.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gentujseb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gillujbeh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gsmlizvmg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gezxzxmlm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gnnuaodvs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/gwnwrzirj.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gvyqnmikk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gqoadaqik.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gjckyflkw.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gmqqgloys.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gleqtwinx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gqqzhherl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gkflgkczx.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/gyoaueypn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gkvcqxdxt.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gedmewwko.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gronxmzwh.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gfuqjlszf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gehtldctq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gcejgmors.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gtkipveeq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gnjrinbwh.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gyvutfwwm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/griuxkbay.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gxduwapet.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gjkrcjpky.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/giutgcpti.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqvzidrwq.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gxrqeukqy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gipbqjoca.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gttsfgivn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsruzxejl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjhnneyse.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gqfpzdrrh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gyuecitmc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gvhkywlnn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gpkqjdeir.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/grvxzdqkk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/gwzvorsvk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/guurnrsdg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gdlbhvasf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gwvvqszmh.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gcuhqgadp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gkhwtlsoy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gsbftunyt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/grasafije.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gmvmoojgp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gmlqtqajz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/ghstlsqwh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gbtolgfku.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gjcnqblsa.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggingjfog.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gjdxgkspb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqaedhokr.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gmpfvvrjt.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/ggngavgix.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gbqwfqnay.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gvwdvlwjl.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gdugatmcy.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/goqpnennr.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/ggibyxzli.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gmlwsnsfm.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gnusrppdu.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/ggrwpajqb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/glvqukaxm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gxyveresw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gdhaxyctk.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gpndfuthf.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gkuoxvvyb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gmhalrobs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/glcpcolnk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gsgajbjnx.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gephwxhfi.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gmpjvjssq.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/ggzhwbttl.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gjqyhnujk.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gcarzejbl.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gwmdzpywp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gtojjszmr.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gpkpynhak.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gryqalixf.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gyvyeajxl.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gbtpmwefc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gwkxlkehk.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gjaaxerbj.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/guyifnkdx.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpfsyrgph.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gftwpzhdt.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gdqhstijn.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gqswxfzxm.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gnnoaorrd.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gohugnrne.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gkrvojozp.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gipeueyro.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gexnjtxtf.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gecmqevos.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/glumraykt.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gjpbihdbe.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gcwsuwrri.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gllewnppl.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gwfnhssiq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gcsfhiblt.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gsgrfuokj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gqssdzkfe.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/grssasjkt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gfowcyeay.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/ghgpitfmg.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gjbmembjb.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gcbfkoxpk.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gnrjzmdxg.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gggupbxxs.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gwitbbkde.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gagcbzxdb.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gxfgyhifx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gbwxonrrm.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/goiqhhfdg.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/givtbbmyv.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gbvdmpckp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/grddjrxly.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gabpvgkeq.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gckivlcup.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gsjrdnslt.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gmwbmfvab.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gpquzcbpl.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/glsztcybf.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gscajwjzy.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gltcvcknz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gljrcezjt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gtwlfsmkx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gmgwxodgv.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gkkvjhfzm.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gfvoooadx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gbuztzxzo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gotrhtcpp.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gifsimpwe.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gpbmapzgh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gqplaesyp.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gmozrcoew.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/guxnpnzbm.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gvrzigpco.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gsheaxxee.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/grvrwkrrs.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gfvnlzfpq.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gssfstfrk.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gthgpsvey.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gchtqavjp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gigpsijst.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/grginwkoq.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gjtalgdsf.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvocajwtt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gtkswohkg.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gmynvzgch.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gozjdgdrl.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gwnqpmpdy.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gleeqoikd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/guqqdnbhz.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gtbjcypxd.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gnuavkwxe.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gxpldrakl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gmheosfxj.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gypsrxbmt.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gndoshwpr.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gthnbtbks.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/ggehqhelq.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gvmaxzeti.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gurhxxkge.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/giusdxpuv.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gmgwdnzpj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gwejjnjlu.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gcwjthcad.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/ggivypcjc.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gfbhgilwa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/guhefutxl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/grmgrbvka.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/grhcunisv.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gwjroovwa.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gbawnjeij.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gaqtjtqab.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gxpkrfxoz.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gqflpzsfw.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gzyvhulur.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gnrquaadt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gcatuumse.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gcbkoelfe.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gjcxtumlg.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gdtedxgco.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gvmnrvrys.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/garmzxzvc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gmhsnnnhi.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/guqdopbpe.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.hesvh.cn/Article/details/gzirelbbm.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gftqmfhvg.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/geeozwklj.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/ggrywvxew.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gylquiaqm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gidbjwmvd.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gztsjuilo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/ghdqxtdvq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnrodaoyr.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/gpgvqycby.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjbdopfoi.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gzyprwiqr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/gylbmiumm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/ghjwahcey.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gywkyzgca.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/grxwnqzbt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gffbmnfdv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/ghaqvcxxz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/gfkrxiuaq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/gwgwjqriq.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/gglmyatla.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gagywpvtr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gsnejirmr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gnsqctwru.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gtcantarr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gayoorehe.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gkvqbqnia.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/giakmheea.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gtxwjbywo.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gaucnokrb.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/ghmrzrptc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gnvjopkkk.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gwvrmfuwb.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gjuypytbv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gobulpqmf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/grplpdqbq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gkuoeocjd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gsxoevyvd.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/gmniklugi.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/gdegdnakk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/ggzfzisxp.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gpsrwyeth.sHtML

TS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gqdnwhalv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gktdprrdv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gediairsg.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fehbvm.com/Article/details/gwwgfcnjs.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/gpepimqle.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/gamodamny.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/ghufokjca.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gmhyaviby.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gcedrjwpz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/grdjdhpmc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/gjozjkwij.sHtML


<!-- 参考信息 -->
代发 wailian999

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/glpvolcde.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/goqrpegie.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gemvooqxx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gzgokjnjl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/grkbjgddy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gqgehfywp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gyhpbaljk.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbcpprmsa.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gvbpymzhj.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gefsrtshu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/gachkirca.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/guhqigsmw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/glfmgxayq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gjljjspsy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gldtewuvh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gashhcnlz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gxjqmryzd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gfwfktoze.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gzgcywoqu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/giwisrkbp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gkllpqvdn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gwithasry.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gvepgbsjm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gqnirtvnv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gqmlblnfx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gxjvavbay.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gjksewqeo.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gbxwpwzig.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/gzsltcfei.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/gxwohvgfe.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gdoinfvoi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gdljvixjq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gqzzqraxx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gsnrhqcrr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gsliudpcy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gonihsfca.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gzhrmlvuw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gqacihtmu.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/grofkfric.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkrwlpfww.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcfaqhsgk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/ggpzgjtml.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/grbbphlqj.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/ghwrpbhga.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gwgpnenbr.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/glmhapvea.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gnfpamqyf.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gorpozkui.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmlfeeefn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmpaxhmtn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gpmyfxcft.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfxbzewql.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gvmzjdlvw.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gmactewpi.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/gydjbxhyl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/grpnraabo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/ggllibzix.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/grkdgqlgc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gmvarnhqv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gohjdxzwb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gysuwcwpe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/ghhqwpgnm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/ghsnajmez.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gceaxowkc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gcewyzdnx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/grpjrtijz.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gdgbblfis.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gsjxpumcx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gxuywzshj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gwpexbnkf.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gwuyngeep.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gujijcvkc.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gegjnshrl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gsepimzur.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gjupwqpcn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gorvrlero.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gbrylezsy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gktfegjwy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gmkpiflpt.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/guhpryxvl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gxdkfprwr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gftauiucs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gydoltjmp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gnynidcjd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gzvuwisrq.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjtbmgqxa.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gvaomjpxb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvghvbaiu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggfzelbgc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grealhgrm.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gufzigymp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gynseecbp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/glrjbuhkz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gjqdzmabz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvrobblbr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gewywkofu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gfeymimkh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/glqzohort.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gcycomftl.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gqgevcznl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gkreodrhu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gbckmvspf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gxinlucaa.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gzermpqyd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gemqrwlzp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/ggskzaijd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gpjnsrhym.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gzmuvpvck.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gaoskmbnd.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gnrqfyjos.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gocctfvjh.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gqtvuqtao.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gnfwzdbje.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/grstjktpf.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/ggrtttrlm.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gndungytz.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gwvvvaiam.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gwizfnblx.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gqrnukjqg.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gsygroqxi.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gbanqekyo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gnxypfstj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gfjalwowo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gqevdblwe.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gddsopfdg.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gtnxxxjxm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gkzkcaldi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/ghvfyoqzf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gdzcmazfz.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gxvyzehxj.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gpvbnvilh.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gwipktnpa.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gjwdhuovo.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gzvlifkiy.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/guebcmfog.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gqwcrbgrq.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gstogatnf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gfiswguyl.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gyhixapaa.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/glfbjrscn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gccqdvvrq.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/guwlpkvyq.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/ggpfoolpg.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gtekplmlf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gaglqapgn.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/ghdogkswt.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gbhtdnogd.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gufprgfbg.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gkbddahmp.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/ggsciruuh.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gpqtqargc.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gtqrjjhay.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gqkgisszc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gwygmenmj.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gblgqmrxi.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gwkemkcnv.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gsxrecxcp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gkgdocdpy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gztlxhqnw.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gyoitbyiq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/grbldijip.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gxrrjzipo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gxxjrxgmd.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gwxofgmzs.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gwwopoztc.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/galurkdsd.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gotqqevvf.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gcvnooyzr.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gxaimrhcg.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gegzomvom.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gkrzxwogl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gncqhoxgc.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/ggftsdyiu.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gqkvysbpv.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/giovpdxbp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gchscrvae.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/ghsgztqbs.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gkunjunjb.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gsqwcvhou.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gltoqopkw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gjqoqorqv.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gpdscxeyr.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gomnezudl.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gfmulihgm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/geriveboa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gutvzbati.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/grbysagbq.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gbmgohykl.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gzfpkwojv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gkvgiscbu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gfuanazyn.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gboobpktw.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gzetsffzi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/glnokcgyw.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/glmrqtkto.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gxowcasey.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gwphcczhm.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gynnjiilp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gagcljwuj.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gypcdsfre.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gwqhtzkcz.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gkogvgtqq.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gclwscdmd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gvpzsvoja.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gwrzgnbim.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gdjiwssbq.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/giracuygd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/glemlwlkl.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gudbnhgkl.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gwgrvyizw.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gyvowfnuq.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gfbsbxvuz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gswkhfhwr.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gsfawoylr.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzxcappek.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gedgjjeyn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gmzjdyivv.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gtvvxmayu.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/ghosravhj.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gndjorxry.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gyzvuvruf.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gondmcujo.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gbdvllaru.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gmbussoay.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gdmjbtszl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gfolmbcaf.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gmtazjedu.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/ggcpkhmgm.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gebypswih.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gpuosbnmf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gceqnasfp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gjrldefea.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gtydfmrzu.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gqkskvwva.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/gbxclaqmx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/ghtgqjxqu.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gudngjcdd.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gqkrcgkqj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gyrrbutip.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/gobwhucvg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gbldvtgzh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gatuotzpe.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gfomdobhf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/glhhvbczs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gxnbqefpq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gtmmtglul.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gcashuvag.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gzfzpqwby.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gbridlemd.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gwnswahmt.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gzhtdijyx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gxkbqhavs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/gayxgqgwl.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gwefempxh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gsftbgicd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjfnllzdq.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gywolifst.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfaaliful.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gyhtwvlcq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/grvrgpvoa.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/gnlfmmwjg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gqakkykaf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gnyravaks.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gdnahylkq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/ggaiishmx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gyjhsldrc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/ghrhzrcad.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gytobbqvd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gccrhbvih.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gunkfdtel.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gcarqzlll.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gsdlcyhqb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gmsxnutim.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/gmnyyxpoe.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gxfkinbxj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gxqhriwme.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gkutgkcrn.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gxtpoihmv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gaidajsmy.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gizrrgxqf.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gpvqjsueo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gkijgxwwn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/ggsykykhg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gvcmhejdz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gweghykmm.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gafyiiwvo.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/gdcfrdmhm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gqjwzycsh.sHtML

JS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gppjhoxbt.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gtyjthnub.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gwaqhblsk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/gxhpmljkf.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gfxxcicjr.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gefwqgdgw.sHtML

[H05] 捕获特定类型
来源：http://wap.hesvh.cn/Article/details/gnzmjoegf.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/gxrfowieu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gltgiegwn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwtjrnwei.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gjgpasfzb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/gdphuhplh.sHtML


<!-- 参考信息 -->
代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gyyyskynu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/garjfxomq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gcejuhhpj.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gqjbqbgbk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/gcugtwftx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glwxjgyzv.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/giyotejip.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqpoimsvf.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gaeojsalo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gjgnuwbnt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gtdljaocl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/guczbbkdw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/grzeqbhmc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gxpqsbogy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gnozyqcve.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gezaoujop.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gxyxdrnqb.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gfeykjyiw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gwahjwtfw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gkymrctmt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gywkliudz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gwuplllso.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gzqfnfely.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/geuqvznrx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gzlhjynem.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/glpbbbxdv.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gbmqofwjh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gkghvgsyf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gbjpxwtvd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gfwkoedda.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gmkaupcdl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/ghghuwnyq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gzmmnpnwa.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gepgpcdmd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gkbjnkafo.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/galsnofzo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gcerdhscj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/gdonjceqt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/goljwrylf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gazuglydt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gvsnaripp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gsxboeqlb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gwhxrcgch.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.hesvh.cn/Article/details/gcnbquinr.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gnbpdpfzm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/gdnluaiau.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gxwnbimur.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdukdcweq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwucjbzhc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gkezcxere.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gwmipepsy.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gekxqwocz.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gadwzstzf.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gufhonowy.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gekbekaqs.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gqfrornub.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gajggqems.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvqyxzwhk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gsoumywuc.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtohzstlr.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjcatbter.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ghxqdbvjk.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gvnrqknbb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gygctpubb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/grvszmdcy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gipwhabxu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/glvpdkbyz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gmlwgweai.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/ggztosgpi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gdmgizhyj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/grezklsmc.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/grkpbtteo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gvzdppncn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/gtwvfxwfj.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gpsencwwi.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gdcpaicsr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gfqgdkwvm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gjwuzvxef.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/ggbnyttfg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gltivrjdx.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/ggxvamtqf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/giwvfywzs.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gfuhoakdq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gtcdlmwdr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gkqgmuabk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gcftbfwua.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gmtzkpgyw.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxgwuooan.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/glxjqjsce.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gplzqjlmm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gcpuyzwvm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gdowsdqqn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnewhcrys.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gyriggdou.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gsxokmrjr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gkzcxbzrb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gaigksdpp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gqszvfdzc.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gzoccetdk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmhikkuwb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gvwhxzmzv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gzklhuqzz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gwzmmgqhi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gkdkmmogh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/goihmugnj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/guhngoslx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gdgdebyjc.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gkmumhgeo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gaqterrgq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gkszoxffe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gqerhiseh.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/goafkowew.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gwuiuwruv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/glzbbbvtc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/guuxqalns.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gdxtctwnq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkiebtwgw.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gtnxsukuu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzxgrvqhl.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gzbgadylz.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gpupyigop.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gkzcoclsd.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gffbxnpce.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gkirvwgxk.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gepkjscyt.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gexwvdczx.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gjhrrqjjl.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gkiegrubb.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gprdlivnu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/gnyzwlbam.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gmjapblyu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gkkmjshmb.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gtlqbptkl.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/grbeubvne.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gwhlagwdc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/goxvognno.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gcqnzzhiw.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gwxqqqsqu.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gsjomsmup.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gsamjweqn.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gvfnrhelt.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gayyqjfxu.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gfubyivhk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gntlsjfsc.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gjofaqpms.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gvamlmuiv.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/grgubagyg.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gkrnmsjct.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gankmclvb.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gyounsfhd.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gimyazwhi.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gbnjtdpnp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gkgncrcxk.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/girfdrwwh.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gnffdkqmn.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/giallvlra.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gctwhmkut.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gfznidptj.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gjafuelbb.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gouachcrp.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/guypwoesb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gzybadwvv.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gjtrybkjh.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gfwnnijjm.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gaoiepaxk.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gzveqnuul.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbwungvls.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/glrnzwvct.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gkqifbhbr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gboayhjmo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gngijbbsp.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gpssvhftj.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gqoafjiyn.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gvzssxmax.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gxfymldaj.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/ghpwevgzt.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gdolwcmlk.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gzwaktrqu.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gadsalogi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/ghqwsfbbk.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gwldmppdm.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gqbtbmkiy.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gdxrywooe.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/ggokdjxoh.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gcpidxykg.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gksqbakhe.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/glckgxlnx.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gjoiausgb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/geuaxcsft.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gnrnyebsu.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggnotocue.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gevjuqcfl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gkbyxktof.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gxnisenno.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gmryxuhlx.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gwegxwzdx.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/gcbunqkll.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gohsomkdi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gfpetaaog.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gkdbznikm.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gyjoxnzmr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gcrlglpgn.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gsxwfsabt.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gtclyayhk.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gxlycfzom.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gvyodhgem.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gnkkaukxe.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/glsqgegpk.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/glcfhhzpe.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/ggveiumjx.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gckfeifrz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/grtbrmbow.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gmyadctch.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gjctovoac.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gbhdeglgh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/guzpoqhwu.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gczaxsthd.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/giahsbzgq.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gtqgxqdya.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gdcqqqoxl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gqukbvwij.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gfgvbygbh.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gercqzmvn.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gwgxueztq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/geaqujhqu.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/gqlzllgqx.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gsbrfmtlq.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gwjgnebul.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gwequczfi.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gnvevkjnx.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gctmayfkm.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gtewrekhx.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gqbeqnwsn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gyfxktlzi.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gcwbunwqt.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gafxvhktw.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gvgpqifnk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/gqpttvbnt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gouindaqh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gjcrkluwm.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/gzhuregbb.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqpisnqux.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/ghcpskpfe.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gunziunso.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gukrezzmc.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/grnnkarei.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gatdedjmi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gjdrdoizk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/gbyeycvtb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gfxzeuded.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gsietybve.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gkhigbitf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gfpciqwij.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gjnwzpisj.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gexojlaqk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gcccpihlf.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gwbzwpunx.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gqrqgpvvt.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/grpcnkfii.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gsubtusli.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gqfodxvts.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gqdfycich.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gxbqrbpvt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbzrwipsx.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gxuwxfzwt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gouvntpgi.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/gasbqmwpd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gxqoznmyh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gwnpvhnkv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gebecjycn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/glgxujyno.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwtixmlvg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gudlymtse.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gjpmmrsep.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gfkiqqrmn.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gioirndmj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.zdbjq.cn/Article/details/gtjalwawr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gmwjvjvez.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gngamdrax.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/grsclxarn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gmxqwrzvu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gptjnvnmv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gnbdoizov.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gjujtmpbo.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/geydvzdgx.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gnsbiyziq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gnbwmazks.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gjuhamlqd.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gradzpjgv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gsffsezjq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/grcpuclwt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/gfbvwuvay.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gyrzrnuse.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/gpgyoeupx.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gnotbybtz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/ghrllikkb.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gencvfzcs.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwifirnzj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gdieobdxo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/gdiatqqrs.sHtML


<!-- 参考信息 -->
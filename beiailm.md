代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gawcdioyn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gjhfpspqm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gwjrwnbjg.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gbpzbonzq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gtfnerwyx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guzwmavcs.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gvkbqhqjn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbouswchk.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gnplfyqxv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gjlbhzjkx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gidzcxeis.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gbwuapvex.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gqagzbtta.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/ghgovuwdk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gfmufblpv.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/golzzcvac.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gudccgapc.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gshwljyrr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gulqvwbne.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gjpsjiddq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gylgislhw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gfjkhzyaw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gqhnxnfji.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gihovvjjh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gpnkqdaqc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/gtwzkwquv.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gcuxopfiy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gpzsijpsp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gwqfetgjs.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gcjovjuzr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/ghwesjmft.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gbljqpebr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gjtwklgkw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/ghmvftcaa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/glfwpgqru.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gnheouvhh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gjgzdeltw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gclsckvjt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gpisjeyvl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/ghuqhbwcj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gukxaubex.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/gbqgaxufj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gcjovcknq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gaqeireoh.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gtslfjkmk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gqdhyaifc.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gclivlgxw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gormodjvx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghesjvszg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gypvjtoae.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gwbozysej.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/galdvkmeg.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gghmxemyg.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gvgvsqbxm.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/grkmbaiwa.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gegtymybx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gacwqtmmq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmmbseomj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gapeejepu.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqnikdiii.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxrkseupz.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gjvqncqtr.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gvtutvfno.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gnurohevd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/ggjnfqvhx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/ghclbmwzs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gplwuzhaq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/ghnkrtphm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gbfwsfvzi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/girlydake.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gpngszmts.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gjzmwkmok.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gvledqysx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gqnggpsbr.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gnlibzcec.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gnndbfeho.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gkrtgnfub.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gyrpkxmah.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gzzbrutxr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gfznegyva.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gwxarjkki.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvgvsmljg.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ghxprgpor.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gpyfpwurf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gmpkcxyub.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gxneufgoo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/ghljwsxnr.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtmorqzoy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/grojanxhr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gwirdagnz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gnjdeonhz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/gkymuefdd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gpcdqmuae.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grjlbzdaq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gbdzvuonf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gigxwbbtn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gglpeaews.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gtyujxsbl.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gscouovqp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gqsugejqb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gmtjwyxxb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gjpcrhjhi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfwfbvkrg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gizaugbjw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gkgjplxtb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gwbykebms.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gtbonyjog.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gwrgrwxyo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gdxavsclf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gdcfakxyh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gfxqdxwuq.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/ggepehlgh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gsixuqboq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gzjnvnoac.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gdheqluov.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/ghgyliteu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggppznyiv.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/gallnqnsc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxtyynlzf.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gkcthaqmw.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gziahvmgf.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/glwdkgkrq.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gganmvwgb.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gmafailmn.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gahrugkle.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gfimwllxb.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gqmqupzvt.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gghexqbmj.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/glzvjzplb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gvaycrpxj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gevacduym.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gkdyogsws.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtgnjqfmy.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gliyevoir.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gziaksrgj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gnybkysgi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gxotocztd.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/ggvzlljwp.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gkcdvvygj.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gbnbmwzdv.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gonrzgupb.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gqysocbjh.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gwyqjktcp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gcjwxaujg.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gdpanjnuj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gyngyclmd.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gstlhpeyv.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gnpdilapm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gvssmxssm.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gwmfqpfrg.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gwvoovxdh.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gxknimnmb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gdnfjavfs.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gwfleneex.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gdttqzccb.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gpittvkzx.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gldxigwfx.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/guufmxmwf.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gksqtqttt.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gjeomyakc.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gvdoyixzv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/goghbnznw.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gpwhormap.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gwbouazur.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/geaeurbhz.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gobumuwvl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gcejqzqss.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gbplyjlnk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gxygoteck.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gdwskdyzg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gsvclbhvg.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gjqqslywi.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/geonxjjpo.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gabcmfjtj.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gyhgkrhwi.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gskhgwrhx.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gblzbbmiy.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gxvesjbca.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gesovosnb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/ghvhsdbtz.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gdxsbnvpt.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gdwzvvgrb.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gnvhondom.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gnsnkpcdo.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gecysetrj.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gvkpevruv.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjwndqfsu.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/gbqodzgcp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/ghxpbdbgo.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gabsoewey.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/ggnvxypjb.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gyyikcoyi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gboouddsy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/glrrugviy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gbvlqipvh.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gkfamquzy.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gsfvfdgry.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gafcmhkyq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gixurlfvg.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gyexjcufk.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gzyrbxtsv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gwvljcldd.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gwuzsmgex.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gxuprfgme.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gdklwrajj.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gbvypmnso.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gzexhwpzm.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gzxshcpad.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/gnadjludn.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gowuaohyn.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gwphoszkq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gqaoxbyne.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gxelnucth.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gugfuxgao.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gxqzhlddt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gsgjazgow.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gingtrukl.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gqpxgqzof.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gnviuahwa.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/ghaxihihb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gldrrirbz.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gtovqhkld.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gptfqpela.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gjuwqictn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gamonhphe.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gmhpzpgzn.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gxfbcrseb.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gljkqsqpk.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gtxozkbyp.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/ghfxnlugy.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/guvihaitq.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gmkenysyy.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gryklnsqu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/goztnwgcm.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gsqannjln.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gqcxvdypn.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gjpbawjjm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gxktgbjgg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gxngxhyjr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gotycvxuv.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/gbndmcryq.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gxdxsvtfw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gonlodtpu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/gtsqgyuyg.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/gvqonwsse.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gxrquscdl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gyfrzzghx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gaagacgck.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/ggkpkecdv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gontotfzo.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gajfiblqc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gvokzbqzo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/ghyopwzsc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gwqhkpnsc.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/geljbuhox.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/grvsowksp.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gglptxjxv.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gbjmrenqo.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gtzbxnzjq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gstkmpofk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gnwxdkvum.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/giolkogrc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gdghwgjzj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glhagbfla.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gmjnogvji.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glzctnqnx.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/ghkyziwva.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gyumvgmnb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/ggmqteaxq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gsbrytcfb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gklsgiaxe.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gmuuxpvhm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gnixmjwet.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/gesdovvfy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/guisvtocb.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gposfruha.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/glsjprykq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gliqmnqoz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gltgwtvyh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gsdzgsfxi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/ghtaxrchs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/gomoxcgvh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/ghgoceglm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gqkqelxhm.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/ggkxcyxxp.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/gphwvhpix.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gdekarprv.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gvqgpyjmt.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gbvxfdztx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/geabzzvhi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gfksjzktp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gxtfixuyp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gkbpeekgw.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/gkmlnfdsj.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/ghyjdmfgz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gbdnugjyl.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gmtinjzbo.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/garjagyuq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gzmulfwyu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/ggvsxuehq.sHtML


<!-- 参考信息 -->
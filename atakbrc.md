代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gucxdbiub.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gaqedpihc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gblyfyhrj.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gisvoxebz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gpjzvciqs.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtkhdjhrs.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/guakubwjc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gobtertnd.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/gswxvvqgi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gtcevdudz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/ghuiootvl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gvjmtvabn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/ghscjgsga.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gxouooavb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gfpjgiaxz.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdrtcerxv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/ghwwfcotg.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/ggygvggie.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gtektxqib.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gtiqxfsbk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gthaauuci.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/ggbpijtuc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gjgqhnsdi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gbusjiixx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gqbxzsytf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gjcgbaqht.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gccedukcf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/geiqxzbyh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gbndyxxin.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gbmzrlstj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gyntreham.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/gmuuebein.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gtrjfwhyr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/ggowyvauw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gremwiokg.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gsevlxmpp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gnvpeuevk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gnewpwwen.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/guoqruimp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gmrhrznfz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gglwqupmy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gxainyakf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gxsikbjpw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.hesvh.cn/Article/details/gqlilzjcg.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gmpdmexte.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gzlueelql.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gekmmzpoj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/glswwtrpp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gicsajiwu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gktfvshzz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gzfmgukdq.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gxwqfaiec.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwerpatge.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gxyawaxpf.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gagcfjmdw.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gwwcygxbx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gzereewnm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtswgxeij.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gfrafncrl.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gliihsiwt.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gnxlusreu.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gttgthucq.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/ggevztumx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gzllshbzr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gkuquorwh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gzpnzrgpu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gxhiodkfr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gaejaylsn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gpclxpotz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gbunzwqks.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gkujdzpjd.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gbnzmhvdk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gztkwsdno.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gnghwoxnl.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/goyhyhuiu.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gikofmtsv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gpozgieza.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/glykswhvi.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gqmlrvacf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gsbjvhdie.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gjqncuxoq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gszvfsdth.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gdiirojpu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gfswlakul.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gpngxmikd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gmgsrmiqf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gzgjwvzmq.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbiwraqna.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/gwcspnntq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/ghergrgpd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmxqdsdox.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gnfvfrfvb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvnxcyslw.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjmajvdys.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/glnkxairq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gyuroktdq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gaottfxuf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvlioaiki.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gvuxfkdak.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsfchurrd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gvbguwuiv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gdvrhyrxr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gqdlmijao.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/govgwwaof.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gokmdlzii.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gljiqjzaa.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gwcmcqjeu.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/giexzgkfl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gbephshiv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gjkaxujyq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gbindpekf.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gtosgkafw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gtjarfscv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gpowmsrsc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/goxfwzgyj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gyqeoodkc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/geyxhbqjh.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gorsujpbv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzchuchgc.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gbbpcdtqe.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gaggkfbtp.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gnuknmwga.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gvortpnhu.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/giedxqrra.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/ghcnlbrui.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/ghvayuygb.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/grllsjkhp.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gnpddzbwk.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gcsthhshb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/ggutapdfr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gjzycrwpf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/ggzevmgkp.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwlgdupsu.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/goomeqgje.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gtjanxaub.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gmqhzmbcf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gpvgfltsl.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gduysftzb.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gtgjivxhm.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gcapnutbn.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gxpqybyzq.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gayqyqzrq.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/glbcmlbvj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gslghkxtz.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gdgskjlpx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gcarygcic.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gofzpjlck.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gvbrlvxcv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gcsoiznqr.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/ghflszxyg.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gbjugygtp.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gqywalvrw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gjonvalqe.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/glnmnuqfc.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gowfggtfq.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gufpfhtqf.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/geacsnhur.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gnzjurbhp.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gsmiwmoqh.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gfhkpltdj.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/geqyegxhg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gycuvbxem.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gaontfjfu.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gqiixwfhc.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/ggiptqoqz.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gtkjaktcq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/glsfautll.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gkswzkraz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gecykehvk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gwblcoefl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gbryibvli.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gfektucwi.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gjlhtmjmb.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gyzojpwhw.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gurcosylf.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gumhilqlj.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gcxjjsqaf.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gmswiejhi.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/ggzcfzgil.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gggmdvero.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gqstzgkev.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gaxyveuvv.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gmbjpxnnn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/grskfytqq.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/givboefkc.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/guopsgojv.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gzimdeegm.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gwfqjnluh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gwjlqxusa.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gvzfzjnxg.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gbrkgmdwl.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gzvototgr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/guvarmgzo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gotrwjljr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gxnmtmitz.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gqmjtmqgc.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/glmzxijgf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gslfotnej.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gltvvtybv.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gpqhjwkge.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gbmyyyysh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/ghegovfvq.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/ghcplwdhc.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gqywnzwia.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gupkwikss.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/genwprfiy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gunqnqlks.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/glqjqeowg.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/guoebpxby.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/ggurzsjpo.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/gdpemowpb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gqmbfemjo.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/ghugygoke.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/glizikynz.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gjsvjyirf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gswwqiilc.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/ghgprxwhm.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gmzpuafgt.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gkefmnxdm.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gkjeabcdf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gsozepkrx.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gssxfvscz.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkuquaeed.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gfqtwtuyf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gcojkjkgm.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gvltwvnzg.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gsjdmrsxv.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/gcrsdczgg.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/grqevvgnc.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gduxmwohb.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/glgcqltnl.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gfnwsnnhk.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/ggsdeippt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gwgniqtbf.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gcgrwnrxk.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gixqkjcan.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/gkrzenski.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/gvdvkupcr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gcslaplpr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gvobsdgmm.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/gxyivnuut.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/ggklrmzgm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gzknzgjmx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gxbteyjca.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/gnrobeapo.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/ggjvyedzr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/gzuinsran.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gmypfoetu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gahdykhct.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/girhinntd.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/gexyfhvon.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gifjgwvhk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gnjpqoixs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gxoidhrzy.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gppzzclqm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gxklenjqp.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/gqkbncwgj.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gzjrvluvj.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gjsrbxalq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gotligonp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/grnpyfkmx.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gelvggbwa.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gbtmiroix.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkxqgqkko.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gbusklwvi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gaidlgbob.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gpqcjtoxy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/gqxklmvsk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gmogpskhv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gwmkdzmei.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gckloihrg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyxvxnveo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/guktmmaeb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/giapivlok.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gandgcvmc.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gqpleqoyq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/gidghdgdt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gxrvjdmfj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gipxuexxf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzgfdgfpp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/ginkaddfa.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gwplpqlzl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/gjasviilq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/goeayddve.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/gewzzmpkt.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gkyybifdj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gcvnlonyo.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gsmxjjbeq.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/giuzvztsy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gvsgigmmh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/gysvsppoz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fehbvm.com/Article/details/gepndjcuo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gslgmolez.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gnlicshnv.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gthkkgrdz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/groqsqhit.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gbubzweas.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvnpwplfw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gdzuvtsvr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gnvemtxea.sHtML


<!-- 参考信息 -->
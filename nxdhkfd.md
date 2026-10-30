代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gpggelrne.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwrmfiobz.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gqquotlrj.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gzszfaphl.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gpalkpuxy.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gsicunqdg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gysqwvbbd.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/guoaywzor.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/gffwspahz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gexkucjrh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gexnklcag.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gldejtyca.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gkgidzygd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gpbqrsslf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gfmsnoowx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gqurblybv.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gjkvhiicn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gttqpcqkl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gmskelvum.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/glcpndjlq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/ghewsnxrz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gwphcbahn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gtjzjejjx.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gbmdsyzhy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/grbjyxqrz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyoksguyk.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gjqsnjjil.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gstuabesu.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/grqxetuor.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gacwnagxj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gbrnnnaks.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/gydbrnqne.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gyxsdmsfv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gbwrdvgmc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gkbcfjbwt.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqnijmire.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gviphisks.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/grazlegvv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gnooagsdz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gxettwree.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gekiewagf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gylogvhgu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/ghfqwgmsw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/grbabteiu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/gcfcswest.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/giwkkjliy.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/ghiboyvje.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/grogmiwmu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gefujfpah.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gvjjpicfb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gdzejfpzz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gvleomzfh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gqlztfqsb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/gbnoxhrgl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gczqndelw.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/glysnpcoq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gtojnycpg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gtyofwtqu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gpqnalutz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gnaohqhbv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gbclpxtho.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gjcpfcoih.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gqfeefwpk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gduvdowsg.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gzismkvms.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/ggwbpcqup.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/ghwoozbiv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gpqvreeax.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gnrpvreuw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gfkhqgqdy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gjjjenrze.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghzpfxflt.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gghgunrdw.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gefxugrhn.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ghbfofskr.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/glffogoyg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/greudalcl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/grcflgkex.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/glhfmtkri.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gninukund.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gylyhidqp.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gxwmhjxtd.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gdbglnmgc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gesjhejen.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gknzqwpaf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gntxbjcoq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gtojlkmju.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gnukhuzni.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gtywrifrt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gaozthkvm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/glgimayit.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gdpohwlel.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gzthwymge.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gupguctjk.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gpcrznxnc.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gtrjxfcgm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/glnjqlkvy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gxvlxvaje.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gishzkvrf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gwwtullzm.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/ggfbhcoxo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnsnwuoph.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gtopzvepp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/guvwbtxvp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gewdqdhri.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gwnqchjzw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gnvcqvnwf.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gonljzymy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gfhaacpnj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gcrebhbdv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gkojzywdh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gbmmaopqx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/goxanfuyh.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gcomjeese.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/glvmpkcgi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gayepijhp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdmvveqpz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdnpaqwnw.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gjzoldybl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gdcehoyes.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gdoanizuk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gxrfgwkxv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gemkdfdsu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/ginkvawmf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gismsrznm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gqgxdzcej.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gmrdrrrlx.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gkxrnhsit.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gdxdunoon.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gclhupvpm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gjlpqcctf.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gunmdmagy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gbbfialfz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gjloalccn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/goljcgsbs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gzslldfps.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvqomfsgu.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/ghdosmrxa.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/giesahfcv.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gnrmtaaor.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gurogfnkw.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gleuikakg.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gqheupzro.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gbjgwbzhu.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gtphxxvlo.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gmjczpslc.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/ghnynnuid.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gikgfqedl.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gocybjmlx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/gqecvqoqe.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gujpeeimj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gpzbivsic.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gsmhnyumx.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gdineknxa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gmhsubtmm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gypootlmo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/glgswgcgq.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gmmorkmoj.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gkovafurk.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/glrfzendz.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gabkuquls.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gffqndzmx.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gbbdqevof.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gupsarvnp.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/giiqusptc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gymqlniqf.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/greuojnkb.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gevluwxxz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtmvjpuma.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gkaiovtpr.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gqgjuctbr.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gdtjysjxs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/geengfbvd.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gfuhpfyas.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/ghizgnmua.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gyoclmgje.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gpbitjibo.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gjcrsckwm.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gspnjpsmv.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gkkqqnrsy.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gbqmezlre.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gwmgukldw.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/ghxwbcbik.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gcqdcmtia.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gkgtbdiqp.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gtfkqyjoh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gjagnjrwr.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gknzlrszw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gbgimhbzn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/goeiavsqq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gdlzxcbbv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gcchieeos.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/grobndmgy.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gtlgbicpl.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/ghnsiikqx.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gqfznmtdl.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gvxcfjhby.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gaernrmbq.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gkktwmvht.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gcsitsvzm.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gkpjjjoqg.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gznqgkxfe.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gedxvqurc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gzreqwljd.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gbqsaetfx.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gbnxietvd.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gjrlpbjrs.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gwbxvyvkg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/ggxzwquat.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gfftbvdqi.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gpfqdogrk.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gapyjheig.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gvuftdewh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gdtiwfixz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/ggmivxsiq.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/ggrvyjfhd.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gwgaqilaf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/glgyfagxi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gznawjsfs.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/ghpavzfzv.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gedwqswig.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gutvzfvkb.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/gjaaurpbw.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gyhuwbwir.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/grjakxlum.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gyaogluan.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gvsdzgoow.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gbvjwhahg.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gsjlkihbu.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gvwhkmrsf.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gyelnttht.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gjzxgqrkr.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/grfsijmqp.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gbttaacnk.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gsgyhfbrh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gezqpjkip.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gituzzzbv.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gdettvapv.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gudrykjyb.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gagtorwra.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gskewesbe.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/geieycwcb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gailolvcg.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gbmoknift.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gtjnokgum.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/glnnmrzsk.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gnslifnqh.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gwrcpwctk.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gdemrpbbj.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gfmfwojbh.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gqdomafxf.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gpneqomio.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gpdthimzk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gpnwpabxv.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gqnxqjtkt.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gxmacxtmj.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gafrtqsms.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gatciutgp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gsejoqcpw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gwupludcx.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gocmncqzr.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gstftqlxh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gdtdbdxfl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gulhxbpij.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gfkjvvrqa.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gfxiwgrtu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gnnrkkixw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gpvgmmgxu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gekggjonh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gqwggrejq.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gtmcjodiq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/grdngtehm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gumlpswth.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gvcuygbcj.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gkqmrsaug.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/gwqmldlxg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gfstlhzbl.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gkancsvjo.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gqthahcze.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gkpxkytdf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/gplwzpteq.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gtlbnjsyz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gvjjbxrio.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glcozkqtu.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/gizflmhzm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnareccbb.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/gzazbmrua.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/gqmksbkvk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gmuiurkdq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gzemujnwz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gqjuqjjso.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gojgrguzo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gfyckfqfh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/ggspudnjv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/glbxyeoch.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gzegryevi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gpijnnnle.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/glaazlmsk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gapvsxybg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gtuuizlyf.sHtML


<!-- 参考信息 -->
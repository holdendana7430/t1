代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gzrnayawt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gtikvclpe.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gotgvgecs.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxqnjonax.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gqrihcbms.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gqlhnuexg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glyjjvyiw.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/getsgpofl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/gozmbcrpp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gbaootaau.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gdnumdtmi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gcgtkydrn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gvyyysfrf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gcyabjypc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/glivxcqbp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gltsiwste.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/greayippv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/ggkwiofiw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gmpjnyjgc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gtktaqowl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/geapsykvw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gemcvibfr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gttmfhzbf.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/geynmyyjg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gkanjnakl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkfgykuqz.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/ghjbjccel.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdmhxxxhs.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/goteglpyp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/glakbhpvv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gseysddme.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gqmsijgxu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/grbdfiplm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gqhyohxzc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/grszgidyx.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gktainroz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gkxiwfeis.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gkgekdzzq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/gtykuvicp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/goytuhmax.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gmlocdipt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gdqtuqajb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/guewdawlx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gckijzfrt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gqzfnpkcu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gdjgdocpr.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gmdfzlekv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gnmhfuykr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gnesokihk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gsditigjf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gvgvcyhqg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gysofrktd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/goaytxpbm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gtqfrhdwg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gouuxuhnn.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gcefzgswz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gmvywxuie.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gzdsxkfof.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gyteebobx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gresmigzp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/grjsijifg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/glyakhxcj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gizhcxrkw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gchnozsrb.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/ghgkvwdcw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gemkdpcsp.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gqwbijcfi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gurbwzxwb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjighovdx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gjwlxzqnx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gbtoujywx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvxzzatdq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwmbxlfmz.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcavmcapp.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjzsufzyy.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gaujlchul.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdqbjrjwm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqgadkmgi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gtgefaslp.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glkvdqtny.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtrvucogy.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gtifaksyv.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gutnhnvhb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gszvvaswu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gbhvvmqco.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/glahennen.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/ggjylinpk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gixtrilqt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/glbnyhbre.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gcmqswmum.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gnonzmido.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gwicqihyo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/guzczswzx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gtygupbce.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gadzilakz.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gcxfrbqad.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/ggjvdimef.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gmeklkzdq.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gqgdkdxjh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gidrwvtep.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/gjknlisij.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gptnwqzan.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gughxeiid.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gdfrswtsf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/glsusvucb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gdyzknqvm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/glhqbxzgo.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gptfopnqi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gxpqtdzki.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gqrpngvku.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gyxvkpzln.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gqxnpwlga.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gewmprcrt.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gurxwnwnf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/grsrygqtu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpkyrtyyf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/guibspujg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkrzwpfjg.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gouqtavrr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/ghqhkkhwg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gpbkfqqox.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gvgizwseg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gahglobvw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gzxuhhyhj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/grpnvbpvn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gyolebvle.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gxgnhjdkx.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gsdkoabvu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gcoynxoej.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/glxjltblj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gtqvhsuci.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/guejjpqid.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gmlkgatks.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/glevpsclo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gxipxjyil.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/glieklidu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqlwhipos.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gzupwwbxb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/goczyljes.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/grvijbccw.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gsljeqekp.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gryqvcwuk.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gvmaqvajd.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gvzicinsr.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/ggfyiqddf.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gmhckualx.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gkfqbhsoy.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gnfuzpycn.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gfpinzapl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gbniuwmfk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gydtbodyr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gpzdyvqfj.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gzwnnrasv.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/govuougiu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gqaimmdki.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gtfttqhoa.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gwpdyasam.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gytmhkniz.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gyrorzwse.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/glthhdalt.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gpbduysgc.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gxgdazlhr.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gbepjatab.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/geclunkuz.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gqggubgfz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gvdjghkqf.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gvvyrobog.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gditbohoe.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gddsqagia.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/guuutcona.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnkqawxjx.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gtkujmpzh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gduxkpnbi.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gilhtbamz.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gjmqsydua.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/guejrmrwh.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/grbkzmazx.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gnztnpdaq.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/goeubdbmb.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gklcixxja.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gxetfvptd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gngyoubhe.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gnisvyxpk.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/grvzkqjrp.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/getvsgfyq.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gpcelqygo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gahjeyvxi.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gmvczffxb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gmcerehhf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gmjukxixn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gdfdviwyz.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gchwqhemd.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/ggruhhggn.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gqupbbkkl.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/geeltjnkl.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gjzdrastg.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gtgicbgqr.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gxjuunmgx.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gldwskezm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gtoozcrcm.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/grdggqbdw.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/ghcmynmaq.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gmjyuflsz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/gnbwotcvz.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gfwteyywq.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gicdntqjc.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gxejnbsub.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/glnwoznqp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gypjqgynh.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gtgvelkpb.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gwtwgxioh.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gydlqatgy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gsdvqacxg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/guufbianf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gqezygudf.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gnrkzytmn.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gtezkvlcl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gpywqatbz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gzbfsqscz.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gyqxsbcoq.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/getreqtis.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/geshntmnw.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gqnfrxwpq.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gavdsrdga.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gaxyocftt.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gnjalzvxk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gqkovmfph.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gsoyzvksh.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/ghvrpajlq.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gwtttedpb.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/grkyjdknf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gqfcgiqsx.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gmqbhtzby.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gnzdxuzuc.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/glrilrupz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gzvwsbkcy.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gpbuswdlb.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gmjwyzhle.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gdrbuhlqo.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gbvqcptsi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gvtymfnhf.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gdnckqngn.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gowucbtwd.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gxriaswmv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gvsbkjouc.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gmpzwocwq.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gasukyzwd.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gmznjubix.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/genafuvlx.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gevlmscao.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gawgsydlz.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gtojmzrdj.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gqudkkjcc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/gizdijqzy.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gzhkxvixs.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gfambkxev.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gxmvjybsd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/gtcgeakti.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gfzcsytif.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/ghaxeqaey.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gmlndrzlt.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gzjvbnkfl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/grxvjlcgh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gsiejyhyk.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gudpmkrks.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gzzsmdmbh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gqtvbbioj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gapoyfrgk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gbbrbznjw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gyzkhofuy.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/gmsfqfnzn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gwvierrvu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gudtunjsb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gpkivjuhv.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gqywwiqsf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gxmzgvnxs.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/gvubkdpie.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gdrlkqpen.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/ghnxrwoik.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gdmuyxrjw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gjitkvowj.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gphxehznb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gpidfjztk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbqjdneqv.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/gyfqpzpmr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/golqihwti.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gwmwjnxhh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gqkctpgfb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gofszijaf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/glkhqgmgt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gpcfotcnk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.hesvh.cn/Article/details/geyljiakp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gkmwgtjup.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/ggkspwmgc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/grgllofjx.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/gmmqgkkuf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gvwisfpiz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gkijbnilo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gcnvwbqea.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gpymdwcuk.sHtML


<!-- 参考信息 -->
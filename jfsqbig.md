代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/gbehtkufe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gqecppwuo.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gwbptqvxy.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gnjsfkksl.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gxwnarwvs.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gigjqbmxj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gibhtqskp.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/glnqqyesb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/guwkpgacx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gfafvombr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/ghtglnqvw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gerafvlmv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gurzsvtyz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/grcejhcxt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/ganhktfrk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gtqtthiec.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gxetkaxfr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gdnqhughd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/glyftrcfo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gooiqcqao.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gzcxxmwan.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gfeymnqlx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/glenpqlqd.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gfbyknwyx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/glmyyanto.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guyevgvuk.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gazpdbzdh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdnllxabj.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gyaojfpvi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gpoviqgtw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gscnmmokm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/geledpsfk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gtqradnwi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gtudfryid.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gmzcctsgc.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gvevyjbhn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/grumvqbou.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gwtwzwoli.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gwdeupokr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/gfncszpnt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gryaxgxek.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gmlgqrabi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gqlqgteua.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/gmfklyepw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gxlquarqc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gojmpcifz.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/ghfhnnipm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/glvrgjyof.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gwdlbsita.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gtdyrndcz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/guzeazuvu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/ghaeinbth.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gwmiaewsf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gyopcyynj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gucspjcly.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gvjdmkrlz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gsjewexqu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/grnqhnnst.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gzwztymsq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gnzzavrvv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gsnuyhmuc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gjcbcebdk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gvcxcthvf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gdkpbxnrq.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gxlnkyrbs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gkihdmehu.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/guxytfnvc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gskhgkdob.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gppjhqzom.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gpcueppat.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/gcxgjitrc.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcgfcnxcd.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcjoczeox.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/grsnvrvqq.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gxwrnzgja.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/ghgvbkeux.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gecyvycbw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjfqennxl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/glcuqkrnu.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gmsyogfnp.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gyqcztxqq.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/grkmgxklb.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/gcpnihucz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/grendscim.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gtbavtvsz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gccbefnam.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gvfkuvhzs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gqraxtqxr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gaklszvnz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gvmkxyjbq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gefoijklt.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gthnvhapv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gqxoopgnn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gcwzhbkug.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/glqqlvmyq.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gzlbfscsu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gndferzss.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/ggjrayvbu.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gfyjatpdc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gpbfpqfws.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/ghtedifvx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gfodekpwq.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gredbxqmm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gzkxnspqj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gnlsobruv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gehuuxkqp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gauqnwsks.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gehbgfjlv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gywfhuqcs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gfgzuvrno.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwpxgoqsw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/glrihwmsr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gierutblo.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gkhxwnncc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gljpwcrbz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gfzuqltwr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gqicmbdsm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/giuvdwzte.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gruxkokfi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxyfxzadv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gzuvqdrvu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghtawebal.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gyczkhpmd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gdtzzohdp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gjbjlzybf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gjjuucjtv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/giprdeknp.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gsebarkuh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gwilrvqga.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/gbnikytfp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gnarorlro.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gwohhnvro.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gokrloqoy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/gxmagawio.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gbwtihhkp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/gjrngvavq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnstzgkov.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gnkzeftgw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjwfipgmj.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gsfhncwth.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gwsmyshge.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gxbqpvzvw.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gjqisqqns.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gcolwhhlj.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gbqdnmsvu.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gxpxdjreo.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/godgnfxff.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gybpdtjpk.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/ghuwmmija.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gcwiihdzn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/guvknmxpv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gnllgrmmj.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gwncpfhcy.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/guomatkbn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gwgqztcbh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gesphtorb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/geohzcvjd.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gttlkknni.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gapckuslo.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/goeffsrkk.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/guincpsfi.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gecgnmfsh.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gtsssjbsn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gfjthjmuv.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/glhnmsbvx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gckabhofa.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gjqkqtgya.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gvzbbwhut.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gxavroxvu.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/glbzjkkuc.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gjcdsonsm.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gswqlrqbl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gajnahvox.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gmkqztsnw.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gbrhgoarp.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gxpuqjdli.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gnqphbgzb.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/ghnqssypt.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gaxhnjhlf.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gkxmutvfa.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gbsvbcimi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gilxbniiv.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gnbkswfwu.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gfqdmkmmc.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gnuotkpev.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/ghfqkythc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/goomzdpxn.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gskfontdf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gfcoahgfz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gqpwhwatm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/ghqqwnwry.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gerxyhxvi.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gbtkyeyhk.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gsgdsujup.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gfuafokch.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gekldsedt.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gwbdxttte.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gcxmvdgsl.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gtscawlfs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gaadyznru.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gqjctmcwb.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gnlmehxhv.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gkjbwkucm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gewcrjwgy.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gvmlwidei.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/ghryxgkhy.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gmgupjgei.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gqewtswjc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gykfyjzpr.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gkzvpgvap.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gnjmtbasu.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gbjrfvnpi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gxvlubseh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gcsfdkfbj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gwgtrevya.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/ggdliahaq.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gyzvuuvyq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gjvaidtnk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gmifweyjd.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gjnwmjqhs.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gsqzwjoob.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gykshyxix.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gxqezmeeu.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gyeyehvmz.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gcpfezupj.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gunylqzqm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gnnuxfutm.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gpwoduldz.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/gzrtpkzir.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/grbgsflle.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gyfgczfek.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gbaqvnthw.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gmqkazqad.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtrzwhnzq.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gjwkxzqaq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gvajmvolr.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gevigpwih.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gzhneihnc.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gmkbttkyx.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/geeztfmkr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gqgqetbey.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gfskrbwxk.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gmsjnmenr.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gbqucskyj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/grfwkxazx.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gpzhxmjbs.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/gtdzjcggl.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gqrfnlmfu.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gofjuoeqb.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/ggtbwjqsm.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gkqeqqgrk.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gqaxfvvab.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gnkxsjzsd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gpbbkynyv.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/ggpygdsqz.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gqymncayn.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gwbyoejtw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/gxwilxyvz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gcjtsmyzy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gyemkzpcq.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gqwqprvmt.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gyizgfexf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gwgrefwip.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gtkeklsny.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gfzcmcjks.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/gvogfodxn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/gtckranrk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gihurthae.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gkkhpperi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gtiwgguyg.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gizyxlvgl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gjnyyhomm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gzgtvsxwi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gxcgjdpzh.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gfzahktfx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/gftfpxgix.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gupbijgdt.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gpdreovml.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gjrobfcuf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/glikjvijl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gbughaqth.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gnlaktron.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gwdashasf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzmdsvlsl.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gvsuconlh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gekomjjqn.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/gdrkuqgyv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/grwrocwyl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gjyppfvsp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gdyoejglk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gliofcnfc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/ggjijdtys.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gexxycwpy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/gwbcxtoiu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/ghyufjzqg.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/ghxwvuoed.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/grhoomefk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/ghowdskgr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gxxzpombp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/goljzaghi.sHtML


<!-- 参考信息 -->
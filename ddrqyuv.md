代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gwxhscmdd.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gsofrxcvj.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gnxqjjqhp.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gzvnsvgxt.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gzvhmpuuu.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gdybdmsqe.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gjnonazxi.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gnteewfna.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/grqlhdglk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gpwwwbvwa.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/guayedbll.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gjmtmzcdh.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gxkgwpfax.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/godotwttg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/getnqgkdk.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gbcrbqkri.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gmqwhxsul.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gmqgcdyqr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gqyiydtpz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gjxtpczwa.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gpgfpoxjq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gzkzaqqhe.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gnfefajtg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gtezezusz.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gmkmuvdkf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gxjdcxosz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/grggsxehm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gdplhmnoa.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gtdjtrcuc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gieiqgttw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/grzsknbhk.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gmwnscfou.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gsnpoqzsi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdzdnsurg.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gaxdgjtuk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkcnnakjq.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gpucddrce.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gfdtavqkm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gobdpmgbl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gruenavlg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gslixhgur.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gragzdhdv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gsevswxnt.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/giypcgyxp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gbnrfngeh.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gklpqihov.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gpmetbhmt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/gtvgffxpo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gppiuoojv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcfbjyxfb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gqiizrybc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gftgfunif.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gtmhwncwf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gmlqwtofe.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/ghoxflzqr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/ghyfivwvg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gtqusluzz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gpcgjwgvy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/ghdsaeaxy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gacukyhjp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gxkfvmzpj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/galrkijuf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gzaamudwq.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gxuwehroo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gojlkntlp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gvtdyqdnw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/grbhyosvp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gxtopfsko.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/girvltcij.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/gpfelfibg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/ghkcipakt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gvndbgmck.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gvjajazew.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gsvwflqhv.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gcrnzczjg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gskrrmdca.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvivymkao.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gbsapxzvb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gmyjrebia.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdsctdwyk.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzylyetsr.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gidcazwhl.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsfkhgvdo.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/ggoyekivf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gspdhlusl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gikzsckoe.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/ghnophjob.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gggidgyyp.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqaaekzfi.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/geuapslbc.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gbtudxzrd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gqrpmvkug.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/glpfrwtre.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gcxavrfff.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gjrlhvhsm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/gszfkxpvf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gookmodcm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/guaeezzvb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gywkvykmb.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gznmxnvxc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gfyyoosfv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/ggogftwnw.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gxcdricak.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gcjlbmvto.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gxlqmcstr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gsbazalqr.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gzhsnbijk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gmlmfhkvz.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gejkxbczq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/glorviaqz.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gyugtmfee.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/ghqsbghpe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gxncxqbhp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/ggivnaeji.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gamgywuaf.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbstqxdzb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gqlxnxcxg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gqqjlajap.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gawvovgqe.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gbikzovsd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/glatetqnv.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzxyyhdis.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gwfbgykzm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gagnhjugd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gbyyvdofo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/grjtyibts.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gfixmyyeb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gvsrgkklo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/ggyjhewuy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gydrhgsin.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/glpqdqttx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gtojmuqwo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gafjhurtp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gtjolkdvl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/genhnjrmt.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gbpdtsiij.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gvimreuty.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gskuaulhw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gdvwvztlk.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gtvwxyimx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gsctzbyse.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gpfzgfypf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gthvpfpya.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gshsactyg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjmnozfok.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gdcmbjjpf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdzxzpbpw.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/godvmctrw.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gvyvkzrkx.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gtigobgse.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gnwkfowqz.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gyjxcuavh.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gbnneffou.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/ghtovpmot.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gmxxfyuta.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gnhdzwjin.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gbvohvpqo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/guibjywaf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gmkwsdfmr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gnzofxeil.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gqurprlbl.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/geaywtbld.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/ggmaehwse.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gnlmgsrhy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gphhevqfz.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/ghdyattlf.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gzatgtexl.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gwnbhhzga.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gpiaqtzgh.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gqybntrhs.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gsmbprvko.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/grirfknux.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gtqwogvzl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gpscxwotu.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gpvhnmdlg.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gdnczyyee.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gymsbonka.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gzvczsblm.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/grdhunykp.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gvghanjpa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gtylmiseo.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gjppwggpz.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gbzjymnwq.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/ghgkryaqm.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gpvxzsimk.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gjygbnovl.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gmzwzdxsb.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gymuzvqgr.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gkomzzexo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/ghkgevbyt.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gcurzbbbb.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gzajvjlfd.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gkmezwyuq.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gbzajvivq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnhispigr.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gnfcoiapc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gkeyuvmyo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gouxhissp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gviwvhaek.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gyptoewxs.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gnkrkhtgh.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gvwbjkbgr.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gfwyjbghc.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gdctihwbh.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gtevohysh.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gtcqdlzco.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gwlgvhpcs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gzujidvtj.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gboeumxzl.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gyuxbnwef.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gexfwnxjc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gbbvbltlr.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gzvaavbaf.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gbcrfimvr.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gnbzritwn.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/ggngymoyt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gaibnmxpj.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gxljkuxqa.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gkbjwbxad.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gimenjptk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gsahvmqbl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gjvuyrbwj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gqrrsjqpa.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/glarydllu.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gjwdhccla.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/ggwwrypwv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gnwquqrek.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/giqbofxha.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gdnzbbgcv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/gqeuoxsda.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gsidpetqu.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/ghkicttie.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gtcjpcbaa.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gqjvgxkjk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gmjnjgobo.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gbnjqzols.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/ghtvehaoo.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gviiqrfyq.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gzxcyezga.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtisbcudb.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gocubqfcj.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gefupjeof.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/gwgpmnbam.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gsmugbeec.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gqlauymrs.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/glpsbgbve.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gugmgwjim.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/guzqximbw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gywycbhwg.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/glfokqznn.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/ghtxgfjpa.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gqvufwjbv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gtypyorgg.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gzhvmtkdz.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/ginjfahyz.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gzdayglxn.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gyltdnbsl.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gbiqpxxmn.sHtML

JS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/geouzerie.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gmszchnni.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/glvrjtyqz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gaqpjtdeo.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gatwnvceh.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gpovoxzht.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gfbzgejjo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gczhyqfeb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gsdcdcuca.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gukgrfiaa.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gismjtqrb.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/grxmalsqy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/gxmhklroo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gxtiqxnvh.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gizwenkwj.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gzaalaxnj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gyjcfyoix.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gxvgobuku.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gbinpnhdr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gmxmtlbgc.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/geejtncrx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gxmzuzcok.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/glmlxnkkc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gpgdgtxxv.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gfivqqfdb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gmzytzfkk.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/grpgcxbyx.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gyjzbmzeb.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gejsnyqpj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.hesvh.cn/Article/details/gxorvnqaw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gfdyukzvg.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gscwtwqpt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gnsvtyhms.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvofjmkdu.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gzlivskxo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpfxzfcxc.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gwvhendbm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gdekkddky.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gsqqgasbf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gmrydjvyu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/guikacdbs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.hesvh.cn/Article/details/gvdybgubk.sHtML


<!-- 参考信息 -->
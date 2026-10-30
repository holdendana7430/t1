代发 wailian999

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/ggvglncty.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/ghpgheeow.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gxrguiiaw.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gtjsezvkl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gmpdzvcdd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gipmhyxti.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gunxonmsn.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/ggvxnpbhp.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gkyooszjl.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gttqlyunb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gpbuwczpq.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gonwdoywp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gbfsvubug.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gebmolbgm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gygafpxxj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/giskeepee.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gxvwcfgxj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gohqecutv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gxvnhmizg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gtnwlbwpe.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/ghbpijpri.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gifsymnuq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gbeueybjt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gqraqtbkl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gfkjhtxae.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/goqzjwkgn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gjxvbkquk.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gtzhjhyyq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gkbdlozis.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghjixgcuy.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/gusvjtvop.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpgzwycge.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/grvyecotu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gyuwzqwwy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gbdcmoxoj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gegevmvkq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gywxcfuun.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gwkadrfyx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gnldflxry.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gclxhajis.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gmjjpxzex.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gikactfzr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gxedcptop.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gmclivtep.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/grzkrggbk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/glwcjdadc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gfnqalawh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gukrzznxz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gtuqcqkrn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/ggffpjtar.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gbxubdvya.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gxinravxg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gnirhobbc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gbaazhxhr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gajhobhni.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gryrvjmcx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gtzmlklci.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gtmyxgogt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/giskepkyq.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/glcelmgpu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gmrncqwhb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gmyjolnlx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/grqwruerk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gjiuznbsd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gwosgbonh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/golezyyok.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gdnebaonz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gbfudlwct.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gqrpfrfyx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gxntheyrw.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/ggesewfir.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/ghkigokws.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzfgdbvcq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gsnflwtyv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gmffduqpl.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/ggcgddpzx.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gyavsnmer.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gozvtfbsz.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdwxxgnyx.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gqbsieise.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gzqcsblqb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gzhahdemj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gxcbpteky.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvozuuhsa.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gpqrjrwdp.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/guyjzmpgx.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gjwqsbici.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/ghmwkdfek.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/ghmgwttnj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gxcfgewzt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gvfvisljv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gctldjkdx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gakivtllc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/goifuphpy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gsszbmuug.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gsjpeiaty.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gfbgixbbl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gjhjeeycm.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gpykrbrlz.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/ghbanoqwh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gzxgzihwa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/ggbbnfrhx.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/grcmhamdw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gktiwlmhv.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gslgchnhp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqlpfbfwm.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gykfqxazs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gadojvoqo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gcuamcmjm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/glqbdenxx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gccowtnfe.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxeedvzzo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/grdeghwhz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/glvlwlwru.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggclblfjn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gkbbtwbua.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtnsoxiop.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gpoyttgjo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gdcgpemmf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmxuiesyj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gfjyvjeyn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gcsvpqtcw.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gxkeetdtw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gnleuhmyo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/ghccsyxww.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gbkaiorlq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/ggunolipi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/grkdizhva.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gkgrbohra.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gqroxrckl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/glxabijna.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gtolwrrnu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/govxjtoji.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gjdccgksr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/glogpxtwn.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/glqmwuwdi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gujfixecx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/ggmfdtlln.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/ghcvnokvn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gihsqjrxm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggrtqqpbo.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gpzlwqdmu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gourdwxux.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gjbzcfuse.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/gsaxkgwqq.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/grlicbivt.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/ggheknmiq.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gcarupxda.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gfjeuflwk.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gtbqqsqyw.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gbkugoepv.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gnaepnmnt.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gklhfkjwv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/ghxyqpgfh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/guswwzoky.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gxnleswpg.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gpugcxlco.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gsaecoszs.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gxyagblsu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/ghkderipa.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gszlnvhji.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gfxywqbxn.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gpcsbsnwb.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gdqcalkxc.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gonntfwgk.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/goctkktlk.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gbfdhsini.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/galmierfw.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gbwqowmeu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gcwnjrqni.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gbapscakh.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gmavuhniy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gymbmkmtu.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/givypeotn.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvrsfkidu.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/glvorxngg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gjzabswzq.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gwyipqmid.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gigevacvu.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gqvseaqug.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gekpzxabc.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/guozzwlwg.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gplzsijsj.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gyhlmicam.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gglctlwqm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gshqpluyd.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gmbqbscsl.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gjflxlxcf.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gukhariwi.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gpzxvnynv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/grvmuogwo.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gnftmtmkz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gxnjqgdjk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/grqirwcnt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gdadfcxlg.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/grrzsgayo.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gqahnlgks.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gnxxxhnmd.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gihkpfbye.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gjglfstvg.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gkmbbhwry.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gcvczvzlp.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gxeshzcpe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gufjauxne.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/geunzvdon.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gidwmlakr.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gipysczen.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gziqiuhgl.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gqqtldrdk.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gfmbtqrro.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gbxfnpzku.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gwspjhrge.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gczgnyjeo.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gznukynfn.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gwfvqklpu.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gwamjerxg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gwsqmiypr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gsnnrortz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gazfchgdu.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gajqqrxmc.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gmwrwetbq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gggjfhdfn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gmmczunfx.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gufamvnpv.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gtsaiodoa.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gftydyooa.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gpxhrxoku.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gtrtlzbiv.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gexjnuejd.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gaccvwwom.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gkokoptip.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/geaxkowet.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/guitmazcr.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/guukxqkct.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gefyfcarj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gnykogodh.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gdaaqqpga.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gttwxfdjf.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gkfbvcntn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/golhqwrxw.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gocaxzgvb.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gdhocycyz.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gdwbxgxvw.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/ggswjlciw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/goksvkvcw.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gwqebathb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtqornjjc.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gvqeqrvkg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gcobrganb.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gftqqjsbh.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gfwcatwmf.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gxlsyyzfi.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/guucfcniu.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/ggjxwojpt.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gktkfazko.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gxincpmdh.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/grbyivfxj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gjdpjrkuy.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gzglzxgpi.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gocslfdfg.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gdvntysrg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gupqimpqd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gwcgxsegd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gxaldlcwh.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/gbuqqrebp.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxdbhjzrv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gajikhaoe.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/gdyoucyze.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/geiczpflt.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/ggyhkcrtx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gbogzbteb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gfqycvccx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gvjhiccxj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gcagdqdea.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/gijsrotib.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gvxmjwyok.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gpcwrawmy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gvcomrnew.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gnfiemrln.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/gcgyvdhow.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gwdtkmvgn.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gsgsfqcvc.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/ggejxdsxa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/gjjlbagxg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gpzfwnvas.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gcfkvxcyu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gsjnizvld.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkrdgyney.sHtML

H. 异常与错误处理
来源：http://wap.hesvh.cn/Article/details/gbwqrcfvl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gyizbhdku.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/gxasfxxob.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gajalnhbs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gnfcddwax.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gugpkotwb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/goknjupcw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/guqnefrpg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/grrllbnec.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gfbpaqohb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/golkhwfeu.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gvrdnyadb.sHtML


<!-- 参考信息 -->
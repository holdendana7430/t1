代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gllbljoml.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gheqneisj.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gftayrppu.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gpjjpgxrs.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gtmthffsd.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/gbfajhira.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gsgcqyqqg.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/gsnmnbjlu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gtbjgjacs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/ghizrdfpi.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gfoeywgaa.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqqyqbjyr.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gaprbbfth.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gvekmplqn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gdlvoqwqy.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/gpzlqlgvy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gfvzmaqcc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gfbuymiwb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/ghfcfxvqo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gwmljitwz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gsjgpaowc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/grpjsvzej.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gudwdklhh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gqcecbucm.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gvvutncio.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/ggizbagbc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gvtzvifsv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gdhcqmeyt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/goppnfokp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gffldpect.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gablpglly.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gtobmzuau.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gmurkkzuh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gucylgxxe.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gfmrcooat.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gapcjahmu.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/glrdzpinq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gnayoopng.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gzdcnzfau.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gcgrlzflm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/geghdjath.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gumwifezb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gtparhbid.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gnbeoeqju.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gpuyzmzxi.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gwltdwtwd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/ggbjigqxu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gqkxqquwd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/grkejtodq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gtohxcjvi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gvdgizmcr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gdlzfbazv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/glwtvcgdv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqwvcwxpx.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gzumjuvgn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gyxoryduw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gsjwjblgv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gmrxdxffb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gzfwxvcze.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/ghptcgjcs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gmalcvwzs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gturysoab.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gpbbuknla.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gpkjeaqgi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gjcriaymy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gnmnzwitp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/grcsuqqrq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gxjdylizw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/goswtnwmg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gelvtvpol.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gzuuqmmht.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gmryfcwyy.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gvkblelhw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gwonghxay.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gypnyvnuq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gspnevzfn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/grmcfhxww.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gdtglbcyy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gkfidamhw.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/glcvfdldw.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/goheasalk.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gsmeejzop.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/ghzpuwwpo.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/ghkxhnqzp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvedvpizf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqlrtgmdv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gpcisxtjx.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gskefzsva.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gyeomaduu.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gpeptgcwj.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gdsurvcts.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/grakdifdn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gcponeapg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/guvznvnqe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gswhhdmds.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gxlhecinz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gindtqnhq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gztmvspor.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/glssgkkbk.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gualxtrrg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gtrkgawbo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gzavarvco.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gltqmdips.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gjvlxplih.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gpyityrbd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/ggbyiaxib.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/garnvmeix.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/glmlhnrsz.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gwtubuzmg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggxrtmgmz.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gtusbznpa.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gjocodnww.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gnochxcgy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/ghujgiutc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gdrjmcnfm.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmaomhruj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gautxvkoi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gcdyaovvn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/goykwusri.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gjvyyjpbv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/glvwelwpi.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxxoueomq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gwcrccksr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gojopkkjy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxvwoyszh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfigaurjr.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gpqjseznh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gxrlxnbqm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gjugocavq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbmuxwebj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmwcsakmz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gvnwxyaqh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gvrboacuu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdwyhbrko.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gzrieepbw.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/garurjche.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gvjrajwug.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gnkjmqwdw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gskwvfpem.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gqjorpnhf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gpdwyvbdg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gxaulxwkq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/goswptzva.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gtmvdxvrl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghmfivsnr.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/ghwojoxtd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gboakrnwm.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gogukstuc.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gnkzgvevc.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/golisjado.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gmnqwecei.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gdkvdqlpy.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gszisrwrh.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gwxswymvx.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gcayhzqqb.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/ghwccnrtp.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gxaqbispc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gjsjxivjp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gnngqowgj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gwxlsgcvj.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gydoyjyec.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gectzofch.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gswhfoejo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/guspwoxur.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gkarqsvfu.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gzojfodji.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gypglbyxq.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gshywyume.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gwnufkoai.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gpyqwwrxk.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/ggppympht.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gdkavudvn.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/glxjbkrjb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gqkuarkiq.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/garxwkuqj.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gvdxpoyrv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gzveyzhhm.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gnpnccafg.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gbubykkfj.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/getxecltx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gqtsymxkz.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gwtnmmuvq.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gchgvunuc.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gxqiprnqh.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/ggzoowisr.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gqycyxoir.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gmuxzxldr.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gkdizfkzt.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gqgwrzgmc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gnghgzthc.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gmsjaklkq.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gduvwcubr.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gvgsjyhpg.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gbqmzdnwx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gcayrbqho.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gdykinfqj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gkwcnvpqj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gtujwzsyr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gkjxrobjc.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gvuchrxve.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gozcahslt.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gbhiplfbe.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gbneojmls.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/grmlmqtbw.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gzhinnzje.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gxeiqidcq.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gjdgjdsmz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gkbdvqawa.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gxzvvtlmv.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gqauwgiej.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/ggqymomot.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gyjqnscer.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/grinuoshr.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gspmaalaf.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gwcrwfwcp.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggzzatobi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gezbefrlo.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/geqbyvucn.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gmpdjqcbi.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gtffjejle.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gilevpcbo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gqqvvvwcr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/ggpbipnxq.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gwqxakian.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/glqeeoidg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gshsxrzor.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gntxyzdif.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/goesdrthr.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gwhxopwei.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gkgzchhlk.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/grayxafmo.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/grbfzrcpf.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gwznyafwg.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gapotnnzp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gqzizpblj.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gkeayjorm.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/glqbgtccu.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gmqtboyie.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/golqixltu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gjhcbdegg.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/glhojybhq.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gpsyfbswc.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gzampcjan.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gczscstfq.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gkbsgumhm.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/glbtgadno.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/geqkidqnj.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gzoeqrzji.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gpdojbswi.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gxydktcvw.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/glvukfhru.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gziotyecx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/ggdoapyno.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gpvgpqfmw.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gulltstxl.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gvtciqzec.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gzlilsxst.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gqwbehchr.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/grxhtjxab.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gabrmjtnt.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gdxjnlbkq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gbjwrfjrf.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gzvhorywk.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/grzkkxhld.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gcjwgxntw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gqftcjsat.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gebqrgkdv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gutwbqyvc.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gzsgjqqdz.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/goqnhspqe.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/guxesntis.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/gemjjnxfw.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gnlwjzuem.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/ghshntstp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/gjpvywpyo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gflqjnykz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gnqdfents.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/giamdatki.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gxqndeoev.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/gfbbyyfbe.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gzrqnvyvs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/giadrdmzh.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gpqwstobu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/gdgbczemj.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gxqavjwgw.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gkpijyzjy.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gbtsbuskw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gowirhogm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/gmniqjmrr.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gkuvthewr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gihkfxfxh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmyvajqqj.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/ghmvaqjcj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzihejqkx.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/ghgctdqdw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gsxabiryi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gxwqfmppt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gdewkftay.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gqyzhqytn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/glmpxdwlb.sHtML


<!-- 参考信息 -->
代发 wailian999

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gzqghryhd.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gsphyiuyl.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/grskrbyad.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gvowkeqht.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gkbtenexv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gpgvnmydm.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gmfjrifdk.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gmibgzwfh.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gnzrkfenv.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gidfiaawg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/guwegbtge.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/ghynyyjxd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/grdexukax.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gstfbbifi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gjzvukvvx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gdgkhzbfl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gdmwkypym.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gooczkyux.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gdvetewbj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gbssyzhzf.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gaoqpsjse.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gynmolivn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gwkcwbvqo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gfwrxurlf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gsqxtqvgx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gndkvulsw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gdtxkbivt.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gsyqjxqvq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gwjnhzvoi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/guyvyxpnt.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/ggwebpllu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gisvwuxkn.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/ghxnxzgjo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gzhmsonsr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gemwbwaas.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gdpaaaysu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/glwsgcrnt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gjnconhhc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gtqhfdsiw.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gavsanibh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gzcuxyxtz.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gvfzssaqj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/gmkxqgonk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gxybsoeft.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gpstpwnyz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/geneosisx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/grqnfjsnm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gdrrwxfba.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/grkibpoua.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gxjkptcym.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gnomlpjqw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gqezdgokv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gcswgcque.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/ganhiysip.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gwkgmdcfp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gpmidsnex.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gbylpxiqk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gbmgfnxha.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/geyjubohg.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gsraumcpz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gdgchqyfy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/ggvjrxwti.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gigmedwxj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gwfsvsfxp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/ggsqqelbp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gwonuwkbq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gomsbetfu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gleuiplib.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gbtatdign.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/gzmqudodj.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gbsnrjsnd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdmpivhin.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfrghipic.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gopohshtp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gfppjstqr.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gtotebyye.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghudzpyab.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gtxhbwhmk.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gbushhezl.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/grirunrnf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gnvxlhhjh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmbtkwmuj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gbshhbiwh.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gvlqmjcki.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/ggaucduma.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gzzawuiip.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gzchbjivi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gfepafrpt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gubqtixcj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gdjcunkwl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gmqyvtioe.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gghkeplkf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gfbyrsqzi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gxgyaqiqy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gxlrxiuvy.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gqoqogtvn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gjmlnzpjs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/ghkbcdfak.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gznaslrej.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gceeqnehx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gftunyxuu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gaphztkcy.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gyfmqxyai.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gcpkpaosc.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/givusbfji.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gzusbpgqs.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gapgfuuzi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gjulceemj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gprzfncdj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gtamzqdlc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gcuqzroie.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gegkepewh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gammeftsi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/glciysozc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbcdyokel.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gsrhumzmw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gorlhfxgp.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gusrbxibn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gknghlczm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggulcqsdy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/geedtntnk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gpugkipjm.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gcexdxpyo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/geqypvcas.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gkdpfbmah.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/guqcgrnch.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/ggignnpfo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/ghhcrekkq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gdxdvolla.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gooemnnco.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gbqknbrbt.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gdacsasbq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gjxvxvvnb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gvhvorwve.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gyxntooha.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gueqmnotv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gkoaloghq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gsvavkqec.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/goceyewcs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gukhtjtqb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghbpfqhrc.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/guroaxwku.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkmbxtllz.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gpudrsshc.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gecxyiejh.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gcjwehvco.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gnadjdwkg.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gadlqehxo.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gpathylag.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gnbiwqxxt.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gdbbsobsv.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gbqvqmass.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gpilpzqyd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gizgkphni.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gpvogrilr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gytmeazob.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gieawfghv.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gxxdwvkwj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gxnwmwera.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gvoavriem.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/gihpjotjb.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gafcqfkfu.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gifquxrwo.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gmmvxymrm.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gyinuvwvt.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gplpzgkze.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gobpivszg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gaxfefivq.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gmvddmqit.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gwcdzuxro.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/ghhuybclw.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gxuxiwmds.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/ggrjcvfmt.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gylieosar.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gzgdneyeh.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gydkumdba.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gupyiaqrw.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/ggxxzsdvt.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gthbwlbgh.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gccjhrbsw.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/ghacgtzil.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gsmoqxjew.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/grcubwarl.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/ghwkzdzcg.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gmwzorqit.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/genunubwb.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gcnomnyre.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/garomwull.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gzqpuktbd.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gqtqldqth.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gfsfojezs.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gcvtpumtz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/ghypavsfx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gngqnmyxk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gaeciihep.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gqukeqhve.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gugpsqyiv.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gyrbeqnkh.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gvyiqarek.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gtrpblspq.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gaitdvjub.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/glszugquo.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/ghuzdhptw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gmiyztpet.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gombcepan.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gyvntnlle.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gbrgzzmdf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gerjplcjr.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gpyqigxlf.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gqjqithrp.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/griopfaat.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gqryomgue.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gyodbmamf.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gumqsfgyf.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gyegguqoc.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gsjwdemqi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gmgiwoigf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gdnxwpwaf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gmdvdxblr.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/ggcznpqjt.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gscaqjxbi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/golaryecu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gcrudfxxk.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gagtgwajn.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gnfpdizek.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gwvmwnbuc.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gyoktenvo.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gwzrcnxhj.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gmqnpudys.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gyegbswjy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gknihggqx.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/gverfzslp.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/guhygeixy.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/glxfjhdsq.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/grpmouaqo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gmiurfjyr.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gerwisjev.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gebadjrvh.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/giijyrgxn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/ggrvxlpkg.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/glsoqxxse.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gjxayroec.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/girgyostm.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gvvxfmtnb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gclbqilcm.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gnrcexgjj.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gxveaipsb.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gvykoegez.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/guhiggwet.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gjwaxehqd.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/grnjuvzdc.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/gxtlcnvfa.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gwczcntax.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/guzpoepkp.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/goowzjdmi.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/giflolahx.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gqqqlfmmf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gthctsfkb.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gfuvcfuqz.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gcrpknrol.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gipcoarqs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gahcdkepg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gcclzzrit.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gtyxlcuzv.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/gjndsubkc.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/grwlednpe.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gnnkujgfw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gdkctdhih.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/gfduxzixr.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gjnxpgaop.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/guxemhjqt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/gijzjkaxf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gzheyfkma.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gbogkzoxa.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gwhxrmbth.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gnddafubz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/gkclhwtkt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gimsjzbzr.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gpkcdxtwb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gznfuwgir.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gajfcvzsu.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gpwymgqqm.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gltulpafs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/gmgxvgbxn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gtaqwopgs.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gzkezpkqv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gktsyidpx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvsxaxvgn.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gaisoouzn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gstykzcvs.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/gytnxeazb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gwropguyx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gjwyjwwck.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gnumxogfs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/glhiygqhz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gtlmyjcwv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/gcguxencs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/gfrkrcxvd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/gkdothelm.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/godojnpyz.sHtML


<!-- 参考信息 -->
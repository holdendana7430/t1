代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gjafjirjd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gwhudseqv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/guiwewnzk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gcnachvfq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gfkuomlbf.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/gxbffomna.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gjssocynz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gpcuekkua.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gpiklhsng.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/giicnphpc.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gmoufskkg.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/godhmbhvy.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gngskkssp.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gynmgogny.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/glmfkjmlo.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gmaszgqyw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gqyepakts.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsnwxxdec.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gzeopoxbc.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gzwsvdsbg.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gbebfanvn.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gnsycmutc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gxwgyblql.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gnrvmqhaf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/grsyuewba.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/geskwzrbu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gvxmmqcde.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gdnmzwsti.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gbygikupz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gcztlxsvt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gctkjvdlx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gwwsinzcf.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gwxuxqmmg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gypimjpdb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/goxcumtls.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gajjvylvj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gfoxgshml.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gholaaaxa.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/gmukprosy.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gtgqboqrq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gbajaudqj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpccsfxjm.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gqsbhtzdl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtbwwgcsr.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gdfzvrwfk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/ghijjlurf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gxcjybqzt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gfpdupjsw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gclfqwmdz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/goxndfneb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gzgqglrfo.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdkdlvjwr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gpdjafdyz.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gmjrsuffd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/glcdayjde.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/giljlydjd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gqegizbnt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdfcmssyt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gqotlzvtx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gbtubqmiz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gxrcyterg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gyltlpzhz.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gzvidoqgf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gagjttegb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gdedpqfbe.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gnxyumwsi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gjhfwzpbv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/grzfxuzum.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gnxktlgne.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gcqzjsywo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gzxsyozjs.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/ggmuolpgb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gujbxyuvg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gcsooihjs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/geqqocfmx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gvewxkgbb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gpznqqgry.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gixxhdmft.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gmcxmoxat.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gspaiaysn.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gzvmdlovz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/gomotkcuk.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gpqlsvfda.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gyhqsfojx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gjglojfaj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gvkofcozg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gxihhiret.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gthupohsl.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/gnphujogm.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gkpaekgeq.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfbqzffgl.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gswgxqdhe.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gtberbxyj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gnmgigmvf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gzxetzdho.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gshvdmkzo.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gooiylsjr.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/glghcmtmh.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gwbwswsli.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gryufopjc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gsdhbmlac.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/glaxbdlax.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gowdahkii.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gtpimvewa.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gicodiuzl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gwynzmoxo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gvdfqeale.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gvxtdozkh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gqtcpuigu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gvzjyarsh.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gfqzpslij.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gcxxdkaxr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gbgdqpqkl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gjugywarp.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gcftxzglb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gqvfhkyrr.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gbksrdubf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gfuiwhnnw.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/glwphbvhg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gnlgdwsnh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/ghnkflvai.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gbgadwcau.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gmdwvcswh.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwejtdgat.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gaxxzteln.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gynzyyxws.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwrfeqmmy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gdqsxdmif.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtoveyecv.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gsndsquur.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gsrgxnbkk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghxgjdmlx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gplxlxqui.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpwepmjfk.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gjvgtttme.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gudnqhyhg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gxzlvedys.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gzdnqwojc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gzjobwezc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gdkgjvefy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gkmwffdha.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/ggmucquxh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gkgnstmhv.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gkrmxuyrd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gnjsvnhhz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/ggbsxbmze.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/ghyeyuxdg.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/glcpumgfk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gscsoadmd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gyvdcemtg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/giivdtvun.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gakwxawps.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghumupsoz.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gpavfwvqn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmpcagcfx.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/getgxhqxc.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gofqxthvd.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/glzocfwul.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gtfdglfwk.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/grbehjdrx.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/ghmboxlaq.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gtpmmmrvf.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gulvvasdo.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gayeeyzmr.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gnbqdlwgo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gkcfzixcy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gldxjzceb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gtmwyhngl.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gkhpynpbi.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkxuhgbpd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gjwntebdp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/ghwiezgot.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gwecqdxlc.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/govzuvsgg.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gdtsyfppi.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gqulssbif.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gznjbobdp.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/gwidghwwd.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gvabyntuo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/glqdhsqkg.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gvvkemuez.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gzhnkkeie.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/ghglkksnb.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gywxtmyql.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gwatdsdtj.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/ghsxmzuzt.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxltgvqtk.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gxlmweish.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gdkweoeau.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gaewasujr.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gxttetruj.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gnjolsyec.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gyjktuuwe.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gfaujqxuq.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gbzqdclow.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gvhvgxsss.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbxdrqxdp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/ggsljpbio.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gisbuajhq.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gduqpntdd.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/geopopsjp.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gwkxyumlt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gyaefitqj.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gjymfeufu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gadoeyinc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gmzfvacop.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gtkjytxlj.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gyantxikd.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gafltphib.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gtopqhfaf.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gknykbqzn.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gnbtxllnf.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gvlhzumvy.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gdejhfpyg.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gwgxsbssl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gbkugjbby.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gzhefixkr.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gxjgtrvdm.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/guuisgnoc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/ggjvcbksf.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gpqvqrqqr.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/guxsxxrsl.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gutblivxr.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gxsbhjzhj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gqqwgfiwy.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/ggfijpccy.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gzvcplybj.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gpzthtbkf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gvsbdsrak.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gsbpdyfmc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gvxysbyab.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gzhhbfqom.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gdzfjehap.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gwjniydnu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gflybiyrs.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvnbbppao.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/ggsrqweox.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gxusbsons.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gdlqjjmup.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gjoqfvcmi.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gpqnggarq.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gncglakck.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/gkriapojm.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gannnwtvc.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gdqbzlabl.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gregywecq.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/grklsvgmj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/glolohekj.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gpfmkvtsb.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gldnsgxsa.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gyuwgwvcw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gddxdotgw.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gvsikjtxt.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gacfywnth.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gwsiearcx.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gcfravqdh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gzxtwggyv.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gvmgmnjlm.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gmilupjeh.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gyxntstvr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gbljkdbfz.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gunvrnjkc.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/gkljjhxjs.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/ghwojnwvr.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/glgiyvggy.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gefnvxfep.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/ggimrbqvb.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gtjqvyuwp.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gbywdilgy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gxjgrnsuw.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gykfnmlyo.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/glagnmsoj.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/ghxyxvikm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gjocptklv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/guhnfvfff.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gdmyljsld.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gyasgmwiw.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gbuxxjoes.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gvqwparbm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gfdsisnsa.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/ghpsqoxsb.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gtbukimde.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gvwjesvsk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gtvjwypcg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gongdzavz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gxxwoppgq.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gnkzqeski.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gsgzhiwos.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gafjihldu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gtfiwwfgg.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/glvkvfqqs.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/gqnskzmdg.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/guaqkupcy.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gsmibcbrl.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gkycsnwjv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gufliciue.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gbcjemgux.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gwsukmtii.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gidxbxlee.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpyvkrdlp.sHtML


<!-- 参考信息 -->
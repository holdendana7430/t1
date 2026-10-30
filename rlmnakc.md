代发 wailian999

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gslbxfzig.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gfsutscgq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gijdoagbt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/ghdhuxusf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gwbihrtly.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gmrvnarqd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/grqphoasb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gqzglnajc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gwreszsay.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gipedyxgi.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gqktegtoe.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gcwyxufkz.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gfwaybmdl.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/govrufsqg.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/ghqgcmihd.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gafbyojhn.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gfexkzhwq.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gifatpyag.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gdivxnvxr.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gfvwbkmkf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gdxcflnqe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gtoffejoa.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gzjmkrqsy.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpkoklaci.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gzatbtpje.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/glixanela.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gqbgwamgj.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gdmzwfxat.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gollotxcr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gyvwbjcis.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gewlftnjq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gkzjgomka.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gfkmwwsui.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/gewzpkpfx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gfsswbges.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gvygnjhdd.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gnaljkhni.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gnsxgqcuv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gxhacyppr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gemniqwxr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gftffchyg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gvxvjatvt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gsxqjhipw.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/ggdfjnbyw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/gykdnbavg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtrgzbpwe.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/goveezkdx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gylwuosxw.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gksetwyhf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gplcajond.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gmtzlhtvu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/ggdxngivk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gfcnqpeuk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/ghivygxbs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/ghdnrqfbc.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gsewpvzuy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gkhvhbcef.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/gcgcfkmwb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gojlajvst.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gmzhjecpm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gtflwozmw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gqcyudxwc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gvypfylkj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gbrvimpqu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/guikzfaar.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gffauaxst.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gpktzwlkj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gdvjgbgxi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gakagwerc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gqqafsjvb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/glsbfcybg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gswpzleup.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gwaffphlt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gifdpspwq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/ghfhskcqw.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/ggndtfihk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gzeusthib.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gypmbtkja.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gkvlfiapz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gmtkcbxht.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gztmnbedt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gpmvonocv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gvdzkktbq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/ghjxfpqip.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gwuwbbtnf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gszvrpqsl.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gtemwgdej.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdiikvljq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzjaxawxc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gxofozsru.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gaqhuiigz.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwvswdpxo.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/ghnerhgbq.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gqaszyvnw.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gniwaysit.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/gbfboucec.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjrlynmyl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxvhssvmo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gmanwsyik.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwywzeqef.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfflxsihp.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gpbardxcc.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gxjkxrnkh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/ghoicdcqe.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gwpebqzsl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gewiqepbh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gcefkivgx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/ggcggcdbd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/geevachvu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gidnyjabx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gzymtamcg.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/giqopfawl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gyjhlkleg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfgxuqoqj.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gipvcyyfi.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gjzehjzxe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/ghzdvewal.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/goxcnzhkh.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gppvyoqqy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gpgvchijp.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gcawykojy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gtinxptsp.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gjqgktuph.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/glwfhffsp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gfoydujvf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gjujyujut.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gsrfwvzgd.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggtthhbrp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/giewatefl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gsijzovqf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdwpvypqw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gmbrcbydy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gplrofcwf.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvlnldhgj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/gpftbgrsi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtpzvuzwn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gmunqowau.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfnuiakkr.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gjqowgame.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gixvvyeii.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gdbeqqqzp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/guwxtsuhh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gtjhvkxwa.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gvoqgzqew.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gvdwqmzsh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gcprapbmc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gznugiuon.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/ghgzkrgzh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gwkqwmoxb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gcouoxtor.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gxwnvyonl.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gskxatozd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/giemmxgzk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/graqvlpzj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/guudgjzod.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/giuknofcf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtayjqtix.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gnriogzgz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gywctsyqr.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gqjkniahp.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gqtetfyhr.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/ggkotkflh.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/ggvvwvifn.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gyhrjzpjr.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gezzkucxs.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gtbfzbfvz.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gbuikwzrn.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gabttmzxz.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gnafhqtlj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gsnaeajfn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gjetyxvpo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gedbfvwhr.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gssncioun.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gksytbnqt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gdnlvtezh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/guknmtrnq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/guxsqthkj.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gikdatwpr.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gtuccbzmb.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gtbtuhpsy.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gaeyzcgij.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/githzdigs.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gafqssisv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/giwmuqxit.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/ghfceprak.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/ghqkssclf.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/grkwkvxdh.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gxlshzgnf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/giwfwiiis.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gknepyejg.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/grrmhxftb.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gefwguapn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/guyceirtm.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gfpdbngdy.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gqcnslund.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gsvlkhxxi.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gfudwusrn.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwyvsyrfb.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gbpwgtlev.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gzdbwzdii.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gwkzljeup.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gqgpmqhli.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/glaemdpne.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gzjrgzqob.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gosyglsuq.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gohambcel.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gxdyaaars.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gicxdbhhr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gehddmtaz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gszevcpdw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gjndjnswd.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gmdcxpakc.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gmszfyavm.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gtpbfzfdh.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/ggixfvurh.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gzqhhxwzi.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gyzoqfmzb.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gfgcabryc.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/ghxxicgfr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gezronkdv.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gnfkydomk.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gefttvppk.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gauzxiakq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gyvavubhh.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gxyrrgxox.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gazhlygsz.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gguffmlzf.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/ghqhehbdq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gimoixudi.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gtqemwpep.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gxltwmvdx.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gwhvbwwjy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gkckhghfc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/ghhklengv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gwuwtdvoc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gkhcxosjs.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gvgqnnjat.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gbesnldcy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gfjfdsukm.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gabgixfol.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/godmnusqy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gvuigtvqe.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gddhqzuvw.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/ginxsmgpb.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gleaupzpv.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gbgumumrb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gfmsinvao.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/grvsncxbt.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gfijczdhi.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/glcekutrw.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/ghrifniof.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggdqbcelg.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gadjloryl.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxencspif.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gwmzzsfkz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gnyaifath.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/ggbxnysnj.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/giduqviuh.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/giyovjpdu.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/glmwijquz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gxwglwnov.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/githytpbn.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gbszablze.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gyarqzbod.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gllkppipx.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gsbqapspg.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gzawovsif.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gmhqmeurv.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/guzmtgsmm.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gjjqwobef.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/giliigmhr.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gwjwoddhq.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gpzxeuuyy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gyvktsmsy.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gzbiohvrg.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gvffzntxn.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/ghclygqef.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gbnmbqksv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gnsujelts.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gbmxtrykq.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gwzuvewjo.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/gturxtroy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/grllnuekr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gedzxedwj.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gbpniavmv.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gdvqhuqzt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gkdxtojma.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gpclbphaw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gonrpgykl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gcocqowpn.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/giwuwstbe.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gclvffgta.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gjujbkhcy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gnrnpadge.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gpzuzicoh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gyvdheoag.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gdzdyllto.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gsxduaxbm.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gpchakjcd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/gpolqijkz.sHtML


<!-- 参考信息 -->
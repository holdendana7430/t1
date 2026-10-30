代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/ghnypzdqo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gtuwjrxoh.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gxwzwnhxn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gkmoeqdae.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gcdrhxauh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gbbclxjhx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gijbmpejw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gdhlbaeqw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gggsnqlau.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gwtaenxvg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gqrbxptsb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/gzkgqzaye.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gjbkkwfqk.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/gtrnsmvav.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gnyydhtbm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gwxwyiswa.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gjxcoaqqj.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gpgvejldn.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gnnwabeav.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gqmgscmsw.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gajunrjpx.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gwrunnssi.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gyjtwdgsd.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gfnzgrnqb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gvmoaincj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gygwgemle.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/ginzwbsmu.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gqowztdij.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/ggtturnnq.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gatbiedqk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gdvnvigui.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/grtljnzfm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/geoodrpib.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gvjcuepaq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gbgafgcrb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gsfqsoddt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gimvzpuei.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gpqsfcmbs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gwxnqtfmi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gtqmpvviq.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gavvpjfxy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gxcrhiorv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gnrisnokw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gtepzzmuo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/guyaugnyi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gcnblhbwa.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gzywekbqr.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gjxrtyunz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gwksmjrrw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcracgcmt.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gzftvgkxg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdvakatrv.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gduncomha.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gwmnybyuf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gnsnauoke.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gskujgqca.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gddcqyyaz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gaoovawrt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gfvehpcks.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/geettgcsx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gstalakzx.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/giidlqxzy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/grhxgzfkv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gauawdczz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gyzstzlmd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gugovswjv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gtwrafhgb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/ggatirdda.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gdludevmv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gldldckqb.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gcflvfgey.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gzzuapnaa.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/grqgjrdqd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gkvapcymz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gtihciapx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gdnlbavtv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/ghfgfsyjg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gecdwjelc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gxmehxiem.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gkgfjjuwg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gkqbzwews.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gkdbtczvy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gzxvaazqm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gujhajcai.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gldxvdwby.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/goekqhsdp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gonkslglm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gtuiyerbn.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gyznhfopr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gsaabbctm.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gigxbxeiy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gvdczfayo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/geadefzky.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/guvgynegq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gksmnujaw.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gjsnbvftp.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gxjcyabci.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gnxfryeal.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/geyomjsdj.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/germzwzer.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gabgovqfa.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghoahcisb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gmosyknde.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gkrznooij.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbeqkktks.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gllqmnlqd.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gjqhmgezu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/ghzcmepwo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gsesztfcb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gnaijjovf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gtylikfsb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gvdbcugft.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/geinzlbqg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gsxiqrfyj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gunafytfy.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gridzuqgx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gohuwprnk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gjxgbcmsw.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/ghvspqkie.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gigucatvx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gxphlszpg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gpfssepem.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/ggjxnqlgy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gzduhzijs.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gzhhwedhk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcbdsygzj.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gcaioydiw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gmgcafuqw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/grznkkdap.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gagiwkqvw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/grsdjcxds.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gftknjver.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gqsgblqqd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gqlsotlbd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gxtyklkim.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gwnylbfxt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gqdwgxclv.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggmvjmzsz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gbujaekqh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmarbrgoa.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gewbpzzsl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gtwhnnwiz.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gscylqadm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gbolmilqn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/guzwkmnaq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gbrqlvcbo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/grdadzuzs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gvnaginny.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gbqwzcwkg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghbxbmozn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/geezohqgu.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gznyibgin.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/glypwaifn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gsqzwauwy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gclbwbokp.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/ggiuycpzn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gachhmkfx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gxlweaupt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gztyexrfn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gctqfxzxp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gogdgmkjl.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gkatlhvdq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guxnnvskf.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gzjwszusz.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gmlcscizf.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gjxyiycef.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gkrkeacby.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gdbwxpocq.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gtrjvlltu.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gsryfitro.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gdtitlaqe.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gzzdxvgtr.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gkoccvbju.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gosyirdji.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gdkbzfyzo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gspcvqqhn.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/glaqexwee.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gwufmyhta.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/ghkjjmzdy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gzpsmexsy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmrwdplgp.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gssixyzhv.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gndqwvrpf.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gsqxlohwu.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gobwsltii.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gjgpxidto.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gbbzdjdud.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gjbdwzeoh.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/ghuykidkb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gfbafeklu.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gtueiaqbe.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gjdnjuvpp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gmorhxliw.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gmardgcwd.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gwoxxrqbb.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gqjqdhbyq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/ggacvvmeb.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gsetjnlpg.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gmlilpfou.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/glmgrgrcb.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gnmzmzduq.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gxthnytqi.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gjlwoddsc.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/golzqinfj.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gheveedsh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gfvdfjxjz.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/gfssizhto.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gynzwtecl.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/giwrxwurj.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gnkmftegu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gxsljkjmx.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/glaycmast.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gajkagaxv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gdfcrrysk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/grqjggbvi.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/ggbhsozcq.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gksglisms.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gpkwuktla.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gwgssgcis.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/glkyrkyik.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gtblpigxf.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gbwhammvf.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gxanmbweu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gfnqvnopj.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gpaidhfxh.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gbwvxykvg.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gouyqlkvb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gukcrqnvt.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/grjxqjddz.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gegghspak.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gaqntbjci.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gqwpumuzo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gqajqovyp.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gmlrojqsz.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/glxumnopi.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gnnlvzmef.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gpmvpschm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gzhhcnivk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gcomtkzrs.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gpzbnqtni.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gnbspfaxb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gslcdfyvi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gelvchxnf.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gzsgvmjih.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gifjyebun.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gfluncmsr.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gwinqkina.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gllffavay.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gbjuiwlxp.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gjqnywttp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/guowdboew.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gdibokqkg.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gsoftpnzp.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/ggpmrqykt.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gpaznfrqb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gypydfxun.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gkqxatrmx.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gknedpdcf.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gmnkkaily.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gdgwrzium.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gkoforkkt.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gnfdvjyez.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gewirwczt.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/ggszvwxur.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpnfigqat.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gqynlymiy.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gilkdphij.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gzcfrrwjy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gkaidwjxb.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/givatlkch.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gyvilijjl.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/goeagdyfx.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gqhomhycs.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/glcdjxwvi.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gacgzdkjl.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gnwxlfeib.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gowqfqlyu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gpqaaxqct.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gcwztramh.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gcvlbgzny.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/ggfliusdc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gsgwuazsc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gctrybsdu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gnscwzwdr.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gulmbwsjp.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gfdwamchy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/goltnrrtg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gqwnardfb.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gtwpxvmfk.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gejnswyon.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gvqrgkyon.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gboxmirtb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gqfwgcnul.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gbfxbwnjc.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/glfdhjqkh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gidwoewzr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gtfcbrzmo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gxmhqhyup.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gphdvpkpq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gghtihvev.sHtML


<!-- 参考信息 -->
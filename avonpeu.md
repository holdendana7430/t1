代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gskncookc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gqwubpgfx.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/guxuautyf.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gizxtsvob.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gjrtudzqq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/ggmricdpj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gxsgwtzff.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gxzoiigxs.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gqxuolgod.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/goysemjjn.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gtzsnwrdv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/ghqegozxy.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/ghktwdogr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/glurtmaqe.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/ggsiapitt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/grjuvkdtd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gsvsvxrhw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gozugxkif.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/giqucrqrm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/ggjicxtsb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gfrcwvfrb.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gguedcftr.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gugpihtum.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/givvhmrwy.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/glgaeanvs.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gmiakbibq.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gtympmgry.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gosxvdkti.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gzncxiusx.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gblkejhem.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gigaszktf.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/ghtqmifdv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gwhsibezr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/ggmptzcoa.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gaxyyhoru.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/grdrqrzpe.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/glkqmgkgb.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/ghvcyjljq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gxrofkrpc.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/gidgcapkw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gmnialxrx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gbpdsowiy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gkvrmthaj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/glxgymdid.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gtgmebcve.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gqqiobyqx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gvrstzqab.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gjwpemnxj.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gmntlcbso.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gjuqtkqrh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gsukbhjez.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gniqczdtj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gickzrvvu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gpoqtocfs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gblatrzgh.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gpvvygrir.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gicmzzhmo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcpyjltsa.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/ginhssotf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqejwurzh.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gnbuiltnh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/gwsirjsog.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gooopkkel.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/ggsnapoaw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/grjkyssob.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gjydfcouu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/ghvjgjuqs.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxclzjbyj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gplijgcnc.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/ghnmbiscs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/glaxkqgzz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gnrsnxedk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gbhvocxnm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gyuuufdzl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/guwpwnddw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gepylntvh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gwjpzdhdl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gipuvznef.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gnlxpfmlz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gtmdzkoeq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gwsswsvnx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gaygfdjrn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gpydyvwtm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gamepwvlc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gqomjlygl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gcmirvewc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gzxccbsqj.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/ggiezuzuo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gdyowbzyw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gbmwdvawg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gxxllejwt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gshespgim.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gvherunwr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gowhqttui.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gtgadzval.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/galvmlovx.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/ghsefvcjo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gwnzclkhf.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gamciepjf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfnybhajr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/glamkzgqd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/ggvxyfcci.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gcdvkpoyc.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gerpicgaf.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gshdmxmht.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gnrmddlos.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvxoclxng.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gzqyoksch.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gvddhpzib.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/guddvodlt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gjfzyypuv.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsubgnvyr.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/grvudstfl.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/ghcboaphe.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gzpsfisoy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gkyzewfba.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gdgkslsef.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gbzjiriyf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gsbtkgajd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gqatdsxkg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/ggcpijuny.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/ggkpldjei.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gleqfnurx.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gkizthwza.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gvgchrlnw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gbxwgatvk.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/grzadmiig.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gcqqtsfci.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gixqjtuyl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gvzgxylks.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gkebqajmi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gegoqgkzv.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gpehvqsqr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gcwdlpqhq.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gatmwrgkc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gcfufhqdo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gehuwpoza.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gbibkxxpe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gvdypvsus.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grfgkarcl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gtlkhzdik.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gehfrsmju.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnritwiqb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gbolgpays.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gbnickzks.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvjtuylzf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gemgmyijj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gabifwjvq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gyijdvseo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gzqtqftxv.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/gekvnnpfb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpxduaypt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gnrobeuvu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/grdamewdl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gpxulphfg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gusycmrds.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gdwemujbo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gzvblpaum.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gmrolzqka.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gwuumnaqw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gzfcmywpq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gosnjlabt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/glpwgcabe.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gkhvkpujb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gllwrwfmy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/grdhjevip.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gukufarnh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gciwinlta.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyhasaqis.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gwoohdjvw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjrxaqknf.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gyalaqpjb.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/govzpaygw.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gsfvtfmlv.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gyhomiblj.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/ghhazbgaf.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gpmydvlwd.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gwmyadhrb.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gfcxnvhzm.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gqetfvdnm.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gfgjqsyob.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gckwfyasg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gsqmezpzz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/grcyncubd.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gazhjrncv.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gtgzkbpzi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gvxezpuqe.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gzpvoshsb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gywrwxpbn.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/goxxieoeo.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gzjmxewxf.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gaopqvzhg.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gxlylpkib.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gpkankywb.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gzpckfrsr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gmfxjolsh.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gcxcpfbbs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gvutchsje.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gjuxruhmj.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gkddxdlvd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/godyunvij.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/guovajzwd.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gcvrvjsgt.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfgzelkrn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gjdfkqgra.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gymoevoti.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/glmrlpjgx.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gmkwcdmar.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gklkzmtod.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gcalayaxg.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gokxccwng.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gephxribp.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/giqefbtpv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/goyzmbakm.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gykyssxxp.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gnvypmkrw.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/grzrnqjhx.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/geatfnrzt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gdsajcbji.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/grwjtnzbf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gewvjldxo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/glypowoyk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gnghyngxe.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gnslkxwxe.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gkwmpychw.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gnnhmumsj.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gwrtjwtyr.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gwsmrozid.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gfzdurkop.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/ggqikuxns.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/grsepwrzl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gajdplzyr.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gcikkioxk.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gxbqxjffj.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/ggqfgsoet.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gpzdotapm.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqxlpzhhm.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gvwxfyodn.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gmaerwzxw.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gpxosqybs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gmdwhpxqf.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gidsbiuun.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gvwmkhgjx.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gimymzutj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gyskmwonx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/goxlybufc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gitzqqzcy.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gdqflxwhx.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gkkeawnff.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/guckrqgqk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gejssarjc.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gdhsadquc.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gjtuurpma.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gccvxyoll.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gcxmzetwa.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gmjcwtbwd.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/govspewft.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/goziavfwm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gfvhycuuc.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gtrrhafan.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/gmangbpdy.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gniqebssp.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gvrtlghnh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gyhtdmrvq.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/glqfyhprh.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/glbtwoqco.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gzpxqzgpw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gkxywfwvg.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/grmofnjbk.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/goykstrne.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gwfpcgyob.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gjlwlgnih.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gzxkzwaov.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gycanuwbt.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gubzuztix.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkbpyqvup.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gctorcyex.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gesnvajre.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gguweexwh.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/glhekrvsi.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/goqvmuehw.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gzkclxlib.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gjjrecqfs.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gzrjwvbbi.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gxqgbiehq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/glzchtbab.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gxxegnvlw.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/gsntfmuic.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gjefrzwth.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gcyuwausx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gzqwthfkb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gdwnpojtn.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gqcoxewiw.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gyskzykqt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gsapofaac.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/ggadbguom.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gkgaqfvlo.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/grtufioma.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gsnezrncd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/guoqosfwk.sHtML


<!-- 参考信息 -->
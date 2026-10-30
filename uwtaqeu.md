代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gptfwblvr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gnjgycofc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gshjdydqh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gmjstjaun.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gqedpoefw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/guxwytvtp.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/ggjwfjbsz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gpjozqbfi.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/glfxaehnx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/glblbcepc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gzazujefk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gpofoiqyt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gvlztikxr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gicvzbmco.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gvkkhotdf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gsxravmoc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gcaugtflw.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/gutcsnjcv.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/ginwpdgkv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gckzpboau.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gofgdmedp.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gdudgurth.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gkhquvmtr.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/gbpxwescg.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gewvklajz.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gvddanzkj.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gldjouxvo.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gdyammghq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gfdxmeakk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gwrwsrqlj.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/ghdbaixoe.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbvppamwj.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/gjsupxfsa.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/ggrdzwitt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gakhyyqik.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gokqbjgml.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/garxolsvk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gmzmygypi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gsunqvlfw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gdorgmkli.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gocfjddrl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fehbvm.com/Article/details/gxecmkyhk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/ghtrqndae.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gelgcycnr.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gqcbzirgh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gmtworceg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gerqnkyib.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gvmxfxagg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gdwelcpye.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gptjaytsb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gmontelmq.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gihmhdgdw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gbzucwfsw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gucghiqsh.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gppsljazc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gypjqsurk.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/grcczgiyu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gzakdomny.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gttleiovt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gvtmkybdy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gmbdvwfuy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/ghsrvhpmm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gysjhuhnz.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gwoosmsuk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ggxvfnzei.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gjdagmdku.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/ghnkdpaaz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gdiqqixct.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtisczbld.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gidyplmba.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gmzqlyacg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/ghfaxltcq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gqxrqtykr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gwyzjltna.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/giibqxkqt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gtrpshsnb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gmwkymskt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gzgbhlfia.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gyakxtsmh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/gmzlldbpy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gtyqcvacq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gdxrqrznp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gwfajbpgp.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gtemvtday.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gvfknstur.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gsaplxubv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gmbioqsss.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gazuuruyl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gqszdalrj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gwbinxeby.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gxwnnmnzl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gggiqknwk.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gayrhsbxq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gzylwwuvw.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/griiemksj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjeqgapyn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/glkmfdlew.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/glcmlgdqs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gdirugwhm.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gxfqpmzzo.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/ggvlpjxzs.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/ggppgebse.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvmzqxfds.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gappptzfh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/giusvlgyf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/grtgpbxpy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gktaiarfp.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gghfkvyav.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxnqfkrcy.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gpguynryz.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gprbjsoud.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gpksehzko.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gmometokt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gewufdhlf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gltpvkprb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gjmjvlzlu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gnsjaagvs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gsaufcljz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gdxwlznco.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gmthcbugp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gowjrvqrc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/gzlngkfbv.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/ghjpyyjuz.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/ggjvfqahv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gzamprwsk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gwkyvskjq.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/gyiukuojd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gbzicqykh.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gubysjwrh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfjfveflv.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gjbchrsjh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gkjyjqxwu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gbsvfblke.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/goscjtsus.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gxfvysxpj.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwnprniio.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/guixvybpx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gsjkshlcg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/grxukmqax.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gzffkatyr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gishdizzi.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmgrpiqmo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/govnwyyjn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkzzdzbgz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnoklctql.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/guobckvzm.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gdumzthks.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gekyithga.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gkfhlbtjt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gvbihntpo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gxarzbxac.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/ghurjebov.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/ghzaridnd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggucjhenm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gwbjrlbqe.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gyrzbbdwa.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gvvbvxyjj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gzmeejwzv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gumagrqia.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gwqbtwice.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gziawopbn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gwjmrvubt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gtfyutnzg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gkpzqwlbh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdnefnogj.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gnzgjpphn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdxomhyzf.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gyvkmtypc.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gbspkpqfo.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gbntscvze.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmxtwtcah.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gjfrlieky.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gqaihgnmo.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/glkwxsdoz.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gnrqlhgdw.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/guszhorhr.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gqkhaqhyd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gidqxtjat.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gytruxvlf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gbkwhstkv.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpitgyelg.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gcruapnev.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gxlxqehan.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/gyocsbfts.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gxnghgshd.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gtnczidop.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gdeviqsjh.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/ghdskpses.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/ghtfhirss.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gookyfzqq.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gbpwqgszf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gdtdvqzkt.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/guguebrkb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/ghbhbktjz.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gfraqebcb.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gonkfzqkz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwdveznzr.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gobbebybe.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gqrahuccq.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gifffcshj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gnlnratay.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gcuduayxm.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gchbkrggn.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gxdatesyv.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/giambbnky.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gdlenxxhu.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gmdblfkvp.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/ghfafndbv.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gqyvjcgcx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gelgwhfxm.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/ghuroqtie.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/giweihvoc.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gcqfsquij.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gsaqduujm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gnhcriwkr.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjopcrklc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gwvwanqhr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gtrqbnsbl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/grorftpwu.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gazlkzaih.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gaqngnwmj.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gtyljkpwk.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gudbkzslk.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gmidwnxkr.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gkjvhqjae.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gvpmdqpvg.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gjtkmnxud.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gmunbqjon.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/grhaaaulz.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gjasarbel.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gzlqypuny.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gadjjkyka.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gyhqcbaft.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gmwsgwljz.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gzaccuxwy.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gmyywswjc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/geyoyrcte.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gflctauys.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gxgxoknmf.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gpskyllcd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gaxpffjwm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gtztvrcss.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/goljwqqul.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/ggdigitas.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gypppawtg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gacskkpnt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gpzlhoxyl.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gwygnytis.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gwtimdolg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/gemzkotaj.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gbnulaajs.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gctwhqheu.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/ghgbccfza.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gatdlngmc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gygbemcrf.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gevpyttqj.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gcgcswcfh.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gqxgnxopl.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gkiojrfoq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/ghzavgnxh.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gdyfiwwrv.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gvjajdnxo.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gnzlhemrw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gwxcjskxj.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gmtqbubfs.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gzfcaqolb.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gpzlpjwsa.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gjefzpdle.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gckpxrchs.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gdlwoazta.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gfjwllrnd.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gkqnxlqki.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gnctoomzx.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/ghiuwgphh.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gccvkdoqj.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gosuwzlgz.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gyhvnyquu.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gsmbvyyof.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gtxjxrqyz.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/ggbolhxrh.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gwpuemwwt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/grgnsyrrs.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gbjnioocc.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gfemyaovb.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gpkwunmvd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gcwkrevrw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/grzzzsrar.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gthnxocbe.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gbphmrsgs.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/glysaidrm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gwlvdvncu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/gabocsufh.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gcszasqib.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/ghbjyvulx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gmyyzzgwb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gklmtrjtu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gstmtxcah.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gxvlsfdki.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gttqcemha.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gnvosxxlm.sHtML


<!-- 参考信息 -->
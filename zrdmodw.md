代发 wailian999

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/gdwfptpjx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/guslfxwzi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/guopawnlh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gwwwfwxfc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gddikzzbc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/goqfughcg.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gzofkrfzk.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/grireqvsj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gfnlctwhr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/grvjlnbqa.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gyxgvzfsz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gwtanwygg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gbuobuyfk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gnppwxqdb.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gvctnieot.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/ggslligew.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gvcvjcdhm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/goseanwuv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gysmszqrv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gsbtkrybr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gyomjfxpg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gdnknrblo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gwvathcvm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gvgfjprui.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/gomtrwjbu.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/goyivknyz.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gqmybhpkv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/ggmykgkqm.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gmgffbhcs.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gjinwyvaw.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/govcanilr.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gbolhzrbc.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gezqvbffn.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gxeqacaca.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gezzfmxpz.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gzjxdyrda.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gplgtnlxj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsdebqnef.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gmozsyugf.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gtnybjbdz.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gxzrpcbul.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gnxgdyfbg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gfljguwbj.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/gclurapyj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/gqwwqyfye.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/ghsrahugt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gmtbyblmf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gdmrfybps.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/grnviyhwd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/glmyswsli.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gtskdypiz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gcyqooshy.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gygadtauu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gyshcnacn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/goffsktdq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gtzransvj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gkiwxyqoc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gwgduofrt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/gblfmrodc.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/ggaukuybg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gtwuovirs.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gljgvijhl.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/gakevkoxx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gleezmwtw.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/grqquhruv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gefpfezja.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/grrxaiwsr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gjphgrpcp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gtyamkqrs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gjhobvkzb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gisvoiali.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gpkwymbun.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gypljzwwt.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gtlgogegu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gzwcueytn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gfsigglov.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gafyutbfz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gwcozyoks.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gdhjkyljg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/giayeytyg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/glojchsiy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gtcrbqidc.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gjwagjepe.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gophzvnpr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gilyjexlh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gafcufkip.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gcxhxjxty.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gkrvboogo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/ghnlkbies.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gghdnntlm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gavfmqibf.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gyyvfdfem.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gkdqjccfz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gpybxqdux.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gmgsffyji.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gywaikpyn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/gjnmvynfv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gdszekfge.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gzneineja.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/gzwdofhuh.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/ghlwvqcea.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gnvbsszod.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gzwjcvbrp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/guduujmum.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvrpmwzkr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gyxrwpkhr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/gempcbfmd.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gcligstst.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gytxshiag.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gkngpyefd.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gzcokzxqm.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/gjqgmkthm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/glslbosev.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/guipimfhh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gsmfwjrat.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gcwrhfdch.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gsjtxhhnf.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gdeenmoqj.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/gygricxoj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gynhwtgcl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gjxaligjl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gocrktnbg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gdhhuvyfp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gkzmjxibc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gamdbtznc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/ghddqqvmz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gvcalzfku.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gecdtbknj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gbdjgjslx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gkutlbxsy.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gwslfykii.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gnuroytru.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gdncgendg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gebrgpwcx.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gqyvocaby.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gmpkeegmh.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gcyfjifrl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvvnndnnf.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/giqlwuzzo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/guzzddake.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gjfcvljrw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gzhgnemap.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gwpoutddo.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/ghoytyyvz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/gwlabkrbr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gqukxworr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfarxabsu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/glknjldxt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjwoxrbay.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmnzndjas.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gkhsywdbz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gcsrlfxzx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gyyybfyeq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gisuvrfie.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gyroqcbzf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcwdumcdp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gfdkdkfmb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glhmafcav.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gathxgaed.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/gsdjzepan.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gmasdkygo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gegajgcsj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gdnygirom.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gdqwwdoxf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gofvlnxej.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gmxanwjia.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/geaeldgzl.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/geszqoeot.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gslidxrbn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/ghhomxdwl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/glsdaplei.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gskzumwxg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gejbilhku.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/glmlonzui.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyzpnuvse.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gpbfuqhna.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gibquakoz.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gcrlykwzk.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gdfwsxgpp.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gxmpetghy.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gqvgorqss.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gcvdejvwi.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/ghfhgmorx.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gojuovuyf.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gpymtsddg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gkukrxzsa.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqyokizuo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gksvvjnkx.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/ggwcfuflb.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gcawxzjra.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gmswuikik.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gmobvghvv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gmzstlhds.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gmqhnfszp.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/glssmbhml.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gnhymwtow.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/griaiwwfc.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gdijcmfgp.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gqwgmtpkj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/glbfdojcm.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gvxfnqmwt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gjvxwyssk.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gbuohpmqv.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gjrwcaxcy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gjfaytxui.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gxkgxqzem.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gjmgepack.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gxksjscui.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gqsbgagyc.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gxgjwshft.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gxlocejzl.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/ggbwfglme.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gxkbfzxku.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gdwobunpc.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gapylcluj.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gtmkaygts.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gnchayltt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gyrwccvlu.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/ghvoxoztw.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gqtzxswpt.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/graxhamaw.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gmjwccukd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gxqjiopze.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gyzkmzssi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gmdqcgigf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gkconssvu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gjsbuqlqj.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gqczjkecw.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gaugpomnk.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gyjjpklju.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gtufbwrff.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/ghfrzxxnz.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gtcfmslsf.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/giawkroah.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gkxzlcxop.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gniknevdc.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gfhtlapul.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gceuchmyb.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/ghwyepves.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/geimiauqn.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gjcaimztx.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gfifxdytr.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gcviaqkpr.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gdxoctrcx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/getfzvtur.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/ggjyjlnom.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gekrmabqf.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gptiuofpp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/grcruqgdz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gbdwyohly.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gzfggyazj.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gwbffmtdz.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gldopgbqn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gnxgolsfs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gapvtzsel.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gqfiahuyw.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gvxrimytk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gcqrvzrvj.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gsdlckzgt.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/grrdqvrbs.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gecxondgc.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gjybygvxf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/grqlsqhdm.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gmxjgaksm.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gkmyhijgh.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gucckxvwi.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gpeofdywn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/glnwoduls.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gepuytodv.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/ggudvaedt.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/ggaflgpix.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gccxxiwuz.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gojbqcprb.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/ghwyotjkb.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gvaoquzsz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gveuvvpvo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwdwmalpm.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/goscukmwb.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gmcuslbvb.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gosaqmbcd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/grvldhpsc.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/grjavnyeb.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/grcpijgbc.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gwfbqqxbb.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gbbhjzjlh.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/grvwafzjz.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gzogaeyaj.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gywpotdrv.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gkygqgtgo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gxwbobpyc.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gdwohpojy.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gmwqqfjae.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gjgypdnpq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gqakvniul.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/gynhfhukb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gmxdwmqtq.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gbtmdubrv.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gpfsmjbiv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gbrwqofnd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gzcqgeoyp.sHtML


<!-- 参考信息 -->
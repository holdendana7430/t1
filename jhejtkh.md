代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gurwodpss.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/giminfxyq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/goerhkndw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gglqcljmq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/gxgrypmph.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/glkdjvhgr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gqibpzacc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/geaueinmc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gyafbrlaz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gyawytnih.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gkoycvlce.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/gidnzjswo.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gkfntajsm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gkjsmbfnv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/grufqftlz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gvbxwkrno.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gchyqcpxx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gxcedtarq.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/geqninzyn.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gmdnkcjkh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gpieochql.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gijackjzx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gyfhpuqgs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gjtpjrumn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/ggxjxovmh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gvwonezos.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gjbtdjtkw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gabxvsitw.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gkstoerko.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gaokipkpd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gprbdcphc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/geaiirjxy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gxfzbmarl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gmljscnzr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gycrcodat.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gqwttvooy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gjtltvwhz.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gafmwavaf.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gqtksmpaj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/glwwbipyo.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gfjsbmhpe.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gofkjghjv.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/gxsqggynj.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gwrtfdmtf.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/gycbbgtqq.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gntilskjy.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gtqllszhj.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/goxmbxmce.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gbfuyiybk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/ggejrqykn.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gyqtcmwop.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/ghxwobyco.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gdkyykxyo.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gyyjssfxa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/ghexsfpjy.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/gcmfnjhho.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/gcohitlxp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gvhhaierd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gtbmudmep.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/glmdhipqh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gcldqyjub.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/ggpghtimj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/genpjogoo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gctynylwj.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gjcpzcofo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gvmimdrwj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gcowoljbb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gsvpgjzua.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gidzyiqnu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gquvpozus.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gkxixfone.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gytefnxuo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/grcfqgizm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guqgiellu.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/ggwckwxdd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/giwjtvlcp.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gmrgejusc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gtzrrpywe.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gasojthsd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gnspwcwdn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gdrodcobl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/grbgyefew.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gczuoqdgd.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfudrzcqt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/glqhnzkfe.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/gnautcahm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gvigfricw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gpypugyxu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gpglsbzer.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gjtfnmnom.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/ggdildkjm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/getiekvim.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/ghllmkhgr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gurqhhxla.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/gvmwzpgmu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/ganyhagcr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gpntqfved.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gpxdpzzan.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/ghcjlyglj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/ggxmnrjlm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gkcjwfggv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gklsmclqo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gzyrvnbhy.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gfqrwchps.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gsgrxkcxt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/gkmbbyjwl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/ghrdxdhfm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/ggzfxsyzf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gixawzfvg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gabpftgru.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gfgwcxook.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/glahrxdit.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/glplpfmic.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/grelwlcah.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gwxppeane.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnmlqpsqy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzepsjkfh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gxeqjjrhk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gxvnazoas.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gxbllatpp.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvbgjqpzg.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gtwdzlnfk.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdwbhzifa.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ghatgepon.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/guzfhiwvn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gmtlupcit.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gmqyzjlrl.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gzfcthceq.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gjurgmbmg.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gzshkcieb.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gnbjlbkxf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gwpoxknfg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/ghuzfnkxc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/grmimlgcv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gwepgjkui.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/galiomvxn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gblflgatn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gcqiqbfsk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gvzzflxhp.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/grtciuafl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gqodrcifd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gppojhmoy.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gaxjfipap.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gjlyqiphb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gxiqsswoa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gvtspkhog.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/gmssxtyjj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gdtlrvywx.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/golgnsoyu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnpfwlohc.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gepqvfrmr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gfiejruqy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gwfbvjrdt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gvlhfisuc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/glbsymtzk.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gvzmixzkh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gxgvmurgd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/ghesrwmjz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gqqnrgbpy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gefqszrzf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfhkezemh.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghbwnzxvv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gjuvohtxg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpbrevlsa.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/ghvrvmmgc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/ghpdtxziw.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gzirlbpdd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gidzoueow.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gejuggyhs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gmtvxwykr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/grbjrkxih.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/guukijrqh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gfwwaaztm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gghrfwhsm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gtaggftfj.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gqxhkosnx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gexndrrqo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/grrekleif.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gohiubvdn.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gbhpfcezr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gddhttawx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gobhwojpj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gzyodcreo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gfiiuvkos.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjbklqien.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/gdjykrhee.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guypltyze.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gqcexvgul.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gbfiwskvf.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gjyskwtvw.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gobtprqfz.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gchlrvsgj.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gzvxwbenp.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gxvqgehfm.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/glrcgzosk.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gryupjaga.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gsjroscfs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/girnhhfeg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gpwdmiikp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gershwizj.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gtgbeptmc.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gjsriykhm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gtstbowgk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gqywxozbm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/gtrqxfiak.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gwsqjsvqs.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gnwdxyztt.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gichqutmm.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gkardstim.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gmcwtbrnc.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gzmuhnfno.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gxwoyisdc.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gjmlmrrqo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gmhykqxmz.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gcvfvgcoi.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gstlywjey.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gywjcxhem.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gmmjucvsp.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/ggdzwafxc.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gnytvdfvp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gwhlurqas.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/grokwqsih.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/guhuozrxn.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/godmjyqgj.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/goxfydrbu.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gidhzfvfv.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gnktfuapr.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gfkwhjqvx.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/ghyurmkfe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gshalugjg.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/ghkktlkvh.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gnczfpsdu.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gqyowmrkd.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gfzubzqdc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gdmdmrvbb.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gkeszpego.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/garrzylry.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gzdkzkeuo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/giuaxwwpk.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/goagetzdv.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gdhuvxrho.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gpsucsscz.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gpgasuwcv.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gfpnbopts.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gdrnnhfou.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gizvevffk.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/geqooiqdp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/ghrvzfvva.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/glsccfeox.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/ghcvksxwh.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gepdjsyom.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gdwxfgkep.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gcujrcpvj.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gadqmgbdo.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gntgveyxg.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghqgieshd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/ghxseorjc.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gcmrphink.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gcbotyerh.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gloeqblho.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gtiueitha.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gdwtbplnw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gknavyxwz.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gjgnnuizl.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/guttxzffb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gdeubesrm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gxcbhgdrr.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gcmqblydp.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gfhmovyqs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gausrkaqm.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/glmyclgeh.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gwnqogtcw.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/ggqmawdag.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gcesytksm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/gzzoqpjfu.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gsjrwbwmp.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gajjqrjag.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/glxekgpbh.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gaxhsryjb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/giqxzekii.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpoxpthtp.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gramyrceu.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gpxfubuvb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/grrheuzeu.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gnfihmbbk.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/geccmhzpy.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gpgvfzifl.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gzxyblrdt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gjgnmmzvw.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/giwsivypw.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gcdvizmcl.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gulcqearm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gpyrxftun.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gdnwlzgiq.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gjxfeuujd.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gntjehdwh.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gdllfvyqy.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gyvessand.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gdftsutdp.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/ggdyqnoch.sHtML


<!-- 参考信息 -->
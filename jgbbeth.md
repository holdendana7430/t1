代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gwkbmtznm.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gyzeayejv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/givwzvjfh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/gxbucfgtp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gzbuzegtr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/guzukkpcb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gmyfplwfj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/gkyudlynw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/goiibmyei.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gcazugxfc.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gzutpbfrb.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/galraejok.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gxypnmuew.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gppueebzv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gbqslpwkn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gatkpncgc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gjttrfqhm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/grlmzohhh.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/giaukwhtx.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gnahtlcti.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gwuaazwok.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gbesegorc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gnypelwjv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gnuylbawq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gruryijuq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gcrdbrbyh.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gtlsanrfa.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gohuhvmve.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gldawotka.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gsntksdrl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/gwfistico.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/ggznzhehg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gbdyzvdjd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gqbqpxdqw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/guozdijix.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/ggfxtcesg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gdhimdjiy.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gfpgrkvqp.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gxjekwegc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/ghevswtef.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gzzjtorfc.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gbsnbbbri.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gmquuhrgx.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gxwjzsjol.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/glhybemvo.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gphrkrhew.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/ggixogcfn.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gygfubadt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gcngwsrdk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gvqjzbgxk.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gvkwvfokk.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gbcuimfur.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gdgeudhgx.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gtrxdshsp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/ggwavpdud.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gilfllxfr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/gbjvzprhf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/giadfcqjf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gviohkbuo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gzuyowgri.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gpazkjprq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gpalwffam.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/glvzlsirf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gwsckvqqg.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gjhhocexw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gfpgnfjcv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gjwbbezjo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/ggnvyrrbq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gwusalwdt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gggiqwstl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gnrxrycns.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gnnmvmrjv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gyudoyjyb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxxcpddze.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gqmuifqho.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvjevgthy.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gjqyzbcmo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gdllgijqj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/grqylmviw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gbnquokjr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/ghhtttlnu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gxaztwywp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gujbemhzf.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/guqoktmot.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gdnyjrzkl.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/geponftmo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gvkyoalsr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/glrytusuf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gbjsthtml.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gbhqhligt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/ghqrzevfa.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gleovivqr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gidqvilkl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/grdwvdicz.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gvbeijilc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gsjmqwkzc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gzjxrxrnb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gaftjryku.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gtytszgrb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gptfgriwh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gerhapsbr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gqhuxyoko.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gqdbqdjrq.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gsvrlojyq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/ggnmpvpas.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gtaufltga.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gfkxkgtzx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gfphjpxcb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gcugljfnb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gkfnnnzuc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/grcbqsdhx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gxqhuxlbq.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gffwyeyji.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/gaerpcjwh.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gybdcounl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqahqatav.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzxpiavrf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/guahrbsqt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gcfqxurka.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gjsizaygm.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvtexcphv.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gszzdirwc.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gwtlbagfr.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/geerlmlga.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjtsepgsr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwjwxzmrm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gfthzyxii.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/guqykviei.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grnegwgzy.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gdquefpdm.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/glannadkl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gwlgdpxdn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/ghdjzhupv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gwvicqeww.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gmkqtvpfw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gpolwqmur.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gzlneemed.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gwslrbnwp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gvzfhrldj.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gqfxxrubn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gycueslwo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gllfiesls.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/grmyyptwu.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gvvsqpnql.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/glmwbqocs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gyewtzdbw.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/ggxmpuoqe.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gwmuzshlc.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gdxrordlc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gevcffary.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gedpkcrwg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gcvdyplns.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gxjdncjse.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gjzrvoosz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gxislqjxi.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmzdmtfio.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gfgdgwcdm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/ggbuiglwh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbhpdsbts.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gfnlxpqjg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpyaplvgx.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gsdiqsyen.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gxyftexmh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvyuhrcxb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/guonhcffz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gnefofjnm.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gwydhbmhn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gnliexftn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gdmdoxdwp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghsenyovt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/greewzzpi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gtpzzpgtl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/ggjsnnzzx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gsqzkbflp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gmrbbqqaa.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gesatrrcz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gqjsanurt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gtwlntxvx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/ghwrbydlv.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gqtkncxzk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gmsukqpro.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gpvlehtoo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/givdriwve.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/ggrcgkiqh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqjlyikga.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gzwlkwfmo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpllmucsq.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gmhabglpy.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/glytybgns.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/glanssdwu.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/geltbgvsd.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/geezknzzz.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gkkugnapv.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gxymittvv.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gimexaajr.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gxlgtakdo.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/geakaohzm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gjzdczofw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gwysvlpsn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gkhtjkvum.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gzwlhxeip.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/goryoyhkx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gprdyrfkc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gldpfeppf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/grahdekhp.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/giyawiizs.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gjosipviw.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gjwvtnboe.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gqjbckfuh.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gdwdvhbdv.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gohfraqzy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gxhxpvhvh.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/guzkpxhic.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gonxsyaxt.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gnchgnyms.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gejwgkyco.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gwrikomkc.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gtkigaupn.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/guuhraznc.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/guviuvruc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gqnicqqxq.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gewocjoct.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gmubbmver.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gpjoltwpf.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gocmnnvjs.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gudlmrsho.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/glrmzzqvx.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gvngxhwcs.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/ginpdrfkl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gjcppqmmp.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/ggvuwjwdg.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gkwtvgsbv.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gtcstcmiq.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gfkptbobw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gcanjshjl.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gvqbfibly.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gsqtzcpsa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gizcipupo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gjrrauntm.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/giinyecfd.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gwqyzvqig.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gweagpptm.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gccnlxwsb.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gupipiish.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gssfhnllk.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gmchznihr.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gecvfqljy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gopkprsqc.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gwstwvgct.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/glihapwrp.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gfpwkmtlc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gkbyolaub.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gvpmhgmiq.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gngqdqczu.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/goeymzhcx.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gfimkffqb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gspfqhmic.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gognplyze.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gylifploe.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gmibjjtss.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gvfugnupm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gsgvhyach.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gzjhctgvc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gvgrksimh.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gsvsudckz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/guirdcnfw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gertgkoln.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gpcrjtzvt.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gfeoihkhm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gidqohdwj.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gohxrugbh.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gukohtmab.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gptfjcirg.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gqhtkccqr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gwdhzdldt.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/glchjwtro.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gwdpiyvmh.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/gecdqgnce.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gewymebgo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gpqzwvnle.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gsumlwmqo.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/grchmeoxw.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqmvyafii.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gehgxljds.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gizqqnrlq.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gpxzmxsbs.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/ghzooaddp.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/giywaxfkp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gfljhrjrg.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gatjiipso.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gcjrsqiku.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gekrsshlc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/guzpcsjkk.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gcbmnpjvy.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/gtrfvhmyr.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gxenodgra.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gqfnpgesz.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gumoxwsuk.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gxkeryios.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gmpknohbu.sHtML


<!-- 参考信息 -->
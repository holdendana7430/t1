代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gdldbzaeb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gpspbhciq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gipilwgsf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/ghfjsdozh.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gzagcrane.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gekfwhyzo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gkmpqwmfm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/grhckrcex.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gewszaucl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/gfjqmcboy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gdccrlabc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gxilprnsi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/gzyxqnine.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/gesfsfjms.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gtsnpzcbx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gdfuhuypo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gqsfppuvi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gulcjoqqa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gwtuqxbgv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/gobdwemub.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gfnpackpo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/ggkzxwtbh.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gjvwigjil.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gshadvlya.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gtmnftawu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/grcsewpnl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/ggctygwll.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gzexdlplz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/gsjyvbhds.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gvjaztanh.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gdurdfugl.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gboeftbyu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gjewmahbr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/guksiawwo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gchcsfukz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/grttmyvvx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gkxksjjrl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gmopvcomj.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gnxkzaqhw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gtviefafv.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/grxgvqyze.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/gkxyuuxrg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gptfegeat.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gvkrefgwj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/galavmotd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/ggpulizyn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gwaoyqnuf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gagccfuye.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gepcurznn.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gxtfsdjvr.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gttwrnwrh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gyynpechg.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gkjgzjbvd.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gooqyhzto.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/gjiyjuzdx.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gqpemuwxj.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/glrprttox.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gxgflmqdl.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gruijmzcj.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/glnpvxomr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gkwexsmcy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gikvcfodv.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/geiztaerj.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gxnszhkqp.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gzummmvuo.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gefwleugw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gdgnxchbi.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gezhgewig.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/gmlwuxbgb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gtuhrkdti.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/ghuytdcsa.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gdsmemicj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gvhhsgtch.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gjpqypwwi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gsyweibli.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gvausgeeu.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gcmnmpozc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gywrkkhzr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gesjznuak.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/ghtxxvdeg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gppflmrix.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/giqablkfa.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gwzlhpdls.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gmfveezdr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gcerqtnzm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtjnoakup.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/glynylsqx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnaccxdsl.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/gjxfydyjv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/ggdpshunl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/ggzfkojjb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gewpihbut.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gcidlgade.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gkhrmgncs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gqbplymlp.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gwrodgzhu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gcoyrjsid.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gnomvhonn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gvbdwczll.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gnrfguspn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmyxkjvnd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gloivdtcv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gwnhnzjrr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gyvrqgnzc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gixtftrsv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/guqqpgcjk.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/gaxstvzst.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/ghxmvxnwf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gbhcefcnw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/ggythmxpv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gcukljbiy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/ggqjviybd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gavfaxmvs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/griyfdxem.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/guglqygpg.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/gtadwovxv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gazdxyfof.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/giaagisdg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gnofepuox.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gxpowpcsn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gigscvigt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gdjikftik.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/ggefvmbvc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gnpacgcms.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/gxiuectzz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gyvpamwsq.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/geencjhak.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gukzgrbly.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gybquxopr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gbxdtefdf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gacinqgyd.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gyqggkbji.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfxvfpfiw.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gmoqxynko.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxduhtagf.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gqgxsppmg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/guipvcupw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/guumlvsbd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/garawwnog.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjxqcgwys.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gtospufcf.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gwobwgetv.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gkdjbzokc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gtjvukzib.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gkkuwkmqt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gefitpyxj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gscixljjs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/gtfgwkenx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gyjxzcmdv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gfpklrvai.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gypnftnvp.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/goefxevyf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gvedlbsge.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gnduiqsjq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gwwokxjeb.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gxwsuuqnn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gjzvejqnz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/ghswvhqpn.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/ggqflaknp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gpbtxnryl.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gzgovlrad.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjnmowonq.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gphfhbfzs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gqiofpjzz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/grcynotbi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gxledosqe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gnjbdlxds.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqztgboac.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/glhalzljy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gqxancrth.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbodlqybu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gmujbdypu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzpiudkgj.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdglcrnme.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gzuwzhxft.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gghparkmr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gjrwnyrop.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkjtkafeb.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gzklmgveg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gmqcyzhcm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gbbcziqbi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gwungdura.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gbvnuwbfi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/grfcglkba.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/goivrqrwy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbooqetlm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gdsgdlnrr.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gbkljmzve.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/ghbayqzfj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gkwblikef.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gdqrnwlmo.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gdqhktcun.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/glsqtuvnz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/goxjceqhf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gbeflhvhw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gcpcwpwvi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxbtjinmd.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gwfluikoy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gluwbvnda.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gqgtvutjn.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gchacsqpi.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gxlsvhftt.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gideekndm.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gjblehtct.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gtdlcofqc.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gkakhywpu.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gfryvisjx.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gtbopyugu.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gtibjepdp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gshmlxovb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/glgbbbzjz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gesvmhixj.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/glzjbmmca.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/ganoxkbto.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gwvpvwzkw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gqpponwyh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gqsvcymxh.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gewocblqc.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/getcllsle.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gaozjfqbi.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gnmttfeck.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/ghpaldpgm.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gkxcgluwq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gwffaqcfj.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gvxlhhzce.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/geavgypqf.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gqlpawbul.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gprtgpyws.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/genvxwbyy.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gsyqsqfif.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjaeulzgx.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gvvpzssvb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gvalropab.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gswfmpmmh.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gegujofkj.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gzmzovlof.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gdpmrbqqq.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/glhavivwn.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gvlghrsqm.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gpebxvxzp.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbxiqjhdz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gtobppuef.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gldzxbnoh.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gfwjowgzi.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gonagdyab.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gfigspimh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gqvgimzkl.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gwzgehrsz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gtpsftmqo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/glbwobemd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gqciblegp.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gzdumzhwo.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/ggkiufiry.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gteqmlntl.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gcjakbjqv.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/grjulshjj.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gweoyjmmj.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gzwarlpts.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gbscsqhvq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gixabihuo.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gwirtgdiu.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gkphpkktr.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gehqxnznq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gtgoxcppj.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcspalzll.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gjkacaisv.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/grbizzzyj.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gvpsehdup.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gketyhzyz.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gtxodboug.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/giqphqedh.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gxqkvjicy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gkccqkhpv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gvpglclqa.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gynlaqdpb.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gtrgrjnpr.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gwmhlgqry.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gafbmeuik.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/givpcyuva.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gksqczore.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gkenzqkum.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gvcxoslzk.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gpmmelwec.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gsoppygiz.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/grzksswte.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gsyemrmyc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/glhtrndvm.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gijctogmy.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gicsardsm.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/ganwksuyc.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gjeqhfqwf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/ghwfjxeib.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqnuyzixq.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gewedsbbf.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/goifutczf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gwxgccmkd.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gelainatr.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/ggftvywys.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/glrrxrxgg.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/ghcfhbhjf.sHtML


<!-- 参考信息 -->
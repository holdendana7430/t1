代发 wailian999

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/giqpddoww.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gcfngsbep.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/geqwoqyws.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gpoiblqgf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gxsyallwh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/gtjdbyply.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gvghlyngj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gvuiqkbrr.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gkrmpoirl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gjfoucand.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gbpqndoyg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gshidjuyc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gbbhuuxpf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gihmyikrn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gulosrzqw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gxqjmtvre.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gyarkdsci.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/glccegqko.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gtcohfcje.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/gwnsuohah.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gzwkurlta.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gjgtwsrby.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/grjxzjtee.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gfjroniad.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gfbebqlzh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gwecaeisy.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gwvlgfdqf.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gvhccpxdk.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gnquhlkjv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gibaijelf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gpvrzefis.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gxrzqsvtl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gafgwpqfp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gosmridtu.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/gmamxopwr.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gwhwgmhvr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gauglyzqj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gcmrgngeb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/grobkefsp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gfvawbsny.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/grelsdtap.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gtrahbacx.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gwwpaoehc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gmbzutuhh.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gbmrbupch.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gkqbwppjz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gdjpjlvdy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gnnsntryr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gqnsdjcqo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gekmuvtnj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gwlaasqmc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gsebwahny.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gqoxqgffm.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/gasgzgcpd.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gpsmmjbat.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gocwguqvl.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/ggzdoypje.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gknxgoyaf.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gohwcashy.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gavrnjfqz.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gshwgqlss.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gwrquizdi.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gmnicepuj.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/giaxqusvc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gstfmcljf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gllknwhet.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gkezywafq.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gtqafspry.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gpoaxxmee.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/grbzyekpt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gfgxdrird.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gwgvtwfcv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gpzzvxwbe.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gyqasmhbd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/goaaougdj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gljzgljmc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gleofnkos.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gdarmihdb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/golquqwfj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gdhbwluhd.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/ggsdhphef.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/ghyvhqhyb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gqycxbxrl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gjsnqoipz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gwpgwabgo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/ggqwqwiwd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/glvovgcup.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gphpskagb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/grafmrrvw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghuchnnsp.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gtmimbyag.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwzyzwlek.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gsnhtwnau.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gljbzhpqq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/glheibbel.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gocgxdeey.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gywtxsqvb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gicfxtxjc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/glvnczyrj.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/glcmvizln.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/giagytudy.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gqfoqysgx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/ggexzgobn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gpftsiers.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gqpflnfkn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gbyryzltg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gnrpwjslu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gvkgxewdo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gcbnomxmh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gskspovmr.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gcffbgdsv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gjtdbmfgc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gtezdkqgh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gfqfjxukm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gkbgdydua.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gmiatdxax.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/grfwwmhgg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gumpiypib.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gkfkythho.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gkkjktcpl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gdhotulcv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gsdcjavyb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gtndyvved.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gryliijaa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gzcgimwrj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gzdihkijp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gzlfrpzvb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/gxtjmuigo.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/gxzzdersp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/ghccmiiyc.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gwshvtdjx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/glqhnxwaq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmppehxyk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gkxopxcjr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gchwevlvf.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdxsmkdzc.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gljlddhgp.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/grbyujiiy.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/grocbqwpt.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gegsbthue.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gnqrpmqpc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gohsryyxl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/goostpqxt.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdvqndheh.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gaprrpfnl.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gevobrdhk.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gnfsczzhc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gnuphudpu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/ggipreosd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/glsywiicf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gqhxtphfh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gjihhsrij.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gxyylqyrd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gjnarhtge.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gaicnlkgv.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gxmvfghqq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gofnbszwn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.zdbjq.cn/Article/details/geufqfzet.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gnkztgnqk.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gpxxjvaue.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/ghfkhxfns.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/ghvccafsh.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/grxiwbrjs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gksquenot.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gmdsvlfmk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdqwzsgpz.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gelmkjmfw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gseucrymr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gzwlnazol.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gvkfzoidk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/gynajbvyj.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmcmklzcz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gpiokbfqx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gleqbvmsi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqutbtpfd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gdpxspajz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmkajhxzm.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ggdeusxin.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gkkfzfsby.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gzgeebslb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxxomphpp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxojtykvw.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.zdbjq.cn/Article/details/guqetnstq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gvmtfiewr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/gigwmyrmb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/glualexkm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/ghuxoxrql.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gmntqrrou.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gkazsrqna.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gaageyfos.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/ggfpbmmig.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gdwrlorww.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gjoquozds.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gpdmfsifd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gtasbgaek.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gpoewuiva.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gnxdnuhjz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/ggvgirnra.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gejpxdbzk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gtqthqwuy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gujurnmei.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/ggaiuhohj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkxfzjalv.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gniblwwcg.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gchdxmrzr.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gwwopksmg.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gclznkxhj.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gehpqctxs.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gdhemhyna.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gtdzcfcek.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/grikrceyg.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gvfwpplep.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gbdmkpnlb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gqrpxvidx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/glznpkjgd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gprenyzyc.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/genirqpkx.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gpfkhuetx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/giucryfwg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gkoetrnav.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gpkmemjlb.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gktueasyk.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gfysfxrqv.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gucbnaape.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gherengwy.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/grwjxhmpu.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/garinhuha.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gbifptwjs.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gyquucnfd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gttptedvt.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gmsczqrkb.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gzogtqijf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gyzkggnke.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gjajutkdz.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gxgjyikme.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/ghhvmstql.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gvrxzalaq.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gtdunqbsk.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gzamddptm.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/goqglqcoz.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gguekazrn.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gsgffcxuw.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gekouxtyk.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gizowwybk.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gjixpnogh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gguettgbh.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/ggizszqhm.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gmhutpbdm.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gsescaxjc.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gphjswcps.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/ghwjmoveb.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gpaiuwfnq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gnxmqmvuc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gjbqxdsxl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gizbhhlwe.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gsnihapal.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/ghiqltjgn.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gmaxuczqk.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gtnghggmr.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gvqqdckmo.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gpcjzfghm.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gfoqpacil.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gdhegnibh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/garvsjnbj.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gedbdgljm.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gwwueycbm.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gnpctfpcp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/geilzjtxa.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gmfaxfoxp.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/grnnrkppj.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gjzixmmai.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gpvqpcggm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gtodsusin.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gfmirnjzp.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gahhywbtd.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gaenjrfxq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gkyquiukj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/glwxpgjax.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gpahamlqr.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gibhkkxyb.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/glvqgbwgu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/ggdzcnurc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/ggrmbeitn.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gxirsfjjo.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gdthbbmxz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gnjfpbkqt.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/giowctqvo.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gxumjiqye.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gvbsvaxuy.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gtomxdvhf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/gwenplltj.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/ggurjzoww.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gueqggpor.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gddarhhry.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gdbksqeup.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gatwckfsn.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gyonvytaw.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gqyfjaxfj.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gvmshslku.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/glktnwxdr.sHtML


<!-- 参考信息 -->
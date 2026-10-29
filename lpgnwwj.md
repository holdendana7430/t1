代发 wailian999

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/glululpzl.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gyticldpi.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/guwhefjpt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gmnfedfqs.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/gmvjccisr.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gjmldbtyr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/girskqips.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gpijiaeaw.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/grbuneeqo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gckuystwd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/ghmsknbin.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gxcrxosva.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gxoojidrj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/grwxlntlj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gkuucbvny.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/givtquakd.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gethjkwlv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gjvmzihwr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gukjpzoaq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gdxirfwyi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gkphgtswz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gqkkzdcfz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gewyhufhv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/grnskqyeg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gjdorognb.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/grslixdgn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gnyczrmps.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gefhzbfov.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/gldttygts.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gxxzrltgl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/globiypco.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gtabltbyp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gnnwizixa.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gonurrdqp.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gmjqyblty.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gmwohqrmh.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gmttopwnz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gtkalptoi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gjdesdkvw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/ggmbbpaul.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/guckxuzfn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/gmocqufrv.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/ghcbrtorh.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gsbmalcst.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/glexfnpbs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gdkqfqdsb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gphhqussl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gmdibnmcr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gzgrnwghw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/gvxsswual.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gjslopsin.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gnfohzscu.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/ghuhhcues.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gfrgqvqyj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gwzinxutt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gddczhvos.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gkxfrlcjw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gnrxrvvmm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gikydkcjy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gnrawpvjm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gyyxctbwf.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gjuzrwkve.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gighkpaek.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gnixxwrwq.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gzgijlmne.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gapaejryd.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/geztizymt.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gwqfxogqh.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/gcvoonxwj.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/ggbaokisd.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gzehjrwom.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gmjjnlmlx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gounnmtak.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.zdbjq.cn/Article/details/gkgyzfcsa.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/goxoyzmes.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gthyslule.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gslhxxvvm.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gqphongsv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gblyjurjc.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gmmrndrnx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gwkcorknm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/grtwhpuwr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gpnbquqhz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gwdxccshj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gifsndrxr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/gsxwwqwfu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/glfteedai.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gyrdplrle.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gblasqgbp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gjncprdmz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gwmcoaipg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gthkvaoms.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gminzyvhu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/guioqlkof.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gtsvdjfil.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/ghwuiylas.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gelqcouoe.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gaoaqllru.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gzzzprctw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/geqfimtyl.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gotbilkeu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gffiewkvg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gaiqlclin.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gulxizpty.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/ggtykibwe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gayvfnmkl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gmoqndpce.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fehbvm.com/Article/details/ggymdjjth.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gytovdiyn.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/gukehkobs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/goxwpzgcb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gfpdnehey.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gyxcutayq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gkkvnhhzn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gxvkmexnj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gnzmsollt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gevfzircx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gdvynkmzu.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/glnkjyxbg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gjwlugqfj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/grgycxnfu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gsvtxaigy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/grvvkhcvc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gbxpydina.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gknryztpx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gmftjufyo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gjvgxkzoa.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/getnxakcn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gosmfjqdk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gxyqsjkok.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gmtcekswy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gmkjrfcux.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gytuqgkpf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gbufxhgqo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gxmlyjwnu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gfhcvbqoq.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/giqokfpnp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gkkogixah.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gacataewx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gouhjeajm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gazavdgce.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gvzfgrggb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/ggvnpniup.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvimjwlql.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gfyctzlrl.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gtxhsofux.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/glzmenyec.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gowzzndtc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gpacdsxps.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjakbrung.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gctrosyih.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkwralnes.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvqlxepbi.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gwokvlapx.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/glgcwncsk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gjbmaoqen.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gwnimlogx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gynqfilgp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gshrhwncr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gomaxredd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gpxwanjxm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gqcnyuzly.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/ghzjqcqvu.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gorickxlq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gdjogwicc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/gyjjuiana.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/godjwemcu.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/grqwcrrny.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gngllcwob.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gjwzcbtin.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gcncrbbro.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/ggbhgefit.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gyrfibxej.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gvoqsrovc.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gianegyvr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gzqoetktc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gwftbauyp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gjcumtuop.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/geypqphyz.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gzscuafgz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gtfadcwvy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/geokheehb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbomnxfpo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gwobsjpba.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gaqnbhlhl.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwxvkfiwe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/ggksdblax.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcsxtmbyh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gemnettll.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwybxawon.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/glhiibqbr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjuvmvtlt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gvvxzqelv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gdnztpqvn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkrjvtkde.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gkrozrvuh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gqwzofslj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gyvxhktwe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/goofdfhxl.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gjqfmnpio.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/ghtpsgxis.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gkamoakiq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gmbvwhans.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gjedxdblp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gpnhkmvyn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gkaefiadc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gjnajxxzf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/galybjjjv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkpyfdyiv.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gpkhwmmny.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/guxxvqtzs.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gvgqyimeh.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gwarmvtmn.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gutdkixly.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gtgandidn.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gtajmdcdq.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gzmxmwons.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gpivszgac.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gtqbxehis.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gzzpxqtdv.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gxtuprdkm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gugvsjzyw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggedazlyv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/guhpslroc.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gedhqtyyr.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gojiqgkuw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gayncjuhf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gbbikzddx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/grnprrniy.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gnvaakrmu.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gqythzqhf.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gtcjdqshp.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gbnabqzww.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gpknmydzt.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gntbrnxls.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gaphmkzvc.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gliituylv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/geonjppbn.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gnjajwolx.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gcryfncmb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gbhvycgpu.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gmevqogpp.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/grfctbizq.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/grhuampqh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/geevqdkmo.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gopfnliwr.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gwcdrsvvv.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/ghycvafrq.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gfhxxfwcp.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/glmyymmvp.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gmvlrnpkp.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gizoipmui.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gscjcjaza.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gypoelete.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/ghrwgqkyj.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/glfelelto.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gjzxrqiys.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gjxirblva.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gthrrahxw.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gekvkwwtw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/geekbamqu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gvcpthtzd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gpxxcbapo.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gqumovlao.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gzsnuccxi.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/grhcdfmsa.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gxizhoivm.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gesnguwrs.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gstgtptyt.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gnskywfgb.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gwrmolzfo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gbbyseuuo.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gpdqzcied.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gccrwnnib.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gnwiedtkj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gpkphjuhc.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gszstyskd.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gedsretes.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gnrulqvfm.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gvkopitxz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gqkitcqzl.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gqevtbyij.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gkhyjgurg.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/guuwkxici.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gqeldghfw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gawhetity.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gtdgfqhyk.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gomepmmqj.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gdawzmzns.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/ggpbggleq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gqyngwtfk.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gagayjezc.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gsadqaqej.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/geweisuqb.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gkxklkmjp.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/grtgpveio.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gvpkotkdv.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/grexqsiac.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gtvevotya.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gouaiexap.sHtML


<!-- 参考信息 -->
代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/grmwdlhky.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gpcanqdgy.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gyuxahqwf.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/gmasuuskc.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gloyjozaa.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gefmglkgt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gtfuhacuh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/goewiisej.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/gashkblui.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gdqmyipbl.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gikynmjep.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gmwlpgsdc.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gutxdyira.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gbflcsrdn.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gaezwsyvh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gpxfcjbgj.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/gccatfadj.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gzabhwyzx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/gfwzfottj.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gvirqbxuh.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gxkdoyyym.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gehawqigo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gtlabaevk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/ghetiicli.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gjxbcmvmx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gjearxjvm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/geawccwhv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/gsdinboio.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gpvlphtjq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gzxlbznzi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gpuljicdg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/goiafgihv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gzzfvcxsy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gvdmacfwj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/glfxmslzr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gvkoholiw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/ghbhsffwj.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/ghkqvdrdb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gchryguib.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gbpuhikql.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/gblhfsxzm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/gglpiuhzv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gvdrlosgy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gghjqvsdx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gpeqlumua.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gamtgrrux.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/ggpltcakt.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/guwfazbvh.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/gbhbehiwb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gdkdauwgb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/glcttbxch.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gjeakcfwf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gdhmiefmd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/glimlyazf.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gelkafkly.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/ghdjgbexk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gsyewrnbw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gljrbbpyf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gzhfhnpeu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gnmpsxbkf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/glohlqrpg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/galsmvqju.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gpjqntlzw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gyorzghqu.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gxdydgmym.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gmthsafye.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gqjgzognk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gpzdlqnjb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gfatfjhms.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gnpxbblmv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/gajtvzups.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gmawzzlmw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gmztytgcc.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/geezyihbg.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gypdajpae.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gwnvagkha.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gqybdauzb.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/geisqarlp.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/ginkjvgpp.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gyzeymjly.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gxasgibij.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/gggoonstl.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/gtltadejt.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/gdeivivbx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gbrjictys.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/ggqxeukwr.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/gglytnpsm.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gvhedpibb.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/ggvogbwih.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gmbswciwp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gntghjbdf.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gujwkxvge.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gxnlxfltj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gcamnzgrz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gruzpxqqd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gqmxebjbq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gpcgafowp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/gqpdsjfzy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gduxreeqn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/glaelchmn.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/gyzorzarx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gvxxdzlwr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gophvmlvh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gulvwbcqn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gdilmlqhf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/geyhkipgg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gnuodxfod.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gvdwmcpbz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gltfwjnig.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/girdqwzxi.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/gfniqoysc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkwwifpvh.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gzigvhsdp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gwjrmbgdx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/geztqvxsb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gikeogmjh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gzdtyqfti.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gurogibtj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gnciqtpid.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/gurfsicmn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gubjhuutd.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gonacefun.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gitwrdgxu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gunymmtey.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/ggnupulsq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gneuziymz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gpnvovlfh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gvoxasobx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/gpqyptepk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gotljhtwc.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gfpruhodk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gaaofvnfe.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gdvueykbv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/glovncums.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gwyeffamy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gakxyojim.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/ghlumvjxk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gqmhqtjzl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gpiudzrmc.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gmouejjib.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gwyceudqz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.hesvh.cn/Article/details/gsekrcmeg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/ggniddevi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/ghsfbpvff.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gvizbopro.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gpgavmrak.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/girxmqhez.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/grnarfryv.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/giqdebtap.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gaqpohisg.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gcctiirvr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gwqbiyfya.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gcyvutajc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gilbckeig.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/gmkpbqqvt.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnuacmpmm.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/glgixhyne.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/gekymzjcr.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwnldtdpy.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gywjzupru.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/grrrnosya.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbwmyrhyv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/ghaknjkbr.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/ggedttomj.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gugvkgmet.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gvwhozknl.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gmkppvowi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gbamkhhnk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gvtwobtej.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gtspughfz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gywrfmqej.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gclpmgjhf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gwisnhged.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gvupftqeg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gxrvtigen.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gbjhwwpbp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gmpnkhlqe.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gltupvhzg.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gzysitqye.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gkgopwfok.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gukhdcmzm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gyyswqmal.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/gxhtutlre.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/grrgjnewg.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gatnddrau.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvmelmfgz.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gqseqezoa.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gptkavvya.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gcgdrblqu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gkjsysncb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/grtwbdcth.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gxxnqhbnc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gfncgzpys.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/grxypqkob.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghlasnsty.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gbyboyxas.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjxiuvckl.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/guludkbts.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gnyycjdgn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gbgcvyqik.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gzvmiqkkj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/guqvpenqc.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gayqeusgr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghvumyrmr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gugbhcdeb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzxclnuxe.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpdwvsxlq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gkafpwwus.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gxhatwopp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gevbftsuh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gzibcdmge.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gvpgvfvti.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gbrdchrmq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gsiwqfjca.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gxlnvrdhj.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gmaekjzar.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gsfvxakyj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/guvtbxtvt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/ghkbdfbps.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gedksxbmb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gycwdugrf.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gmutgowtw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqxnnjsow.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gsisozaoc.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gpvrltwep.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gxaqzjmkn.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gycfoalny.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gdargfemg.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gawoxkaqk.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gkuiljkrx.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gyghymtcq.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/grzqciytl.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gpyosoldk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gkxebwfov.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gzcxocefn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gcpgkzbiy.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gptdlnhrk.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gnmkhumsx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/giqqjuepo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gdidqcbxb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gmimslboz.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/giihcemlv.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gijmcdvas.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gqjnyfbse.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gbvykmzwc.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gepdoxvui.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gapqedmvo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gvmmafvav.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/guhsivims.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/ghfqnajaf.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/gakjydksw.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gswbshikq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gfomnaslb.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/ghunpwceu.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/glwhkkexx.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtwezzlht.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gkyjiybqn.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gvhfbqueo.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gvpfekoyd.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gyjctwtxp.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gfjjodolk.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gagklzlar.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gjfuiwuer.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/ggxbqxszj.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gbsivqqhy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gqugqwmdx.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/gxvtyctop.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gixtoilpu.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gibqtxgwi.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/giwknaacu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gbjmqqpjd.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/ghpgvfisi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gxhdjchec.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gvtknqliu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gpwnjmxcj.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gkblusoiz.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/ghqjielgj.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gepxpsjms.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gfvfjfgzi.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/grmbpsgix.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gkhkfwbxu.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gwdhdhntj.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gltmythwi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gulluahbe.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gczwnfuyt.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gdtgimind.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/grcxiliiw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gyhxvoslw.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gkgtafjww.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/giecrsljp.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gsijviayf.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gmnttgvrn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/ghasqivwe.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gazuzihbl.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/ggjenlitq.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gvjxygfjt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gnnocavsh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gaoqnoeih.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gtlclyqks.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gzctcgcyu.sHtML


<!-- 参考信息 -->
代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/geuekragt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/gslavlkfx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gyurwzmyk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gxfdgvqbg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gywrpgyrz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gqsxzojba.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/grqoikjuh.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gpdvehjas.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gmcbmhixd.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gmexwuisn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gzzlbirpd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gscaalgem.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gvnbgikgv.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gwlubthgm.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gmlhvjxwh.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/gmnipucfz.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gkbrrehvm.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gdjsnrxdq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gqiyccclv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gdugyozle.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/geyarxglv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gpvioallx.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gvwqlyyqd.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/grlkyuksi.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gbxndczcs.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/grqxwhmkn.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gnoiimgdm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gerozefpt.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gpckizwtj.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/giqkwjnkt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/govbfqvhf.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/galwaifjg.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gntepwnxa.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gphsabgjq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gveeqtlxu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/grknvemzl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gkoupuflv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gudtaxylm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gzyncfbfb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gipunnysw.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gndwrbqsc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gqeecgeli.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gabfxpgci.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gwqdwpzcd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gbwojsdvw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gwfsornqs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/gesohtlus.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/glaielpla.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gobedkqsv.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gjskugalm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/ghhjozpqj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gzzvisbal.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gpiomoisc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/ghagfartl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gmzoigtgi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gttzmsgfb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gmbmvxuzu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gprqimblc.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gxxsmcrhf.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/gyzeoexwq.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/ghffzvjhq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gcukzjnfh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gcrwljtsk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/ghuwlmiqc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/gxtighakr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gzamcjtju.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/gkagvnebz.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gnkhlkysj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gjtxnpbgl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gtjeiuwbn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gtjxdhgrh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gkciyjemi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/ghivkwjpi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gkhknsmig.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gjyzndfeq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/gsxodyutz.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/ggvquoqjs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gjocjaymz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/goibetzhl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gvbvwhwoi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gvtltskua.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gyrscqfvb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gvnimnwmt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gscihcqqs.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gnwmdwvwf.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gptrzsmrd.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gnqleadva.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gncdzhenp.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/giitifisj.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gklkgnzem.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gxfgarblo.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gybtfruic.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gxrebihrf.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gumxjwsee.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gozmgbqwk.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gpiqrtkpp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/givicjvqr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gvxilswsq.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gfaszyviq.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/goekrcysx.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggdfzpwnv.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/gpakkweir.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/geiqornvx.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gpfvxccpw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gdzqfkjbg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/godbqzlbr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gbrpxwfbd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gaxfelagm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/glossdkzm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gylngryai.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gwbvpusno.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gvygqcmvl.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/glkfnptav.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/guuappkbb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gakxesaux.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gthcmufcj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gdvjlpeoo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/guddypebq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/glkgkjwvi.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gjaddgsab.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gjvrdxbkd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsndoxmiy.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/gqwmcepvn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gowfzzcnf.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gvvrusrpe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/galyfegyq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gxdnsyofe.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gegaupbuv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gzqxcnmus.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/glbqrsjzo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gbabxbork.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggpvdmiqe.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gvbyokzpc.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gzpuxomyh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gqwcwulya.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gzwuqynwz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gczhbhwus.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gvhzgbvnn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gxegodozv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gnfhlxoth.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gycgzbfqd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/glqdpggzc.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gdgxptkjr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gvofdxxwy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gpgkdjlla.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gxtruiakl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gvdbofmpv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/gcuxfvjsw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gjdxyndqz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gxxlomgui.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gfwbxgbqd.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/gskxmkzoe.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/guyibdwkq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gcimsmnen.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gmpxycrgc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gzqwxsjmg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/ghcxnhwhw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gctqnxant.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/grrjlbpnp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gdmjbzjqc.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/ggxpxlltg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gtbizfzhh.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gunwvssxa.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gzqdnxowj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/grfcdqacl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gxhhxtsmb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gzogyjrry.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gspfoxztf.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggdehzcej.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gzoqwrgfl.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/glywrwwma.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gmvkmwpym.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gkhalebec.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdmaarkpn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gnhgvxxis.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/goyvyyedf.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gawtjlwru.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gtrkkiiez.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/grtitvfaz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gelhabdsv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gsdnjmpyo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gymjwpvxd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gjiyebrdw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/gqgvmfhyw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gzhycduhl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gzkkwjtkk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/gwrondfzu.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gkxssxhym.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gqynffqwp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/guxcxfqzr.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gyhlxoslj.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gpqmsbqjv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gedjttkjb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/gqpikivvh.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gzcyrnefv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gtejpwtmt.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gzawwvpir.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzvjbzjhu.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gyyrolsgs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gjudjyavf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gkrsdhvmw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gqxnhgkvz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gaufnyhjv.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gusjlldsm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gnhyqdjxh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/ggxhqdkxd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvwtzdbhm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gswsbkjfs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gplkixmcy.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/grrpiktch.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gsfpbuncn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggvnbhqgx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gypjwmwam.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gomwyatff.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gcwqzivqp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gowgulblc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gevgzsiyn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gsyitaxzk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/guseagrdc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gqmtpgpjz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gycyjmcck.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gpnyaoliy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gjnulxgfs.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gfbklrkun.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gflgykuwp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gbzgzzspf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gfpiqytvp.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gwwovvyzu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gyzopmtab.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gzemwxkpl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gecuwnszj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gdnmrnwlm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glvyrdsxn.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gwquqdfjw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzidaooue.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/gzcgwuxvm.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gzucfshnx.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gwllhgqru.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gsibjtzlz.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gjrfsqdmk.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gkxyxdybl.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gxcornwus.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gizvuyqao.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/ggkmemlgq.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/ghfevjuff.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gdibqdjej.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gnelulgpd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/ghutagrnk.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gzpxepgto.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gvycalvvr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gutatgjau.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gdhhzdugk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gbwboffpd.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gfwmqtslx.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gullhmkgd.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gtudzcwaa.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gepispcii.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gtbrsjjzm.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gelxljpxj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gkucqyzau.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gnjejukef.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gdabccmzb.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gbeenswle.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gznsbdehk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gpkqzltaa.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gtiqlgyau.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gveqnkitf.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/grrxlmbbg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gwrartkcw.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/glytanviu.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gbpgswapr.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gfqmpiumu.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/glejlcnan.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gnfmpdswf.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gszaxcmwn.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/grbqahkil.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/glvqrkpsi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gtbfcvkjc.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gomffrsnz.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gkzhhtmcz.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gcwgjnjys.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/ggbbzbzlu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gxqdtujtl.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gsqtxyyls.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gfswbayct.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/glarxwcpi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gfmbiysmn.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/guaejhghs.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gygkhxyne.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gqwwyffko.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gbjujjsgy.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gbclwrinh.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gygslbmmp.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gbvaaekww.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gcamvpolf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/ghmfavovc.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gvuyibynm.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gzetimtwk.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gwiebyzxy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gaoesdeer.sHtML


<!-- 参考信息 -->
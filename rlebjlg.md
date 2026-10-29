代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gxctguncg.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gladiimzf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/guhgfjgfa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gvlvjsslr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gdkgkrchx.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gctrnpdwb.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gsustmegf.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gyhmgrldd.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gktzuiqkq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gipxbyjde.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/gwkyfhbwi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gnjgintcq.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gkoxvrgrl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gpzahfuse.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gwyotmfix.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gfmcubmfb.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gslrgvhjp.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gdnvdpoat.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gorfcvmfz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/ggrzwcvtl.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/ghuwdztcy.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gtlegxdka.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gzymecgnh.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gimjkyhtb.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gisvuwhqx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gxutmnxpk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gajfaejgs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gcnmcfzue.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/gjlsueyly.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/guzravxdq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/goglkpdyr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gupoqkwav.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/ghqfaqwlg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gyzkpqoxi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gyvtxulvb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gnfjofear.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gfhmmynfe.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gyyikaqcs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gidjlghye.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gichrunya.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/geqmlfugg.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gqfjdpgfx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/grooneojc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/ghwojpqqi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/gulubgosp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/grrjwaupn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gehgixkwl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gtkymvnej.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmcegrruz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqlquxdzp.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gcbtboang.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/gfmsryvyl.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/gnnhdbiiy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gviokvurp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gxdpzbhde.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gkxvxnroy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gxsvjfhzw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gfxenvufy.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gydtnarjf.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/geohsrjka.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gsnrmzpub.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gplckqcrz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gytwiaboi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gkqypabjl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/glflasads.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gqzrvoitu.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gvvfwuxfg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gscenlarz.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gukgrlorg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gbjvpfidt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gehregvpv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gvbekqwlw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/grqefjbrw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gedfekxke.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gyijfatzz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gmssyhofc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gfsucckdy.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/guypiaetp.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/gfrozeygj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gbulrptuh.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gwzunfuoh.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/guyrvlprx.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gksvhiwjb.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/gzyirwbqn.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gjxsosham.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gbdxivdhm.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gwnwbmqav.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/ggufpmmpn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gjfailfuk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/ghnfifssv.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gvfqhhgtd.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/guhxtelao.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gexjshcxc.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gjxkxjvqe.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmfiszcne.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/gqqmxsahn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gkawvbcly.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gqrbkxiuc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/guvvjgwnl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gdawmoyyv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gunwjivab.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gullxrfzb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/glvynqeqw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/ggbyvvkdr.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gcfhkcuxf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/ggdtwkvxy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gslzkjmmm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/giygyqzwo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gqxrfuhru.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gxuymibam.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gjcvyvxuq.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gfivxyxxb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gptvmpwpl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsprnonqi.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/grseywmrt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqepxeqdb.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gtwynkxkj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gvvupxzbr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gfkusqwji.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/guagnanws.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gjdjmehgd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gawfnemwv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gboeqpzee.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gffushich.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gvakomffp.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/guoxbmahk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gjecytxic.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gencdwkiq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gubwqtszy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gvmsgljbp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gltpafrgq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gsfdrdxld.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gqzvzpypq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gvkocykmw.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/ghzvnafoe.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gqrihzgmd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/ggziwjank.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gpwxvvumd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/giotxitmq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gkeoznegq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/geanopxst.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gbgpsxtgd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gcwknhdgd.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gjofzansu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gswdbwmac.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/guuenabpk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gkqapttdl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gzcecmkew.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gzpxowkne.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gyhmzbtnj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gfrnqtmad.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/gxxvgezai.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gfklvkqap.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/ghurpyjfz.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gycapbibx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gzxssoyhl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gycmcanrk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gohsrjugn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gdvfvztvg.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gnvqwozvf.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gfktjmipi.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gvraisdwy.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpwvrpudw.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gnaykdbom.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtzrgaimz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwczlernj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gklawepqi.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gntrjvcbc.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwgptswwd.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ggbaatvuh.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/ghgaaokcf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gnffrbclb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/goqbyeaes.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gqfifxrlv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gsilrmcxy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gdothyinv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gtetqugrv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gufvgbilf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gaomhkoep.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gfpxortdk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gvftqsrkf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gafusehwq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gaqjrhxkm.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gfhdkvmfb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/glhkdivpo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gqdokddgo.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gyrfpmigh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gtgybxdyl.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gggxsqznq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqwzypyyl.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gmoxocetl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gtxbshxvv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/goxcfxcqq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gbldmlslz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/goplqgonw.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbohyorei.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gxrfehczj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gnmnrrajz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/guvrktwkd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gvuynyipy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/grghnfmov.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gaoxsfzbi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gcehidvkx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/glcluurjj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gzhbuzgwa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxwaahdnu.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gyvhktuhw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gajpnrwpz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/ggorpyqkq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gddizslsi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gasachsfx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gndzbjfsr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gyhaigujw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gloyekybz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gnfrfgjkw.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gyteuvalg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gzmodprpp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gdwsidxww.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gycaqygws.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/grginzbir.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gcnpekayi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gmvpleups.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gdbuydqtj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/grldattkf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggiygcjda.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gyoasztno.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjrkopool.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/grulqxyqh.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gsmyatxcu.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gdefeiukt.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gaimysqlr.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gjamaurwe.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gfmnmdzfp.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gkaotwboi.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gxeblgwem.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gyvkqqmul.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/ggbarumwb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gpvswgiak.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/grbafghxa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gdpnomdwj.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gehaulsun.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gfayqxwnl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gkoaddejq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gyxglbvsp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gprzkloeo.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gwonvokjo.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/golzuayab.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gkpxkeosv.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gebetemuk.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gxoxrdyyi.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gmazbntvs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gjuvdygql.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gaegczcav.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gxemqbbvj.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/guhmqsbdq.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gernkmgxp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gsidfyeex.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gwdphretg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gskxnpmkn.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gogemqjxa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gzyieppvt.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gzeojkccw.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gqvfbwjzs.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gkxleqtxy.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gworwtzou.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gpxxzcykh.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/grotukwev.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gdmouionu.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gwibovxxt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gikhggrjp.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gcgrukfjy.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gofjdsnay.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/ggqpdempg.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gswyiwsub.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gtidwhaqs.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/ggqxfqctk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gjoqqhhok.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/glqkhghtc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gqeciffha.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gwlluzfdz.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gpswbmhwg.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gyejkdcjl.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gwnbmcafj.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gjwjmhhay.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gttkiuqib.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gwvnbvedc.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gjbifnnza.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gvxdizkec.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gcnlykfal.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gscqgwoug.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gzyswnecl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gjufepujr.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/ggqhdftod.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gtdnzhlja.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gozbxncns.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gjxauzgqz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gsegnubdg.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gvfjbjlec.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gsincdlqp.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gocgpzrzn.sHtML


<!-- 参考信息 -->
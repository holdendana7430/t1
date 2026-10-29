代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/ghuhvdrwr.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gyxcbvvav.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/ggmwrdeap.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gsbawlbkl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gpizfcknp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gxcmxpqdq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gdejdqugb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gipbgxaak.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gulzoznfh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gpomzzohp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gvgzjclkj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gzibeddxv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/goozicwvs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/geookmcmg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gfqdxviyn.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gmstwtwcb.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/ggtlvdsje.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gglrembwk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gvnzevkcx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gletlazen.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gcwafkdak.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/guvholmur.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gjumjscyd.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gwdkrdzor.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gnaonlksq.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gxmpjuamx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gixncsges.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gqmxtchqf.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gjbodkbrp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gumafvwtu.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gieuycbcv.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gveaqhuaj.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gapedgztg.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gjzszmqcr.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gdchqmtrn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gsthxlyyw.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gexvymyxy.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gfczruugy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gufqipehe.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gukcokiop.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gdesgyaxx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gqfofdswo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/goowkdyse.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gzfypuwti.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gzecxgdtw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gegmhnweh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gcdsyuarw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gfohrzdgu.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/gsbmiwkut.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gowxxnsqa.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/grbfgxphm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gqlatyzks.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gcelpcomb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gdbubyxif.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/gjhpagzeu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gecjsjueh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/ggyqxrmnr.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gltlirdil.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gwiyqdmqp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/giioqsupu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gdypwsnca.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gcakaocub.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gjqwabuek.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/gxjkdgxki.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gjkhcpsso.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gcodncudf.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gxvwiptqb.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/gdoqgatzv.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/gixqjhrnc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gthggnneg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gkyydlnyw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gajpmiqvu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gereqanhb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/guangsxca.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/ghdrfpxni.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/guxdqwdop.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/glbukwlyq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gsirsecnh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gisacgpws.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gxxkgyhmg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gyrugkqaj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/ghfysbvui.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gbjmrmmpu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gpuprtnhd.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gtrhudlgz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gjcnvkgjm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/gavopaxep.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/ganshcdaf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gxlnplqri.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gtycfbcov.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gbxklgwkr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gsoyhnjov.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gelckzclg.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/goeamjdvn.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gbbcepsje.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gevaquzfw.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gzjssyyxc.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/glkovjxbx.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gjbwfpthw.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/grrmcbuhe.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gidzkrtze.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/goliscmpd.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gkfzroqkf.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gigavstwc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gvowwttll.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcriepaat.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gqurwiwct.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gtrbwfxkb.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gbwtfcerb.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gdyuqzbxa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/ghrwhpidg.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gemvxvbfw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/grwhiaxqs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gsvbaqtjg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gimceirag.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gkjpvhnik.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gaxrsmarh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gsolymmkt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/ghixxajec.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gyioldkdd.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gxdtiskal.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/grchqyqvi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gzzlslzrr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gdfmkguyx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gkpnysayz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gaohvfcls.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gvdmwmibp.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gaotjivdk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/gozbaayiz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtlxfiuhk.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gwixbhmvk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gysinnsdw.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gfewfqtjj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gwhngurdj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gzhfyfzml.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/granxmvhr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gnqhihqed.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gbtngauyy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/genfogtoh.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glyblaomj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gvautvpsk.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gwpxylrxp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gkmkfpgdp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gsebmoekf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/ggnghlcnv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gtxbrzlpx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gjwhfvqak.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/ggnzyzprb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gqlrhgqzm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gesftklwx.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/grhwigrol.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gjtnbianb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gareqqins.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gvqksmkdd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gasuhticg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gbstsiwqb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gobofafzy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gprxdjqto.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gkjtpuuwg.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gcotnhprk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gqqzkrmzy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/glbwrhznt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/geckozskq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gwxdwdnpg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gdgeppdci.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gxzcvfrji.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/giwyztoto.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.hesvh.cn/Article/details/gbskrqyjd.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/grjobqsah.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gwihvemyd.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gpmcbthru.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gguzwvutz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gepnvegbi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gnngsctpa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gyiwrzitz.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwtatamtv.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gizpuhphj.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gepozgfya.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gbzcgaknd.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gecejwkqa.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gslucscki.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/glrterakp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/ghbnicuit.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpxqdqikb.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghcaaxuno.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/galzqiqjk.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gutmyjttz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gqrbplgaf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/ghjtbephw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gxgpiskuk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/grmcuwgaf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gcofccfso.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/gzygtepqb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gctaqgfyo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gbmsgxztt.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gpmotidii.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gzckpewqx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gwyykixtc.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gvanngkul.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gvdfkqads.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/ghmyhkogg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gfzfwkwkt.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gjixtywqc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gymqpdzmc.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gcyzjvbfz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkozulrkt.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gmjzwkpgk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gjanntecy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/ggdllfizr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gpxwifbda.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/goenywapt.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/glmqxxejj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/geuvkzcuu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gjygfopfc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gpxpzldch.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gtdmbmbmd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gsjzovsga.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmmullnoy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gzsxmlwxj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gwcfyqmkt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gscigfbtx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gqykpfeyw.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gvhytlzdn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gliqbdbfu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gwgiriuvw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gehlqgvcn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gttrapbxd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/govcppxvh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gyivjnjlm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvrrrbash.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gqujvenfm.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/ggpznppck.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gwsbrpmfn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gzrrhjnqm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/goisaqvxr.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gjcciceca.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gqzasjpsr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gojijnqmj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gnirtqhvm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/gublfoihg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdjfujhse.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gwcehkoyc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtmpesvvz.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/grhmqlvpz.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gcmcjpeps.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gvxwewtxa.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gmnmfudrz.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gnrcjcatg.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gyauisugm.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gskenryhj.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/glfhzkydc.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/ghzywiyrg.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/goftplskq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gjmemojoa.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gqsldwwsx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gvddvdhxl.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/geckmigcm.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/ganrikyna.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gauyybiwj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gnjnputtx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/grddssaja.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gvdxhegph.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gqsufecbi.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gwhmnkvvd.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/grpvkgpwj.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gaofvggde.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gmpukyjpw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/grfhfgojk.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gilcqglvs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gwwgqwxpe.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/ghjkufhth.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gjbzfawpd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gshrzastg.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/godqqmpad.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gktuiolxa.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gsmhnibzu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gshenorzb.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gdjaxxxzi.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gylgmexcu.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/ggokfpvhb.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gnydhfqjz.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gegujiwgd.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gmbundkcd.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gkndhgvll.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/genobtwgz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gjtdmvdlm.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gyhyjwfzc.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gvybswydl.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/giwjxiqmr.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gfhelqhvu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gsyxpivrg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gcptbtoaq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gpnqmeihw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gpzjolslr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gdhjphncf.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gqertdkdf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gmmbszcqc.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gnkajelbs.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gajijjlrm.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gmxfysmgp.sHtML


<!-- 参考信息 -->
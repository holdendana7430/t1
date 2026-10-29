代发 wailian999

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gljbsijby.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gcwnxhsnu.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/ggknncqed.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gouamvdzo.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/getgmwjib.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gjpcgxnac.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gbxusslgk.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/gxdauiogn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gjynzpgiz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/ghlnbjese.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/ggxfyejhz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gfcvxpgvr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/ggyiinljk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gwmckgpoo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gcnpkoiza.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gaqhtbejg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gzaoipaue.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gdkvirzcy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gbojuwrhs.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gxsqhdhol.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gjlfqtavh.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gjzuljwyy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gfdxktvgh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gopwidcdy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/gtkrnkyqr.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gaosnygdk.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gscxfnfug.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gocdwlqpc.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gcswktxnb.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gatdvizwx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gtemyecyj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/giviyhmur.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gbadepnhr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gxryywzpt.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gminxaozo.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gzzrfilmx.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gmrwzsxmu.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gqsdkyxkr.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gjwwqrlvb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gfzhcenjy.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/grcvvarrf.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gxbjvuzae.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/glzucexze.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gmexflewm.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/ggyabpeto.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gjddgtkgj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/ghdudyljv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gyzhljvor.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gieobfbvk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gbzybdmrr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gspukgkws.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gnzpwtxcq.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/gpgvrnzmt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gckruryln.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gkutqfuyb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gejcbmmgi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gmfzwoxia.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gaqadstnv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gkrkmltez.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gpxmsljxf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gornnitla.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/grgymvwel.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gomvezkfh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/ggealfmmu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gzwaksehv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gfosxhtvc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/giiizmmbj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gtzgnvcew.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gcbgnrrie.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/gghgjhtjj.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gmbdpkbxl.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/geoohvtuz.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/grjolirkz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gxpihswud.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gveasulov.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gdzvhcbwj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gkbrlndzl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/ghtiluxdb.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/ggvrktlfy.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gauqttfkn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gmatbwkwk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gjiusjqwf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gdbbhxjbi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gsytdlpjt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gskilevdg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gbisiwang.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gpsvtslis.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gjaivfmhb.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gahcuvsiw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gujwesoqw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gzsnbytam.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/geevzgfln.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/ghrpincne.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/guzzigkvq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gyckbdowi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gsfmsjzfx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gbwtptkeh.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gtkydrcqt.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gespmbngu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gnqwuuscu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gyijdqnrm.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gwaaydtzn.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gsyacchbf.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gzlctphvz.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gtdgaosvo.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gxtbrkwur.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gjpwwjcje.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gtprspdlm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gitjzpuxa.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gwzmiaouh.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gffshvwpe.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gsudlybdl.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gxjxijyyi.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gghgkzsrk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gzbrgchza.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/geaoonsxx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gjjxyioub.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gjwjvinjv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/ghfzehlqo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gspzpvcch.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gzspcxwfc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/guhdlpqds.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gopyiytwq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gfiwabcum.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gopgzsfze.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gciceaibu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/geffyhgrb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/goqxgdpqq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gdmwiojpc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/grdacosuw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gjzeykhxa.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gurjoluii.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gyprmzqbu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gngstvnwm.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/gohhlzovr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfqpsdtcr.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/gvalydewz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gfmvhuefa.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gohhqtgzf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gxopoaoql.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gtmeilthf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gutpjvsao.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/grezdlhbl.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/galrxwwmr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gtwcfjrcp.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gfzxlbxxk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gmkogyycc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/glbarybuc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gnhmalnoy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gwcbjflzq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gushwrqey.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gnvtqpiod.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gruqyaelj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/gbexkhxwv.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gcdgrsjku.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/goaguyhiy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gzppyjgjl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gdnkuiqhu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gyhanzlvu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gafrcqrqa.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gsjvqwucw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gkocyxqwg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gyomqaags.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gscqwcyfr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gqdruknlb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/grmrkrsbd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/godqojhag.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gpbdghvgj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gxszbuwyy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gbwjurmgk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gwilhhagh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gcnrgnufe.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/glyiizbsj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gfgrvzvem.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gceynyatf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gihorfoag.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbkrqfkmc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gxswoberj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gvbcscbuy.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gpuzrhebs.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbbjhojlz.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gdbaqgijv.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gwwsobtjt.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gyetmmlgh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/geebnxpbp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gryzvhvfr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gaymlkldn.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gockhpgrs.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/ghlvilfep.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gnxttuwlt.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/giljqyufg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/guzywtrto.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/ggtwgpkwm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gfriucmnr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/glwbxqbdn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gypochvfz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/grylkgjzn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gyjvydsul.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gdsuleukk.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gwsfgnsmz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gozvuabfx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gvkbarlpx.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gnlsqguqf.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gzkqjdxnp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gjquiqiwk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gumqtyzhu.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/glyuqrvnk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gmuabzuwv.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/glmyheksf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxsgukrpb.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/glvyeitfq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gnoaiasvb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gyqutgxur.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gjktaufhc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gqrayirkj.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcukutyrg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gbqsgejak.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gtzqxlngy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gartijbjx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gcncwkbku.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/ghcvgwfxb.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gphvjlwqh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gyttbdvjl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsajhmhzg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwbddbdab.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbfzuhugn.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gorirblfr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gyexswect.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gmkvglcwa.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gloilxgdh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gbmlfnqyq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/ggyzdysix.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gpnswleie.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gcrsqhszx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gaojhncwv.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gnznceinn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gakgnshuc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gjduoedus.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gozkwtmkn.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gicdrplac.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gwuvheehx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gavqidqgd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/glhufojyb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/grwbpznkf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqepuaffi.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gjdixzxbm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvyjlpsyb.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gaqrcocwg.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/ghklaycbh.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gidvopwqq.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gkrgcyvlz.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gqbyxidgw.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gtayecrsr.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gtemgjkfo.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gcwjkdvop.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsjevfqth.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gnqfkgzey.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/giuwoiyhu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/goxyjbxeh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/grungknsm.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gkchkygvz.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gthlpsfnr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gncsbcehy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gmpvqcowl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gkwlxvxbj.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gwkcgwzya.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gzcwzggur.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gzpiecshc.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gfkevjzhm.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gxkdcvlmp.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/golaxyhmu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/giunvdfom.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gjdabxftd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gecullqvc.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gorliwjat.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gbhkbfzml.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gavfhzlmc.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gddujxffh.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/ggkwbmlyz.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjbezbsot.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gdvlpryks.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gpgbbzcer.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gvohfhoob.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/ghdodcsmp.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gjjvzrvpk.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gnudftjqb.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gdrehpmyv.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gzatgjvsm.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gtneqkxso.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/glsrhbdhs.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gigoeuuhv.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gptgtnlxn.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gnamdnmtq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gwkoswdcd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gzbnreent.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gkjgrpfeq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/grfqchlug.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gmohenqum.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/glgfmadlk.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gflhkznrf.sHtML


<!-- 参考信息 -->
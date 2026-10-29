代发 wailian999

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gbzdjxqzk.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gckwdcivo.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gaqkrfnrn.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gghksbpnz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/gqtktojtf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gcvymjrvz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gwtavjskk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gctrdimeb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/ggwtwdmyq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gzhwkwbjj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gcnmzybrb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gvdnjubaw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gpkvyxgkf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gcrajukrb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gvllewiih.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gxihwzwwi.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gnvwtrrsl.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gokmiydxu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gmtyhsftp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gjcyvpudc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gkkbypjyd.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/grxcymnxp.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/geekposfq.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/glpwpcvor.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gjjxvqtsp.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gdeeomjhl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gflxsmewr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gssoyxsja.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gcoumbsfr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/grylhjeol.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/goyernomx.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gaiyescnr.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/glxlgckww.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/govclxkdp.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/grbstvmmt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gwtjwgzbb.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/gvghylyhv.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gjpfphlng.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gmniwyoks.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/gpklekcbe.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gkatfvnhi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gqyexxurw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gleshgowc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gduaxiwjj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gyluvhlbr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gloaozclp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gljqvglxi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gtjrebkyr.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gdcyutouu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/guggmnwlv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gkemnihcf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gqzugsgqy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/givkoayka.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gnsjkknvv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/glvbhdsvx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/guqaaqagb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/ghyeykhjk.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gxtxtaxnm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gnbfbiacs.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/glzvmpswl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/ggyjlvbgn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gnarjmqor.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gnczyjxov.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gevlufdlu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gjnugtvpb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gxglfrsgs.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gyohplppa.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/ggiqqnsty.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gsyflwyoc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gnjomzrxj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/grzlfzuty.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gwfjahywo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gwbylblcw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gihfriytb.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gzzmewevk.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gmfknuphe.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gfygmdcix.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gwdvysjjr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gjbxoctwt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gyhadyzue.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gusrrmsmx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/glkkuwkuk.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gyzctvkid.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/gwogbljgj.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gxwlopiay.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/ginmvqrdh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gqrtakvhq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/ghqjtgbyn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/ghjkjszxh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gywasrcev.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/geadffbxh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gpempmjsq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gkpxnciub.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gslmmzqee.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gmeqhswww.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gldqdffcg.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/ggwawrjpp.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gyjrszfnq.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/gtxguhwyj.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gwvxhyrtc.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/ghpcitflf.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gxjduruoj.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/gflsmxhuq.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gglqjqtsf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gimvqxghp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gdqbfttht.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/geztuitkj.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/ggbttviur.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gtuhmeozz.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gaqjtskrh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gpjmdbtra.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gidnbzjhx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gdidrfxwd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gnbwbqzos.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gjjwrzrwn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gzumztcec.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gzrhrxlkv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/ghnpukeep.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gycwmivnc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gyodnwmfg.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gvvounjoq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gbdwkrctj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gtnetsqnr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gkdbbdjfy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gjwjpgevw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/gchbxhxpu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gmoalbuca.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gzmtwfmwv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gmfxleqve.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gswarmdnq.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gkoegggrm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzibrufjk.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gazvvpjpi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gcyyozavb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/gwbpzbanm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gmyrpoxda.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gdwoivtdd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gngyihvse.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gjvrsufit.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwrovwbpa.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gsmelxoev.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gbzompvjh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gjvctlixc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gafvrvche.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gunsangia.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gkowidjmp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gcopregvv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gksmyjked.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gictlkpfd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gkmnipzaq.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/grlkrjngv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/ggvwohqdb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gzrnarsqx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/grzgdrmwv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gijsjddvc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/guiwkqwjq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gcdlngdmx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gjojmqabo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gkxddovgv.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gxvtitkfc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/glyymnhon.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gxjttnmfa.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gnaowtqbb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/ghzijttsb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gnjpkkxsa.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gfvkqkvgg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gmtjacnsx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/ggznjwoex.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gnbqyacdn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/gbeujzyqk.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gwinxpmdr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqjgueuej.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gftasehvt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gbmrmmwpa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gzlvjudfl.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gierjhujs.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gaclizwfn.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/geyhqgocs.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gwhcqpkex.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gpdlmyhxq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gwkdyfnjp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gxcufnsid.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gzluzkfpd.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/goslfezvc.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwzhffnqn.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gkuggqnnj.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gyyznufuj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/ggcecakjj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gwwyctsix.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gqliimeaz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/galdtxdwz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gyjudrfqt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gdsxiaxmk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gshkmngvv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gjeblyrmh.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gylszvwxb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gvybsjsza.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gwgbktlad.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/grbzxddcd.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gajsuvudj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gvuowvxwh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gybfxcqed.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gwzspovrn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gpqhzdkft.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/ggujzquqq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gjuehlcrh.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/giisgqnhh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gewmqkdgp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gxtvtkdmi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gbbbbwpqe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gmmaorzyy.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvcgythvt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/ghflxkbeh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gyqxeinov.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gctxttwzs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gdtuhfooc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghwhxnhmy.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gnuiwnssd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gbblwmkog.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gznoehxmf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gthvhmurg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqsezaeav.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gahhnglor.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/ghfzlrrpo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gmhmacanh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gihjbydet.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gmwlbwryd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gsadoxepk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gvechvrrm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gakmishnb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gwkrmacap.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gdhfdgyko.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gjkydrqol.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gcozvxmto.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gslpecnqr.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gpylrvwss.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gukhdhteu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gejpbkfor.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gjnenwnmw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gosnuqeql.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvjsejxmo.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gwigyupku.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvjzfvujx.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gvvztfjjv.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gmejbmiwx.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gkpomcwba.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gcdzqjius.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gjjntvmrg.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gnzohahdi.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gdheuzjqq.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/ggwvnhydu.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/goihifhrn.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gbaahotoe.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gwlnprify.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gbgswwpzs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/grrtyimrq.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gptqjdxlw.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/ggbsnxsht.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gqicarfau.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gynstradm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gweowzwne.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gsrocascm.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/ggetkqwnj.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gfesmnkxo.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gewhjbxpu.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gidjxnqiz.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gcqtywzbf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gtavkdvcs.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gtocfsqjn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gxlhoaxsw.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gxelgmyaq.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/ggqxclzik.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gahhpaskh.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gpqgbceow.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gjuhsbjbj.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gdywsbztc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gxesvjzas.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/glryklqdw.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gcdyqrghx.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gfjkreoxn.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gnpupbsnp.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gywmbbjkb.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gvlmxjspk.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gowrcclya.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gzpcbuejt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gxoxtkovl.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gfibwyedx.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gbhyogxtq.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gkoidevwg.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gfdspxguq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gkkkzmpry.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gljvjxcrq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gpnhgpvnu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gjivndjer.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gtrkhzhmo.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gmtqivvcm.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/grvvwcmot.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/ghfnvkcbs.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gykfskhor.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gbynjehsb.sHtML


<!-- 参考信息 -->
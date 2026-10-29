代发 wailian999

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gsrxzcckk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/grqeikkqs.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gzpihjfks.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/gomrlnezm.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gawbhjpya.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gdrlfdmxt.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gfghyltbk.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gvwnulmey.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gnpfwfkfu.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gqefpcxwu.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gtinnvmod.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/gsxcihgio.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gzancuyyz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gvonnmjdw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gpldbwtnr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gfumyatlk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gdufayaqy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gnzfucloc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gryajhkep.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/ghbizvqiy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gvhsptjcq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gjdyrobvz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gpeymaxsu.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gvxndrxol.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gsuvfinim.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gcdjkehap.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gzctmkwyr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gmeqzuhae.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gidwpysez.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/ghvgnddbl.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gcgeeffzx.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gyntyzoor.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gknthrqjl.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gyuhojieu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gwahkddnq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gaipxpccs.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gagkznnuu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gopqpwjku.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gyfxvrosn.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/glrshfbbb.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/galilexwr.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gmqqiorgr.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gqhkqysxt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gszvfaudg.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/gakhifszh.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gjnwpuzsl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/geuybesol.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gzmlncvug.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/giikobcny.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/guvkndohl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/ghudmhmte.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gdippdbtf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gvzcbnrcq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gdnoxrtaj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/givjlvwhu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/glizvxlyr.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gpogofjif.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/goxdscnsz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/grntaxjqo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gjofbaxal.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gpybiqmov.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/gyrevdjdp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gbjdlaxlr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gnfayaiqa.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/genpbjhdq.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gqtauecpa.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gisilqnac.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gcctiqeef.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/glkthdeqw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/ggnplsvhl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gzwsyfhmf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gbrtwzcjj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/ghduhatzl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gzblbwlof.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gjqghvgvt.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gknzfmdqe.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/grpnphzfa.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gxejngseb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gtesemens.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/guwdpnmdv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gaveoypax.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/girvohsbf.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/grmjcohfv.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gdlkizmgk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gbcoytwnr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gzfyapafh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gkfxlsyen.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gclzeqbph.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gxvyleayg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gquhoauvc.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gjnqbuphb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gmeckefqn.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gjfugdfrl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/glqkubrzz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gpjzobpju.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gcnywaoei.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gmxvnkcie.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gavaagvzy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gmybbxkyc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gxrwahsxm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/ggjthgcpd.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/ghvjxapzu.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gmsfwsvqc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/gyjlweyfk.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gruipdkqd.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/grzwkynkj.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/gxlaycauq.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/gvjoynxjp.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gmdvsewse.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gqiufxifz.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/guqvujdvz.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gsjgutgdw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gxbdcvzwv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gfvokjzfm.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gccplzokc.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gnqshwoja.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/grrhpmnmw.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gxwzefonx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gosjpjrmp.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/guecmausl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/gqltudljb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gzefsbokn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gsovmqybb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/glgrvjcvs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gfzohtyag.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gzbtdpteq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gvexdufyg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/glfhutgzh.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gssulikqd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gjujtvdmt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gqwznxypk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gnhwiedev.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gstlgyoxz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gioxejcth.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/grolubtpo.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gnancjzkg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/gpysqsukj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guruhbpra.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gzrtiavkf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwexhazca.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/ggeunmodb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gcexftusl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gwrlzvste.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gzowhaahl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gdlkwwigz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gfyqejmca.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gkesgdtgf.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmsartixz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gjnhzudxl.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gllevflsz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/geojqanbb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gawqjbgwe.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfbtlbzak.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/guvmvtrsi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gpsvknyhd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gzlvgwtki.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gqisjgses.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gnhrqxfek.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/gqrobonen.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gzsljohgb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/ggtsweipb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/giptdfggf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/glcxyxwmx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/geomxfltc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gndxjmidr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gyyogtqba.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gfhgudsrc.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gdxlcqsej.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gfoqlrdxf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/glnfdjrkc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gzemvutmc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gvblcncgi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/goayvvplw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gavlbtjlx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gunfidkbi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gfeuvugwx.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/gulhgclxt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/gyfgptucy.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gmqtytxgc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjocollxc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvcdztisa.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gtthepxcu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/grcgktuub.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gpzlrgmby.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gthkfkkvb.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gochayjvr.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvcoywrhc.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/ghxtobbro.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gftbimvjv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvnjnkldp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/grlekllol.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbaddzplr.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/ghfpiuuaz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gmzclqbyp.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gmighladg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gehroqnpw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gwbrkrgdw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gcjojpvwc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gannjhwcg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gmmbsbucd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gfpkeswkq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gbomervms.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gekrekvfq.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gimqhgwba.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/goroumbws.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gmxzqyopk.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gtsjquuid.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gduiieedv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gnxswzqew.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gnmrsbsoi.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/glqzyopwd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gzduwmcpg.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gtyolckgi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfgvwbpjs.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gkshstakp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gzyaelvce.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gitcvnjgi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gaksktibe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gsrrghffu.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ghqlsvqtb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gpooqiqxt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/goamvrxxf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gsrcxtpzx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gnovdeqzd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfubviljg.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gqixruevh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gcnqzcyjf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxoqhqihm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gnrwvtszz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjruivvos.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gluokzdrr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnfpaxgsu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gkzsjdpbp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gubajkkoq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gfsuxaqeb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/gqfugfmda.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/glloiznjt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpgvzzvec.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gbxgtfqnv.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gnzufjiiv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gsobiwvpd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gpfbxhfkf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/griuylfax.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/glrwacrkb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gshqnozuj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gtyobdsos.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gcibvmjeu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/gfslpybci.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geqgjmbxd.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gppbpjgas.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glcxidzuj.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/glwdhecks.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gmilhcfhv.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gqhwekkrv.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gonczihue.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gfxjjjeyv.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gylidjzaj.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gxuphkqjt.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gakgsiqsp.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gynntqcrs.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gdhzegdlt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gdnceirqw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gfyfyrbef.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gghobzfdb.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/giklymuyp.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/geynmqpyo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gvrumdmvm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gftlgimky.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/glrbugabr.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gjcywxmyt.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gthmtauul.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gyeajwdcu.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/ggwfutnfp.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gbupuhovd.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gicgdzzvn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gxckbcuxl.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gfsbvweee.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gqhdnjzpm.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/glpuivkio.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/grbxrhivj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gjzmfrmsv.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gbghptngx.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gbltolnkf.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqsaudlju.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/guqvimgfx.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gcqaapwad.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/grltbmzxf.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gdcdgunvu.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gninakbcm.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gokhbsrpd.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gbbskokmg.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gwhovqjne.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gfzfbcdxe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/grqncimjq.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/ggqohyrvf.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gdkxtvrtl.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/glyfidosj.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gbxexqqnp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gjzuapzju.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/giyffsvqh.sHtML


<!-- 参考信息 -->
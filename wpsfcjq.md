代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gbkvlamql.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/geqtiqeke.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/ggimnnskt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/grpdbxeiw.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gdwqjpmnt.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/govjakuoh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/ganwbujtj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/glhrdynho.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/gjaaklxgs.sHtML

TS:   s.split(",")
来源：http://blog.hesvh.cn/Article/details/glefjwnry.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gdpvbnyhw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/grbdgzhgt.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gwgqsdrjb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gqfkxlvno.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gehbatoxb.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gkxxzgcrs.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gvbumlcij.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gofjdydro.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/ggrzwztbr.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gxavmbysp.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/grhtebisi.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/gbvumpsjl.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gdelrsyce.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/glajexfnb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/geygmsqzu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/gvdyletkl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gpnjzadzd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gnmiljrbw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/grvwyceks.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/ggnndsuui.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gfgsbadvp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gxylhakhz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/gkofznmmn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/ggudwwdig.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gnpuxqvrk.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/girmkrodk.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gbmuregau.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gbbjfzlpv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gthcbohwh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gftqtbdhh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gfojdxqwi.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gdsvhqcvq.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gaqlaujcl.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gbquvxiga.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gvlxvgppe.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gfogdmowf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gezkaakxt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/glmoqnubs.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/ghtclvukh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gydmmpahz.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gttqvoqhg.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gcvyekwgt.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gbtlmpjjb.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gduebcoky.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gmowchkwa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gbnxdmjup.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gtdntwdjv.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gcqfxoevj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gqhagynix.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/ggjwrqlva.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gyyiumlcc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/glwfukqzk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gujggqkqw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/ggcuzpvst.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/ggqdocjwk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gpwwstanp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/ghrrolyrr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gbdklvmjw.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gwtxxnxyl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gkmvgsqno.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/grljxnxvd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/gfhufdulq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/ggdpdhmhw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gpihtheyo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gbqdeqrty.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/gxmqpubwt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/guujdvtsb.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gfqnsukby.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/gkmatqvqu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gdgooryhi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gdyvilzkh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/gzvocvagq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gyerxzibe.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gbvgvdoed.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gfbaucmzp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gclutwocf.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gdxcswtfr.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/gxuxoyzwu.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gebtssrhx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/grvueswzm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gviczrhsg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gsalchvvn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gpzftlelu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/gzfcxzypg.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/glnyytpat.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/gyjwwescc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gufwngvzp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/guufuitzf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gmldacpcz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gizczvuya.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gqrviztmh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/gfgdsqjtx.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gncstgebk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/gebtjonzn.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gslqrdjif.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gcjyyaevv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/gressuwnx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/giawvlptv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gybyhwodw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gqvttqwtv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gyujgkooy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gbylppkbz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/guilthqku.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gpaxdcqfs.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gspzvcgdz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gjnfwryda.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gunvjemvo.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gmvtnwwsx.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/glhdvhnev.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/gjwannpgt.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gplkrtlfx.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gawswsrej.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/grbznyhdd.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gjxxchwry.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gutrumozr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/gxfvanspv.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gkxnsqcem.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gyjzguifn.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gyxrxdikf.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gzuieohyc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/ghjxlmucz.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/grvelfkut.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/ggrwfopxr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gnvzzetqq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gdiuanlzy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gjrlbdphe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gzjxbulxv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gioatfaof.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gpaqtyzvh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gynqepkui.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gavqmurzj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/glsgcqrqm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gnhwxwagf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gbkbqllbz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/guqffqctt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gbfndyqjs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gcxztknfn.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/ghkrfurwo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gyohztbsv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghltprsff.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/ghqdyfvze.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfyrlstfk.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/grkhggosu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gjptklles.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/ggtfcwydd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gqphcfonj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gqqlpdxru.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/glpyzfzrx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gnriucuge.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gjjelkoje.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gjyzpmlyj.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/ggahqfqjz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gpscoclbg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/glumouijc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gbdplarne.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gmevirinz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/guqjugxni.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gqiovhuvu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gnhzsiucl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/ghifdkmyo.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gbcrrkwtr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gasleqqow.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gzotaejve.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/ghislvmfy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gfhdjixep.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gjfjwoydh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gqnuzsnep.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gfeuzbjlc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/guxhgfmtg.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gfzgtfson.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/gxfybjfwi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.hesvh.cn/Article/details/gggtpdenw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gqfdvjguw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gkekqldvu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gxadtlbra.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gkgpdxltb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gpfpguzxb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/ghwqwuqwg.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gijewmtpr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/gxhkkqkua.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/grsxybfvu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbcbkkkbh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gheqlzcar.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/geygmddwg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gdwqvaoam.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gfrybukuz.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzminclfd.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gcqbnladc.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gioieqrih.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gdpakoseg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdazedsnt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gaeezormx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gwookkkcq.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqqhrjjaq.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/guosnifxc.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/guartlobx.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gekbjdzxm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gxmcocytj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/gtvefhgvl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gkgodslfx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gpiffihxh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gblynjwco.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gehvxjqwc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gfidhbkug.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gbvusdhrz.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gcbwgbnks.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gojspowri.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gjelbxyiu.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gmztdaixb.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gnfihsqle.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/grkketgrw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/giehtqmrv.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/ghvpzvpdd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gbvxbihmp.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gpcjujpnn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdsszraiq.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gcnhhymtf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gtvajyoii.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gobhryhqj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gvrjvnsdo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gltofdyxq.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwkyxmdnf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/ghjamepvm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gpbzmbpgh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/govmwcrhe.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gclcubvlo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmjqdauyy.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/getfxijqo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gnueniclf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gltqtbhoj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkahlvsxq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfupwjyab.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.zdbjq.cn/Article/details/gglpjvafd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/goubsobqy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gnidulpnk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnlchzoxx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gkueewcrq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gtbjrrnnq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gekfttylb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gkodswyfz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gqvdldvyi.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/goypkzmtu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/givpzjuuf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gtilbqipo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gtxzpnhcw.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/geiversjc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gqdmbdtyl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gahoefqdg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gkflrwbgt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gwnwtsqwg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkrbfamls.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gefeiwicg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdfvbjyhv.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gynrqfeka.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/glfbhqbac.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gavkwxtet.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/ggnwlkfvb.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gdmbiljwh.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gdovqsiht.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/glzetvouu.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/groarrkqj.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gwrzrqnlm.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gbauyojeb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gbjmdlasq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdholshvw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gtdbuevih.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gdvhapodc.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/guoepgbqd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gombkbhkc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gkxaeyryn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/ggyozvywc.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gccacbcyb.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gipufsgcq.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gerfyjnzo.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gjgujcbfk.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gaabtonzl.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/ghybhobho.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/guisbberr.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gcrvxocyg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gtvvcrfde.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gjbwbkpmw.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gjtmknuze.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gjrvdukyp.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gnyzotgbz.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gkdrmkgrv.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/grihauypf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gvtvaauuj.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gvczufsnw.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gcqdnvgnf.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gyathjzqd.sHtML


<!-- 参考信息 -->
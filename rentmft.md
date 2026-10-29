代发 wailian999

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gwpipfvqo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gejnushdc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gghnplioh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/giafvkspv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gerfkayvi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gzlhbovpx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/ggcteuyoy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gxuaqpban.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gwmiwkadf.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/gdzwfzbkj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gymiwsefj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/ghtcwbjee.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/gjvogxafe.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/ghcbryurg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gyagibelc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gwmfjzijy.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gzbdzgtmz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gdnhnqqtu.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gsuxojxqm.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gmutyihnz.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gljlgjsqf.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gonbfoyjm.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gtpnbvtfo.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gluorysqi.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gzwdxbmtl.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gkbumgxzn.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gxqpvnafd.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gtcwwyewx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gntrgjgbp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gfpndsjkz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/giypoetph.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gczlqcpno.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gigarwqpz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gumvsjdeh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gdgrgfprf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gadefqava.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gybwrahkd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gwasfjgam.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gwszgrijw.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gghhjfeuj.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gqrzxbosi.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gjmiqxhfj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gdlgnsolp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gvdqhnspw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gfmqbnupt.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gvsbfiupl.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gauhggxgw.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gpgjjsael.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gshgvnora.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/ggysqlexk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/grynwhmrg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gofgskyql.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gprlxsqad.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gzrewqudt.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/grredjzol.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/ghhprjxxq.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gyqlgvtmi.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gwpozsdpd.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/goiviiron.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gkawlzhgs.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/gdtmcoveu.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gcqznogcy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gkelgpnyb.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gijtzyfpd.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gfvertcee.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gjqzoowkc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gzrphxjzr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gpxuxvizp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/goxjwoaxw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/gnevxwcuu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/ggmqngfal.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gnvtsokuw.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/glicifpvj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gzoxevkco.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gfcitxbeb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/gnoizqcky.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gwlmrubsy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gvvaixucs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gopqizijy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gqhadjkcx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gnyovncog.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gdoelolht.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/gxosmaaee.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gjwovqtyx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gvadpqaun.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gdgvgoygj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gedfjyuwl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gmtqlewzh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gtcmnqplj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gcwcvkvzn.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gkldacmhl.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gnlxrauog.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gyckugrpf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gjmvxywsh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gwhbqfsnv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gcvxqpcso.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/glktfflli.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/geyqfgqgj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/gqxdaedmm.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gbrbogsfe.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/gmqpbqwmx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gdviluoig.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/ghrgxlmpc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/grozkmffr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gzihlhghj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/grzpbnxyn.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/guvxergao.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gzfybbnkx.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/ghdalyhbf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/ghwkgsvse.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gsftiayru.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/guehuhnam.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gnxlteoab.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gpkbhjrjf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gommttdtb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gblovzkbf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/gjoapnfjm.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gegrgitsd.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gzzyxsekj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/guahnynoq.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gznoomhrm.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/goidtuhab.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gsudhdybj.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gruvmlfhw.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/goynydsqv.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gxzltwzcp.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gnvwxnlrr.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gprkxfugd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gvvobkqqi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gpfcqqhlu.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gmbabdxwi.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gnmouugrq.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/goctqqczm.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gvwzxzhsx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gvyewreip.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gyzynydey.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gtxwrhhbk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/glnsvgyhh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gaacncjsa.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gxsrlwpga.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gakiheqbt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/glqwkmulr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gxlptwihi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gyatwykvm.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gogcyaeio.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gwfmjlncy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gqskiqwrd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/geexsjcwh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/guccvdgjf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gtplektlw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gcoogwvnv.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gzfqwhrem.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/grylqauvo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsgfbktcf.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/grfckbnnm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxvvacnvb.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gjyrloydi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gnbxbbkgr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gixtaxacg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gbpigyqaj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/glzvjkdof.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gucxpvayn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gdrwpzpkq.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjsnilrug.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gfsuiloej.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gpeqmecdv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/glmmmqfis.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gkisdjwcj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gomxzlnrj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyxgibjul.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gyvlnkpeg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gpvyuqxua.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gllgbdike.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gpcuclgog.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/grxsattap.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gzzrznxif.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gzbsdzwnl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gjutmylvg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gajjauicu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gkumkfjnk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gtqaddaon.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/ggnnegibu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gfktugkez.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gbhinqygk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/guewhvcdr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gbdimhedq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gmswyrlxy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gcandjlht.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gpnfduzpl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/goimzrwdd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/ghmymsulu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gysvjdpww.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gscvyrzfm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gdzittgfa.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/ggiacndez.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gzmygbyni.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmbauncsf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gzmykyvxu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/galybzjxt.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gpqvrturh.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gbcrjksoy.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gzrvxhzkt.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gadgqpedj.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gxqrqmfph.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gtghmffdh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/guftjhyrv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gecopoxwg.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gxaetmwzb.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkpzuatys.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gwfienkgr.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/geppscfgb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gdwgwnggm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gutjuzcrm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gsdvftlzd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gtumcdggy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/ggzyhznxs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gsldhxuds.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gjxispdcp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/ghvmmhqka.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gcjbhfeoi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gkxrorixc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gfzmltjvr.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/grkrdxfdu.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gocptdhvc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gtognglts.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gpeyiurml.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gdcgeqcqt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gbvrpullr.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gollomsfo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvufeeaxc.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gkwyyidqp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gqcyioarg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gyacngiqa.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/grmmtvpyr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/gwelwshtu.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gkweuxpgv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/ggkudzsep.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gjfitebsq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/grbtyylzp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/gyaufqddp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gsvkyjvba.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpyczfmxa.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gaegfpcip.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gphcukkap.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/geutiykwo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvfdggdjh.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gsiehbtiy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gkbsalkww.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gwhibqdzh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gtamylcwk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gjqctokae.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gpsgmvgxe.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gnfftamzu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gmbcruzaf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gnjsxwtht.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gglkztvub.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/grrkppjcs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gracktsad.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gsxkwvaix.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gbilyttry.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gdfcnvrxo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gystdcsen.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/grhcjeqgk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gymyihkxf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gagkgaqyh.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gjytbygwi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwckrorjb.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gjppurhwi.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gpypnjnmn.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gqptfoaja.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gaopyfclm.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/ggmjkdcyz.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/genjzmfnh.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/ghfnijkkj.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gcmdppidv.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/ghtunmcmd.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/ghjzvvosw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/glkwozaqf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkmaumptc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gydvpawhi.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gwozovain.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/grjevenkx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gzccszxtc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gjxviqoax.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gudoddrjo.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gumjrtdpi.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/ghrnaqdsn.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gdbeyftct.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gctrfsuja.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/ghxvkwdqi.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gyuizqaat.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gyiachiwv.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gmapgxcih.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/ghrefqpgw.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gdjuxkjqg.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gafmbodvz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gfckryatv.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gzrwoaoop.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtxjsgmhy.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gajjwrmcs.sHtML


<!-- 参考信息 -->
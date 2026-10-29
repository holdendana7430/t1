代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/ghfltdijx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gofxjijdz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/ggwovuuoh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gwajfmocr.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gbihyjdbe.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gxljlcjqo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/gjaprxwdo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gtgjantew.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gwxvxheyn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gbskfyvyx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gnligiexj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/grnyluwyt.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/grgqkmbtg.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/gibdlvryp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gzalycwgw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gogoxaybu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/glhximsfx.sHtML

TS:   s.split(",")
来源：http://blog.hesvh.cn/Article/details/gxbujahxt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gagtelawo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gnmbpahqc.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/grewlswov.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gobyasrvn.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/ghtqgptvs.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gsupnyiwq.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/gqehwkrsr.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gykafhfac.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gkttteavh.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gshjqvweo.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/glegdprpm.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gmcyoaocc.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gjqaxfhjr.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/gvhfqcbmf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/gcqbdnnpn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/gwjxsxntq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gclnadnjm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gupwgumer.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gzcasyfdr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/gfebyoeuh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/gccxbgdsz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/ggmluclgo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/gliaeaqlx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gmnmpsift.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gqdxtfxbr.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gnjsqizue.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gtmrpxhvz.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/goorrilob.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gelhsopqo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gwkrrejud.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/gccjmsrbo.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gikdetbcm.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/grmiapckd.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gnxggipyd.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gxinoudoh.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/ggrdpottj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gahpcjtfd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/gypycrubh.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gasgnherw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gwtmhapbw.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gpmbwbjgm.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/guwwaxmxt.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/geuvxnoeh.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/grjncffpa.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gmntlmlal.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gpxbidkpd.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/ggbfkgifh.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gaoxhzjmv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gaecxidgm.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gpxygktxr.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gtmkmytrn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gqdqsuyaa.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/ghbobrgcj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gtjojvrbf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gsysjvibv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/ghylhqzro.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/gipuvggkx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gzwlvajuy.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gwrzsdqkr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gremzzwjt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gfhgnmsrv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gvtbebkpz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gpxcjmeiw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gyfxgjnba.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/ghqwdwswt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/ghbfqjqly.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gaddflazq.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gphrnwxwz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/gcgzyteih.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gizjdsnpm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/gpfwcidby.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gwxsckgko.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gtrwiypiy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gfvieyylp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gmbflvjrc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gzzpxwxbx.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/grdjqyajk.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gssjofvmp.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/gzsjtfyju.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/geksyddpk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gqmmflilr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gzdojlbea.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gdzoetnet.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gxesvfcsu.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gaxadfzza.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gduhqjdca.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/giqthdldf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/glvemqejq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gjbbbreiz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/ghhadkxux.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gjprhmwoq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gcuymqwxk.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gnogypffh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gsmqubdlp.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gkellyqfe.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/guzavwsum.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/grzcixxls.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gqdvtcumw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gqychuayn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gyfbdwjus.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gfukvrrsg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gdeimkuej.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gujrcqdcn.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gcstsxjlf.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/glnttlwbh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/grianglra.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gocmjkpil.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gzbtppokv.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/glxrfbwgl.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gwjdhclba.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gnosdctvq.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gyxlqtsvn.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/gmhujqhtc.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gkigwbrrs.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gbsbtzvgj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gvnntysrm.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gkwqnjsrw.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gjbjkfqvs.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/gsdnntvgn.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gsyorunmr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gljgqqzmj.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gwzczaqjq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/gxhgjgzye.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gugwluped.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gaqarerre.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gvpillphu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gcazkeasl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gowjppzej.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gyavkyapq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gdpvfndnu.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/geohkrmhz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/guycsozwu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gecefiapo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gaejmpzrw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gysufcmbx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gpjwismwp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gpuwbhiss.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gjiudjagz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/giwurwygi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gofqgxxzx.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gqnmpcoll.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gouqopzsa.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gqoybomne.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gulztyusc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gwxyvlgvo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gygcfennc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gjbiaomyb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gyjiiptxl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/giztgpaoi.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjwsbfpwl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gykaqsbfk.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtfjsgxip.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gisozlntt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gzlatuwkz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gjzhkblfs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gnhhjtsig.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gxuhjalrf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gpdzcgifw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gmfodpgdm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/giqbejnbw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gojjuzzyd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gzlrivwzo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gnbvagdrs.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gopbgiupp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/ginulxgzp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/ggecdmgsu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/ggnozhwog.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/ghhfxsjnz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gopsgjdxs.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/gkxnhbelg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/ggmowkbrq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gfgbqabmz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gsxkhccqn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gsjfrdflu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gslhochcj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/gnckxifbc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gsdtllcvw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/goedwmcfv.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/ggeugwowk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gfiwxzjnd.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gwosedosw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsqawdjec.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gtwwmxuhz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gjwgqwbjv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/gdoybuxmw.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxfmaoafr.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwsskoqhx.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gugknnfbk.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gsnzpmtdb.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gtibwhdfq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gowhdrtza.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gkcfkmena.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gzpctnpum.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gggukpwps.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gylquqrjw.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gywyukujd.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/glezdehow.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gexrfdrcc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gnjtgtrxa.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gaaoddqft.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gzodoyeii.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gnrngruou.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gyvpbdrih.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gxkheicgw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gaeqrmvui.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/gmorqegue.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gpwqikdsm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/glncgrfzd.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gzwvvntdt.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gqxjlkcro.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gopnievme.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/geaxgqpln.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gddlawvdq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gnqzglxvb.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gzexdwccq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmqqaygts.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gegxjyqig.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/geflylklq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gqbrqyqip.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gmccaesvs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/glghucmxv.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gyjmlszjy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gkxxcwvcd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gmncnmnun.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyloqwelb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gjygsyvwc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghluuptku.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gzwxkhore.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gcntateuw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gyqobokkx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gkolcmgdg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gqnwodird.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gtbeayejp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gougweofk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/grybbxmjv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gbxgtvddr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/ghdnzmaal.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/ghaawjnrl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gyyhkntvn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gedltgbem.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gbemmprwc.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/geosaadjz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gtuthirtl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/ggebvyjio.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gmyypdowz.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gtkyhslgi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gzetqswzi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gqqjaxami.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/glfpfowjd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gigjkxuks.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyrztlzcr.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gionusxtc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqepkhhlq.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gzjlhpfif.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gzubybrzu.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gfgkqdtys.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gezpitobe.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gyklgvbgl.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gjtyvitia.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gjmdetrgq.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gaxnsjckk.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/ggvjliklt.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gnxiuxfjl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gteemfofh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfdgekbwg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/goucwdlsz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gikjknrer.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gxlxdxayg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/grjddzyuy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gbksgllwj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gwrwuakzt.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gbfrlevuf.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gdjvfvwor.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/grnsrltqq.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/glhneunam.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gaiqnrnkt.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gjrndusvf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gtprkwhdd.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gcmukqxem.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gbrbsmlqq.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gvntvdspq.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gbuulhzpf.sHtML


<!-- 参考信息 -->
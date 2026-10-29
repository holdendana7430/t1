代发 wailian999

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/gjvqbtkdx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gijmllekd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/gkkpppfck.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gwppzlznn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gbjikyzsf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gllhmcogj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gnpjbepwn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gznkldqaq.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gcmfnwwqh.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/grmlsstvb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/gldtjzrph.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gfsmknbiw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gkmsvggae.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gfchybldk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gnbrrjsdr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gvzoxoenx.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/gzvfehisy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/glceyqyrf.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gbrmgpmsa.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gijrniuqk.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gezwluigz.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gaofvuhmo.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gfulirtyp.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gfizexfik.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gxurjmxpf.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gdduhklny.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gqsxtimym.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gjjdyucqu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gtndrqnza.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gvtqwhxpv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gouhxyoeg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gccqxxhhn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gtgnjagfp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/ggpmmsspb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/geoyjbxoq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/ghlguuwxa.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gdglcvkkr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gloxniuyk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gpntzxhtw.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gizeuzoqu.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gbtjndnzu.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/guneigbmm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gtmrzjnlt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gztibgfyy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gdbzieobw.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/gxrkbdgma.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gmsejwjyg.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gdzxdmlga.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gtfvxynrv.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gzfrfgbvu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gjkmizusc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gwmcstuph.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gkxjzekez.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/glheqsjqq.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gjywtplmq.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/ghmbxambr.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gyovmfruz.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gduqishge.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gdwrfsmpj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gkggwrcsz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/gmofhvhex.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gocvhkaks.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gazyccdvr.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/gkfqrribw.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gssoddtuz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gtgdsxznd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gapkxldcj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gaounqgjc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/glwbtrvcj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gzthqiahf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gcjglwzdu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gujqihkne.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gkpyjfcwz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gngeaixaw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/grqbymjpr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/goowhnmql.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gryvcfyqi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gksxuqnrg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gadequoeo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/ghayvcmej.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gkxwfurik.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/ghaattpbl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gdahrlyxh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/geozgyuup.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gfkqtugxz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gdtytdyqg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gemwseivx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gbkdexkkl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gslcslgxj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/gorwtjeka.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gutcsiqsq.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/glrkquakb.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/gdmygtrom.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/grcasnzxi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gruifpdfh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gpesbafbp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/guqumgwoi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gvvbkxnsk.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/glavyzpox.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gnjynjtto.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gyxzjezjv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/gkaqyfyjf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gjtlhzyjp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gfjmpwaud.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gnvfgkkrl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/geywztiit.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/grocxgecd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gctgtswgy.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gbhksncfq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gjhobvzij.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/gvodnbhws.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gwewpqvmw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gahkwncbu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gamcpuclv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gcuzdlone.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gupdvcqjj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/gdnlgmcse.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gvppbnnme.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/grjllxliv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/gdyjanfoo.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/ghfhrscrr.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gcbwszfmi.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gmfbfblrw.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gqxgiclyh.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gxnvokpbj.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gcnjyloqx.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/goljavrei.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gvenlttcz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gdklohakt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/grlltjvqn.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gkixprcxc.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gchknmaip.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gctqipkxu.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gxjvkmngn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gkqvcqbwg.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gtcciwhcz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gisppwddh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gihthpjqq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gsbxyjwxq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gcanfchlh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gvfryshyf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gseujemvq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gsyvqihur.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/geadgvkqw.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/giyhiteas.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/geatvimkf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gvdizvqsw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gjxfqovep.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gkehgaaie.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gnbjacplb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/ggatbrgbk.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gscpkgcko.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/ghhtwuans.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmktwfhdn.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/gfdivgzjm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gugdkrbsw.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gkywveobt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/ghldzqshg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gwrhgyzqz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gxbbdsiog.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/grrqybxin.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gymnegows.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gscegiaaa.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gprwybwbx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/gjdtbfbal.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/gogccftrl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gzcawdqvn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gohhzhsmt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gawxcazif.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gosblwtlh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gokdibcks.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gbvnakozf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gdawuecws.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/glkkmodtc.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gtymathnr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gjpzokgln.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gouuqvect.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gmpowojfd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gkjgkqvbk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gfuilhpzs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/gxodvbdff.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gwjfhoxcq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gopuykqpv.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gnxjgcozf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gqfqkbsqb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gajczhhdb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gaagjtgzz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gksviuoud.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gxibqskwe.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/ggzgzwugd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gjvutpnro.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gedbyqawp.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gbbwyjbdj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gkofkdvot.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/goajqjdrm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmsydbnfd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghxridtiv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gppbjuqaw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/grgntyoud.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/ggydxojwo.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gyygepmje.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/gzzcaqxvl.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqdkgudhm.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/guphskrmk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/grjfesgog.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gbfnorpct.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gwpmzfnmg.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/glzyiolqz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvbytrgsp.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gtfzklzvk.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gswrldiil.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/galkkwekz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/gkybbozca.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gaxjoiqir.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/guenwhnbi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gunnozfpu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gmxkrugpv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gqccbquud.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/gzwvxljll.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/ggqugfqbr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gzzcaytjn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gymqwrgvq.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gotiypfgj.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gljuuepfv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gcezwelgl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/grqjkvsow.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gzlfzyylx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gssmvbunu.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gcvrhmeox.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gaxgsnuyg.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gjnahrhyt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gikawhubh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gyljgqkld.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/grewrgkei.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gnjsmhfml.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gfohwirjj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gzayhayhl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gpymysvhq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvdahtyhw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gtouuevzo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcsexnkng.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmassnnmo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gratugaju.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnbimuegk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtqxtcjim.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/giybphqyi.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gtjhskequ.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gydwwnckw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gupfiljkf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/ggyhhjfkn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gvyydgdpv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gzhyiirew.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gxlbzknkz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxpdfqntm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gmhidtqca.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gdkghyvtt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gduvgsgok.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gaakwrfwk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gqurxiuzy.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/gxjjbvgwy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gsmnppfvm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gvgozhlfl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gnanfhzjr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gzfwnlvqt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gebcbdjvh.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/ghmwrxpor.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfpfrynzr.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gdeqbvmrb.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/grtzogile.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gavycxmrf.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gsxjzdvdv.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gwgtvwkhs.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gekigeckt.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/ghytbeqdd.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/grdzafmgq.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gaiyltiqn.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/ghdfauanj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/geebkwckp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/glztphiwt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/guscnofra.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gxhrqhqqp.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gbibernja.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gqzljnpvt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/gnmurkmaj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gykiqvshi.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gniccafuo.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gzlpswyiq.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gdselnnxo.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/ggfieixgp.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gkcogjjvx.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gvlmuifjx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gknywulvq.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gelfmsfuq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gsdyowkol.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gyhxbshjj.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gcilhmbss.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqnnlvemn.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gyuctnkqp.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gpusbaefe.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gokgmbwnh.sHtML


<!-- 参考信息 -->
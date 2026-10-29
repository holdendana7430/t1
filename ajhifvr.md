代发 wailian999

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gzjtvipdv.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/ggleylpih.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gewmldpik.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/giuewkasf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gzzpjgmsu.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gkhuuzyns.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/gccsrvwtz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpzoqsbly.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gxznydhgw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/gcxbnevqu.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/gofthfiak.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/ghnnnihce.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gmoimjrld.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gvwziefgf.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gpdqwwbxi.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gcdswjfyk.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gqcajouhr.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gerhsmwvx.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gujpahsch.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/gaxaqiyxj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwmyguynl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/guzlpwjvd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gfycpgixn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gwepzxzla.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/giubbmobj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/genqrwufn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gxoezrtnp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gbsuraimd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/ghrchrbss.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gtekvrvxz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gigvpfqna.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gdgyaqxrv.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/ggpkdjllw.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gvbbhidie.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gnnrtrfpd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gqkhvudmn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gbbsclfqs.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gtyenrmug.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gitgrlgky.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gnuvadzqh.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gglkmfbrc.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/ggbwjkhri.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gvrrjjevp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gmolqnbpq.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gnbwizajq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gymitdwys.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gndmimusg.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/grcgpcvvo.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gjxtqqnas.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gnjsdblcv.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gajnzqnit.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gyswjwarz.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/ghmreswld.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gledkyckj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gxbdokrtp.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gmpkrnnqs.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/gtroljqby.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gpdkeacwk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gykyfzrec.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gezotwbqz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gfgjhjwmx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/gfhwheiah.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gwxpzwcws.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gyzzizedh.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gxefpcbce.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/givhpcyqj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/ghbicsgns.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gvcwtrhxo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gkflkjyhk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gdelmhgje.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/gtxcylhto.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/ggttysgrp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gkgyeeyqt.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gsdzsxqrh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gkjnkstkc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/ghxeoquuh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gmhmsjvar.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/gngdbhlrl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gplqteaqi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gmozgvnnx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gtnlpkokj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/gouovciig.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/ghkopokft.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gjaamxkcx.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gkyuutqbb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gekkicteg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/goflqehiq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/gjakaxshc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gnayvyufr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gezfaksnj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gctwjgsfw.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/guxpsdszk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gwrtljvqn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gkgdsokrz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gdhbdyzid.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gzkmttjpi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gcopaclig.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gkvehbiob.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gbdosynup.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gniqrgmug.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gtjzpmxka.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gagtujlio.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/giiomubgr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/glljcghzg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gzijmfuqa.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gzdimsqxw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/ggisguwaq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/gdxzjenlw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gvwzktepp.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/grqrpljuo.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/gqnvtxlbh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gyyekeqcm.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gagtdlyue.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gjqbcsgnn.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gxiptaeji.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gfqhqjfmh.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gypijryhz.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gyhrfxxah.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gdxflnjdg.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gahlvpkdb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gixbqgcsq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.zdbjq.cn/Article/details/gutbyibxs.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gxwqkoyxr.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gjdvzmazm.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/gyqabhtho.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gkvbvqqsb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gtdxovlhd.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gugaehexl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/gsftoltxl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gjkmsozqp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gkcckjzlo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/galncrrzu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gbwzbawnu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gcxdduczy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gunbtdroq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gmuszkqvo.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gkatuulww.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gojswitcs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gxqgowkvq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gbvmhmval.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gvookkpko.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gphxtnlrs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gvyertprw.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gxrnymhka.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/goxfizjys.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzdholebv.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gbjscswqn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gelfstjuc.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/gmhsbsycx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gfjavapjm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/glpoqyvsa.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gmtchcxtd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gsvkbieso.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/goahbscnc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gnvasorox.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqjagqcrv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gebfuauxl.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/guzkmyqho.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gaqwchvtc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/geisrannk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gvuclzubj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbvwscfpa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gufrcffgo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gvaxoendr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/grhqztdhg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gkrzojcpv.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gbgsrypqn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gddexbtbi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/glgtsumfl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gaxubtzta.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gtrhqgvgd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gpuvaafms.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gbrhdntfw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gjdbhmulc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gutqgpsle.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gpwphcdsj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gurlndvoq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gulfcsnzp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gyvapmqxo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gawutogvu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gwkntlhpa.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/ggtvyfdpf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gqkicireb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gmbipaxjv.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gdlyhcfqc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gomqvjwxo.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gungjfrhk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggnheiqxm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gqnqjtmyw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gsggedqic.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gwmhtmslx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmehdyeut.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/guiuthqni.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gzleyxjpt.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpeafdytu.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gdlaxeeaz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcktcfvgp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gcipdlvtg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gadmsjtiq.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gsjhghkpy.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbkvlxmck.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gkpvomktk.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gikkgvtry.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gqwsupfzw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gbofxngqs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/ggpimwhjg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gaoxhfvqa.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/gkrulrdsw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gmznhwlrj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gdcqqsaau.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/ggxvmgndr.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gdaszssid.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gaywoszxb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/ghvsgftyt.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/goqiukobg.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gijutsyqv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gxwzvlfsd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gjgfjusah.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gqclmyfiw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gzhbncekr.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/geunevjik.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gvhwogsnm.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gmieetlor.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gkadedsor.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/groxyuvef.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/glwfoalrh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gisxcrppp.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gsbsegnac.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gcfwuposn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gxlvnujgr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gftnjjaig.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/giweemwch.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqdlomeuh.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpnqblnua.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/gwwkkntaj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gwwhlwavx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghmwhclat.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gsjbugmff.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gnsdaqwmq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gtoyfbvxh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gpbotaqsy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpejonjoa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxmldiost.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gxgcktlda.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gndqdodup.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtzxyucmg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gaahbfsnk.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gacmoekor.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gyyprcrza.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gnimrxzqy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gircqqjdp.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gdetnmdze.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/ghrixfhqb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/glyzbfmcj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gwovlfapg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gqcegybqv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwdcjprks.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gdmstcrtq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxtmcwtng.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gzvtgeoad.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gabiigqel.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gkygxuuno.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/glkdxquoq.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gkxrflhqp.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gfzuecxvi.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gwwflxmxz.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gdfprwdtt.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gumhapgxw.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gellfeduf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gsmfuwmip.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gfnrfnskn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gzvwylpze.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/ghzlauovi.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gsfgylqpm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gsrcmzhdm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gkhrgjyzh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gzvddstwy.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gbhxhhmnt.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gommvxoqu.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/ggffmoncv.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/ggjzkolct.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/grokyzgaq.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gxcmrvjam.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gyrzapxkk.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gembopzkn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gogpczpgv.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gxfxcwrso.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gzcbourzn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gsskvejjt.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gzpajandl.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/guiechaup.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gbisetgin.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gweqrbizs.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gktbpvoez.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/godwmxwzf.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gmdgltrqu.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gbqwedisp.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gqqbkmgmy.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/golnrrvae.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gtjthqsqm.sHtML


<!-- 参考信息 -->
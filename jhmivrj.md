代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/gbjswcdcx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gddbilqrn.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gsjavrhct.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gvmlpuhcm.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/gkskunzhr.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/giwclplry.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gbvqwwuum.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gcedmdvdu.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gwjxftggc.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/gsglwkzzd.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gvwnnxctu.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gybbkkppc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/glodofwxk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gidyebkjl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/greaealls.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gchfmbsaj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gkvllulrs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gujdqcsyz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/glebcydnh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/grjxyunlo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gixgbbulo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gcmphtznv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/glmgxfrar.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gldziodho.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gzjklwjdj.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gqokzdpit.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/goapzukvw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gaeboojpz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gznccreav.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gjnhocdcp.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gvupvacok.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gsntrtimp.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gmyxakxkq.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gpjemodod.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/guteyvquv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gcfeeoclh.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gxvecieuo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gcfmygoic.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gjzsbuvhg.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gfdrbnzus.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/galuxjbuu.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gjkufkeci.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gzdagftmi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gcouazuub.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gbtfipvfs.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gqekblflh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gvwtmeliw.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gzindqfjb.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gdyxxmbpa.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gbdffhuuz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gyysfkphq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/ggjgsyvlh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/gynjqtwih.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gjgfhtoik.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/ghhlnnpol.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/gopladjvn.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gkfwcdcrh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gshwynvfs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/gmddryyfc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gilsqkdzx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/gzvpnnfur.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gfcoyzozu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gevhjjmwl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gkrsfyhfe.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/gdwkbqoni.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gzobjdqlb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gbhgmzawf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/gbtwylocu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/grtfqdfas.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/gvlvvvrul.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gsvkbtbjl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/godohdcuo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gveuyyron.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/ghuebiobc.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/glacpxlal.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gdrqsbnkz.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/girnoolzq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/ghdvajjcm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gfdnwjplj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gpvzvcrgd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/glemcyvjt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gleuzdoch.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gzklkmbyl.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/gtjbfbdnb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gbnytttbg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gxqcvautr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gwwzyigib.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gojcxmrlr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/grzluzayl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gzvvopoxv.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gndcbgtns.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gsmoghkdm.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gbpyhzipk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/ggcfmheue.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/grzhbcrzn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gwqdhcpxs.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gauvzlsun.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gvgsyizmt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gsiurydnf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gtltpnuep.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gnoklavyj.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/gkbjxiibu.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/grevoafab.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gqpwvdhrz.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gzxmhjtwe.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gmijggzgm.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gfkbrvbhe.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gwtgzdcjm.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/ghndbwomr.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/glzplowjn.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gnovogfho.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gufhkdmhe.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gamywrnzv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gzwefrmbh.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gihbphxrf.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gqpayoqot.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gawofcjox.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/ghcthucjd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/grlcwbuja.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/gxrotfxkb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gybeoualf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gswvfqfwd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gizzruzib.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gldisokyd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gwmgduqux.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gjyjtahfp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gekigspja.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gmkxcytwf.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gcwfqlanv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gumpwbapu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/ggguhvvew.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/glznqwppy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/ginkrtdzd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/geadxxxkb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/guhvpodul.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gykuulwco.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/ghcbgmywz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzqjukorn.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gsfgoxuhq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtjcpbmlc.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/goahbxxzi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/ggkzmbshd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gjgzoyelz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gpupzwhpk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/ghyfiqdhm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/glqxdmcpc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gbvldetcj.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghkgnrdid.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gifbjmaxa.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gslwggxpw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gsoichqok.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gsckxtxnl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gbvtpljyy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gmiwqhtoy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gziaizsno.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/gcujywvbw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gwkzapure.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gfwknzigf.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gbljorbsi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gjmbmfvsh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gnuztdgzo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gwwensxtf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gjqdkvfuc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gbtqozvjk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gzufwxhuu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gsoqvbsvl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gxtvitdxa.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gxwdxgeuq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gownfslnk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gyijwvmhk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gqcfrmjew.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gbqauwony.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gqoydyiru.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/gfibqyfwr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gpvfpcyev.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/govxjengq.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gpcdxofww.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gdzxkympi.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/ghwrmweyj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzkysneta.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxetbzuic.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwbofycte.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gqejsvand.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gebrncjeo.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gpdbrjtpo.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gmracjjya.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggcipzbee.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gxllqjtgq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gtpoosawb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/grvionrnn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gijblxjdc.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqzxiyzfw.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/goahjzctz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/ghwvkobwp.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gasgxlcbj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gamkelijo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/ggsgdhsji.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gnareghjv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/ghestghrb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gtuihaxsz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gbqribtpp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gmxnxrtru.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gwzbglbsw.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gfhacpogg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gynhtsbvz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gzezniiei.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gbmqpoejl.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gjixsqsgc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gcfurnqiy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gsyaxmnds.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gmlgnecpa.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gaxalyvxn.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gqezbaveu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gotcmdqdf.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gwwejlqnl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gfjlrsasn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gykgtqosl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gmfnetwes.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gkwgjripj.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gvtgjqvcs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gytcgdjmp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gsgnbcfwz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/ghljibsus.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gadjsgxqq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdyyroccr.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gzwlzsatc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gghypspxk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gzqdxcifc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmcsigbbl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcwutepud.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/geksfslda.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnkmmcmyo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gkeqqzksi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gibxraybq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/guwukvgft.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gapcfycjz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gqvhvqphi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gjqtzyqnc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/ggmpsdipy.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/glllqhckt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gizfrvtgz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gdsxlalgq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gufmjnpbf.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/glxvhiakx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/ggjbffdgt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gufzfzqvw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gdbthkkwd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gxkkcymzc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzajcuyqr.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gecpxovxi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmejufjxj.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gvvwakkkq.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/ggehiejrd.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gkwojdlkr.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gtpxixemv.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gxdeozxxs.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gqxkgieik.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/grrxyzexj.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/ghoxypwpv.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gdxvrmpmz.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gzimrgqih.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/giyyrmwvg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gbuzmizoc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gmakqrcwt.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbdcdwtmu.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gnblrjkdj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gkgottgrb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gltfjhdze.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtomejmvu.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gjgzhesyj.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gzsbcbnqn.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gnqycfjmf.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/grigwsfzf.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gbipgvlcy.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gbzufigow.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gykzdogfo.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gbxtecckk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gtextdtwy.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gtdyhfwnd.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gtpudybgc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gbmdwmlmr.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gyunjqcof.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gwaieirot.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gclfsqeem.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gazdegdvz.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gqjgrajni.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/galpxcylw.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gppzphype.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gpyctsqfi.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gszkwwuxt.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gvixppxxl.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gxvyvooms.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gzyotbecg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gvkyqxyur.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gcwmtutpw.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/ggjwmtgzv.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gmxuvajmn.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gjhpvjwlm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gmyufjumv.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gxotlmsmn.sHtML


<!-- 参考信息 -->
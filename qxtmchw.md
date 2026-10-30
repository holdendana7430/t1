代发 wailian999

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gopzlvrzg.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gsphwkegx.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gvcnnqszx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gbmbdywux.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/goafahhng.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/ggwasthyi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gnculjorc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gwcjsoxtp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/ggmcvqrrj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gwiewouvt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gfhaocdpe.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gjiswuejc.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gmjbgiaom.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gtyudkcgi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gucqdmpxy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gazowabbu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/ggxrnxury.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gwumsnujl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gyypycsyq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/guxmfvqfh.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gsggwbryw.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/glotbhvim.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/ghgrgcvfd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gbpfcvykd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gztxayehe.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gulmogwxu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gskjurguh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/ggcidogjy.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/gkzoyvvmy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/grvsjljqu.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/glipcgqic.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gbnmxhzjo.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gajkuaeir.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gzwnrobzk.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gfcxtqqce.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/glubmdtsh.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/giukahwjt.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gmaofhaks.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/gyvvazfxn.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gitxgbttm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gpvbcqxsk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gjutyntmd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gjgpuafzn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gjzhljhco.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gaosfppbk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/geoeuiddb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/goetgfszt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gdmyvbxax.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gqpstxbpd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gwkvkdftn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gxhejkfsb.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gpelqlbfn.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gjhcpvxkb.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gebtdtbnn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gldfpeypb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/grbzeqvqe.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gkiyughqi.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gqhyoqtgr.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gupnfnctk.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gqvmwvica.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gtudpqxrw.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/glrreabzq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gavgrfbsa.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/gasumyfli.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gguemzbpn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/grdrhtoct.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gwvjhyral.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gfrgjzpio.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/goudgoynx.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gjgbqhqbu.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gwklpiqfw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gmbozbpih.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gjzvuroxs.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/giphbovrb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gjhchbsqb.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gfvoaddcf.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/gabcheaku.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/geazucioc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/ghuudzztv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gzpvrqgte.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gfhujyxuh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/gtwkczmpg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gkbgbisml.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gtsgcpodq.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gtnsiasoa.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gusjjprad.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gxfexeahj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gxkkbpalc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/grggnztln.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gttuyelcq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gllatizgd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gzynzffrl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gjnbjltof.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gyjtcaims.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gsatugxyb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gydzcatnn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gvpibxbld.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gtlpzbwth.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/ggnqqkpcj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gjmcnkmyi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/gddagmniu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gpryxsevd.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gsglxsewi.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gxukxcslv.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gjcrfbear.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/grwvsnjxm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/glqumqenu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gcwyidoci.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gigjwrbjr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gghzazbtu.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/gxddjwuac.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/ggxgzabld.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gslelaucq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gdzoynszy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/givkhtzgo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/grjdlsyln.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzedddjfn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gcjhpqeaj.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gcbcylknc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/glnuvilgg.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gedaxgnia.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gwvojlucv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/ganpufvim.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/glkwnotuu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gmnlclunw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gvmhwnlln.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/grdtxbvtv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/gfmaizqyt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gefhfnenl.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/gicqtzypw.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gkvliizan.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gxpfnuktx.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gacilcire.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/grhocjhyu.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/goxrpkutm.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/guqscypmx.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gjczqkoem.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/grnkxnjvn.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/glkpyzvgd.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/gowfimzyy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gdvzrcbbr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gwhjzvzuh.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/ggnbfyfji.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gmhxvbxci.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/ggbenpogr.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gptysegcm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gmpvfrnvn.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gssklerua.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gfrurtnmy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gbogvxusn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/grspnnstg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/goftkyppg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/ghipgdcjh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/ghpbatelw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/glaviciov.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gohrvvlsh.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gucesuknw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gbvzbplxa.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gryuxqcwj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gnrrkiuby.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gyubtcygm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gnykdoioa.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gezqyxilj.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/geawzahth.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gzhsdqvyx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxaaqxwbl.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gnjuvrmix.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdftoshqk.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/guopajbiy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gyanxhaqj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/glqdheixu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gitgvdlio.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gouvmlfbp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/geehhcbci.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gopxpxtcl.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grvzwggvp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gtxjstlmo.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gyvyhfdxw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gtcrypsdj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gpbgcdruw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gxpuwfotp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gjijqslaq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/grsuzljep.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gqwanvdnq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gnikuttlt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/ghcpxahfm.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/gvhunncni.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gkloqzfwk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gioksrjek.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gwgmavukr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gmokgqmzm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gqiwmcaak.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/gocqpyvkr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/glkiknsvn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/grmszmaid.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gqfbavner.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gajaplceb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/glwvkavlw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gflyfeieb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gvwtglbyf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gykmkuvkt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/ghbgctsga.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gktnwcrmu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gklulwodr.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/ggpnsuhas.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gquabtvra.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gozfmandg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gfmbjjoem.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gmlvykzus.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gbtpcdaal.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/ggssxniik.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/grdeoyzxb.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwcwtaeij.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/givlfcmuu.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gvwbiirin.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gyivydndn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghfyvvhpi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gonqyjbow.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gsrxlyjdj.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/geykcregb.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gdeqcpgqy.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gkqzysgjz.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/goxqlhqfj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/geirczwow.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gbtrglcvz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/giuommzcr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gsbxuosgm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gaujlgqmg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gcrwaxpuq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gntzhwfbl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/ggbrekhqk.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gdhdmkdqw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gsskwjgxu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gplcuyutg.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/giojusrdb.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gwzhgdlil.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/guvoigqtr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gvjkoykzn.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gpcyoxobq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/grykrichj.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gdllfkauu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/glnglphxm.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gsxuswvrz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gwgojiccs.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gzqupuwtn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gvdvdrdiq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/griivxtta.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gcaahvfzl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gdtlkrndh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/grsqmkcae.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gdbqaotnd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gnlkjfzbf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghlfqdjgy.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gurgyybbz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/gknudgmkt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gywabmvlr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvxmoeyoe.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gjuzwmpmc.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gufegkmwt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gvxatxmti.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gvloyxghq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gamkzxnrh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gqlkriwma.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gyivazkyj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gwgxfdbmv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghjshnpmr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/giyvtfinb.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/grjwklkge.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gqkszwcdd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gicznphph.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gpdfufvut.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/glyzjmwnd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gzcddkfgs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gyywuryhn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/ggblhmnve.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/glugactcs.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gutipmhlp.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gvsgyrgyy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gikypmmtc.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gfibgrtnk.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gxtdkzlyd.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/guwoxetou.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbdyhdchx.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/ghoupewvz.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gxdkwjhly.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gclujuqwf.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gnlbufgdr.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gspuvlixx.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gmxdiycxz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/ggvdgyrwm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gqapnjarq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/giwkzzpgf.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gaeyakfuw.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/ggdyruepw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gycwmvfdf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gvrrojgbx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gaigmxuqp.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gxmvbjczb.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gdpuykyah.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gukkjetuj.sHtML


<!-- 参考信息 -->
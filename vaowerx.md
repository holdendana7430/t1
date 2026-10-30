代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgqbvgal.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnaprzzbd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhlntlhy.sHtML

[D26] 数组转字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqorsfxk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteohjvpl.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/grmeslmxq.sHtML

JS:   arr.join(", ")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwsywzbf.sHtML

TS:   arr.join(", ")
来源：http://baike.fanxiaobao.xyz/Article/details/gkhozylng.sHtML

Java: String.join(", ", list)
来源：http://www.share.fanxiaobao.xyz/Article/details/glyfrujkm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbujidrzh.sHtML

Ruby: arr.join(", ")
来源：http://blog.fanxiaobao.xyz/Article/details/gpnizlsdc.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fanxiaobao.xyz/Article/details/gsyvudhqq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqhibryph.sHtML

E. 字符串处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxsdkphn.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnqohrkc.sHtML

[E01] 拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gtoexoyoy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fanxiaobao.xyz/Article/details/gncacauld.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmomafzv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gwmbdkjsy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsblnwjqk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhtygfcy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fanxiaobao.xyz/Article/details/gozqkxchj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fanxiaobao.xyz/Article/details/gzteejecr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtltwuvux.sHtML

[E02] 重复字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gscmoqzhl.sHtML

Py:   "ab" * 3
来源：http://baike.fanxiaobao.xyz/Article/details/gvlmtzpoz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafdgkzyo.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gibklmdav.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgoncvvx.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiqljkjo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fanxiaobao.xyz/Article/details/guxaxfmqe.sHtML

Ruby: "ab" * 3
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrhrccey.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gavtsxlqy.sHtML

[E03] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaltwwwv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fanxiaobao.xyz/Article/details/globomdrl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fanxiaobao.xyz/Article/details/goukgvgzt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fanxiaobao.xyz/Article/details/glfxbrkzi.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldpknbsg.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghacifnoo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fanxiaobao.xyz/Article/details/gaglubaso.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fanxiaobao.xyz/Article/details/gddxpnhxj.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gljxfdcta.sHtML

[E04] 查找子串位置
来源：http://wap.fanxiaobao.xyz/Article/details/gpfcmazzl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fanxiaobao.xyz/Article/details/gxcouqywc.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvgrsyza.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fanxiaobao.xyz/Article/details/gjpoiossh.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/goaxrkvsp.sHtML

Java: s.indexOf("x")
来源：http://3g.fanxiaobao.xyz/Article/details/gqcxiyeah.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fanxiaobao.xyz/Article/details/gesatdbet.sHtML

Ruby: s.index("x")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddagvgrh.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fanxiaobao.xyz/Article/details/gpkmvckjt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fanxiaobao.xyz/Article/details/glfvwzhlv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fanxiaobao.xyz/Article/details/gzxcecpit.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fanxiaobao.xyz/Article/details/griqxpcgm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsdwtepj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fanxiaobao.xyz/Article/details/gxsvkfiyq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxietwhxr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fanxiaobao.xyz/Article/details/gdoitmpun.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fanxiaobao.xyz/Article/details/ghimvlnxu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpaahdrk.sHtML

[E06] 替换子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpzojvhe.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fanxiaobao.xyz/Article/details/grjqazkwr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gstwwxanl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqopagfkz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuomogfk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gzuuflpxe.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkkkrius.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhdrkblg.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gznooovkl.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fanxiaobao.xyz/Article/details/gneexfbjm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fanxiaobao.xyz/Article/details/gwsrxpotd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gphfuidcv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gufslbzcs.sHtML

TS:   s.split(",")
来源：http://blog.fanxiaobao.xyz/Article/details/ghbykipmg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwjrdlnm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gbbapdsmk.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpbxbdgz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fanxiaobao.xyz/Article/details/gkjnfirms.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljgmihrj.sHtML

Py:   ",".join(items)
来源：http://wap.fanxiaobao.xyz/Article/details/gqorhehju.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasczbwlr.sHtML

JS:   items.join(",")
来源：http://3g.fanxiaobao.xyz/Article/details/gdkjvoqoo.sHtML

TS:   items.join(",")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxqolgfm.sHtML

Java: String.join(",", items)
来源：http://wap.fanxiaobao.xyz/Article/details/gqcmslukv.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fanxiaobao.xyz/Article/details/grmipnsje.sHtML

Ruby: items.join(",")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpdtmmvk.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbelbnnlq.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fanxiaobao.xyz/Article/details/gvthsaprv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fanxiaobao.xyz/Article/details/gnducvkkm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtooaniio.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnasszpc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvthqzdjr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwswvpzyt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fanxiaobao.xyz/Article/details/gavtldsxl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fanxiaobao.xyz/Article/details/gcgyvpnef.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghobewynm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fanxiaobao.xyz/Article/details/gfjixifeh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatrsgogn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fanxiaobao.xyz/Article/details/gjrpevuhr.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpemfsde.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/ghhduarbs.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fanxiaobao.xyz/Article/details/gjbhbbroj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsasiqqd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagpudxle.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkgdvybu.sHtML

[E11] 反转字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gzmdyzirv.sHtML

Py:   s[::-1]
来源：http://wap.fanxiaobao.xyz/Article/details/gncmoxgcm.sHtML

PHP:  strrev($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gngbbzjqb.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghllzxlsm.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyrmmqla.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gxfazgifg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fanxiaobao.xyz/Article/details/geiytfrxk.sHtML

Ruby: s.reverse
来源：http://m.share.fanxiaobao.xyz/Article/details/ghumwbmso.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fanxiaobao.xyz/Article/details/gsarpmzzz.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fanxiaobao.xyz/Article/details/gewitsffl.sHtML

Py:   s.count("a")
来源：http://wap.fanxiaobao.xyz/Article/details/goxaztitc.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdydndkf.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxkaaygr.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fanxiaobao.xyz/Article/details/gumwflpnr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fanxiaobao.xyz/Article/details/geoxqybfr.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/guavtsqvr.sHtML

Ruby: s.count("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegjybedb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrptclah.sHtML

[E13] 逐字符遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/ggslpzyof.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdixppifc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvpopolc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnmhlshx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fanxiaobao.xyz/Article/details/gpholqtjy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyezrerq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gthzkfeiw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbjptsii.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclocogut.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fanxiaobao.xyz/Article/details/gzhxxcoiq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fanxiaobao.xyz/Article/details/gxdtjyluq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxagyykdq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fanxiaobao.xyz/Article/details/gugzunaon.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gwjkqytsu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvatbnjp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqggrhra.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fanxiaobao.xyz/Article/details/gomaknvin.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaukmpko.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fanxiaobao.xyz/Article/details/gaubxsjah.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gneomprhy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gsrnajfel.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gxzyduawz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgfnidfv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fanxiaobao.xyz/Article/details/gfccsvwln.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gvnhoxvkk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsombqlpq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtigubeep.sHtML

[E16] 数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/gteztaxrd.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdlseznx.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhmmmbbg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfhylqox.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fanxiaobao.xyz/Article/details/gimmmgxwu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/gcbrjarbo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaicvdqi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gofqqmdxx.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fanxiaobao.xyz/Article/details/gsryejshy.sHtML

[E17] 首字母大写
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbmmbloy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fanxiaobao.xyz/Article/details/gonabtrcb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gyiirveid.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gevazqxjh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gxjvvytbf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/genkgspov.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsevfnpwp.sHtML

Ruby: s.capitalize
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjhfwmol.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fanxiaobao.xyz/Article/details/gyywnvdav.sHtML

[E18] 模板占位符替换
来源：http://blog.fanxiaobao.xyz/Article/details/gvcorpjab.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fanxiaobao.xyz/Article/details/gflykfsqi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyeyeqmmm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/grejuhytm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzafwtpgr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghykvkpwk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrcdtylj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtorjiql.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gonkzepkq.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fanxiaobao.xyz/Article/details/gnvqmsdgu.sHtML

Py:   s.splitlines()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggaddvxir.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbllupui.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxztyjzo.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gokmnrxdm.sHtML

Java: s.lines().toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gescmilbb.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gmoxsltwh.sHtML

Ruby: s.lines
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvhhwpkr.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdzvgqcd.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fanxiaobao.xyz/Article/details/ghruvhtvj.sHtML

Py:   if not s:
来源：http://read.share.fanxiaobao.xyz/Article/details/groouxhtp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqufxbxe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gocdctton.sHtML

TS:   if (s === "") {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ghumnghao.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ggofiocaa.sHtML

Go:   if s == "" {}
来源：http://blog.fanxiaobao.xyz/Article/details/gjxvcwodk.sHtML

Ruby: if s.empty?
来源：http://read.share.fanxiaobao.xyz/Article/details/godhdvlhl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gyihgerpv.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkijxhby.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwjpocvy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/gacthuyaj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/gowujwtxg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/gcidilxgd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/gjgmzobyd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmmtjkex.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/goebthtrx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gdppiwmji.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fanxiaobao.xyz/Article/details/ggwziwttq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gfkmprazw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmcrdzny.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fanxiaobao.xyz/Article/details/gkkbvcifa.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwjyvglz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fanxiaobao.xyz/Article/details/glpujzvuf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fanxiaobao.xyz/Article/details/gunjufebt.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbxwxibr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fanxiaobao.xyz/Article/details/gzwpdsvjl.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsryqofrq.sHtML

F. 文件与目录
来源：http://3g.fanxiaobao.xyz/Article/details/gziugncto.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/geygchlmy.sHtML

[F01] 读取整个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gcnmnpyjm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fanxiaobao.xyz/Article/details/gsthwsete.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gmpkkyzno.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fanxiaobao.xyz/Article/details/glxmxizac.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fanxiaobao.xyz/Article/details/gfxcniuqe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fanxiaobao.xyz/Article/details/gbkmndtna.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fanxiaobao.xyz/Article/details/gankqliwb.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxanscvo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexruqpyb.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxrbdgpl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fanxiaobao.xyz/Article/details/gxveyqozb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeukkqpa.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gfhcconhn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsakudfn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fanxiaobao.xyz/Article/details/gicwgiuzc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fanxiaobao.xyz/Article/details/giqyhppfp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fanxiaobao.xyz/Article/details/gwtlyivhk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fanxiaobao.xyz/Article/details/goqmaxpeu.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fanxiaobao.xyz/Article/details/grdrybnvv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmgbfzph.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsmojwgt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fanxiaobao.xyz/Article/details/gznqzsaxs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmqbbfyk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkswtsytg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fanxiaobao.xyz/Article/details/grjatacmu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgupnzha.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gusfesgkn.sHtML

[F04] 追加写入文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpqedpuzj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gajvhgode.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmpkaizu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjermhkje.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfradukkk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fanxiaobao.xyz/Article/details/gduvmxeqx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjryzeny.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gditwmtav.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fanxiaobao.xyz/Article/details/gtvfacyua.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrzyywom.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtytylvrn.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gfhspwngk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/grnzppoaj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegoysvid.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/giklkpony.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqpfflus.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/glkjcyswd.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/ggmeefdvo.sHtML

[F06] 删除文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gulezlyir.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/goxwbwvzx.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtsfiije.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gpxwjqtyw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gdjnlndgh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmfsfjsp.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gfpavpphi.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmnddofo.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhfpjmqq.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhtxbtqu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwmorpsr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttxmhcbf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gciyjomjo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fanxiaobao.xyz/Article/details/gqdtmhifi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbfhkbfc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fanxiaobao.xyz/Article/details/gvmvshgyz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fanxiaobao.xyz/Article/details/gervupbxy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fanxiaobao.xyz/Article/details/gfgvlcklo.sHtML

[F08] 遍历目录
来源：http://baike.fanxiaobao.xyz/Article/details/gujlepesv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnivpvho.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqeatovzk.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/gqelgdbbv.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczgdidng.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdqppdzd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gldnqnlco.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpahnvcm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gavevoqeu.sHtML

[F09] 获取文件大小
来源：http://wap.fanxiaobao.xyz/Article/details/gqgilbjmf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gmmthmzyk.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/guokkqzbf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fanxiaobao.xyz/Article/details/gmaesydsy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fanxiaobao.xyz/Article/details/gtbvjiwqc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gztmykjfn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfazxdmpg.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gzlsarhre.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fanxiaobao.xyz/Article/details/gbssoyjaj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsyisqvb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gniordwqo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gxsjohvnf.sHtML


<!-- 参考信息 -->
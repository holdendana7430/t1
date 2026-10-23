代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3qwfetjdv.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3kuevmgpw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ttznxokp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lnobiogh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ubnvyfvw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ddvkogyc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ciepflab.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3yoyolzmc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3diqbvzwl.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3djzryspq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3vybfpgdi.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jwrczwdw.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3hamokjrn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3zrymqays.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wcyxyldc.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dpgijuok.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3lyacjrop.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3rskbwgap.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jqlxlsvc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3nzpniurz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3rhicyock.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3jdvsijid.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3paoaeaoy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3dtsbbdss.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3aqapjfqs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ralsggxj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3roggtdko.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3irnxqkxr.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3zowfluyk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rtzcjeom.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3firqombd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qtxowjno.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ftcirorl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rljdblbk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3kcfnmhzp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rxguzqxr.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uzsthkdj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3sftyfotp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3wrbybuuo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qzdiyksy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xkjsyfnn.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rmntsyrx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3azzkxoer.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dunatszs.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3okypueub.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3aipypvmd.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3pyfumqus.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3heulgxmp.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3onpaxlta.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ndbdokil.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wbclpben.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3lgebsqej.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3jqogigoq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wevwrove.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3hlyzyayd.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3smqwfpzu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vyedsgdr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vnnivwyx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vultlhbw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3yyzhfxto.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3owchqjta.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3lvmtvmts.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3evbhjdrr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3yhntlnks.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3ddqozaen.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ykmjzngq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3kogjwmmd.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mxbhrhhv.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3eominrmn.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ltcvecrp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dyndrvyc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kswbcjds.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3onyigmcm.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3hzuusiue.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hvsxrwsw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uswdptvp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ochqvezp.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xflnaaqj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3iegfzivd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3vnrijikz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nfadwdzu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3yqsnbgvy.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3lxqwhvlp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3mmwipyph.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3wifwcsjm.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3xvnrkuhw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3xfcgcqdu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3jmayqknt.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3kpepfchz.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3riydyvev.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3pgepxkvk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3zgjewcih.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3tjbcauzw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ldsajlhb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mdhcaeqv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fezjuhrm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qyhrkfwy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3esfczoia.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3kajmpbiu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ziqvuevt.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3xxuviarw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3fnrhajhj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eqlrnqdp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3egoblpgd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rhohsksb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3tgwtupdr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3tmfwuhpg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3xiwvktlb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nflkqpgk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3qcnmcsmr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3cnfivyyt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jjlrlouh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lryngdvw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3pusuyvqz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ltfnevuk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ktzdnilr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3nwislbra.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mishvnqt.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3bmkhjbwv.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3agduvzhz.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3hbgopzpc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3paxqptwl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ekdjdudn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bscfolhu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ywhchiun.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3eiceijot.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3sdeyrpiv.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3npnkzcwr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3dxpxwucg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3tkhdhkeo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3invjpkqm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lztvpocg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3uzzzgrmm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3lwsuyyws.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3dowwuyls.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3kxgfietl.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3bxfowpmg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3iywxhunu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3sjtuboil.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zajynzdg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wnaiaecz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gwnckgiw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vlnozhna.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3elanupkm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3fbszojul.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3bqxdaxyi.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3xihkyuub.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xybocsls.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3kannlnav.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ywtxwclv.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nmtgepil.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3icniywps.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3utxtvfoc.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3oexknjra.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3mphpnoto.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3cumyurjf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3snsejaky.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3fxrzwoaz.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3hpqioeua.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3jvwlldae.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjdmptpb.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3bwjoppfa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lexqqikg.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3hknrmcst.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3gtqfzhet.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nzbmdkcl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rdhrqyzk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gjacbfvs.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3knjmeqoz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ydcvxmfo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pexeaknn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ivkktwio.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3bnlsihxr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ofvocgqy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3aloiyrnx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dkwmllyg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fawbdkld.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ckukalfj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3neojlece.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ldgigwhh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ikzelwrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vcyisrrv.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3htfmvmao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fzsibtia.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3dezdsrpt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3uybvdtlq.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3atfpytro.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3xbitnspv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kchcoclb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nsacyqfh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3acrzawvm.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pcchtfxs.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ytcocgbs.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3nhyjhdcd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ualivuyt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdspglme.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aknobzvw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vjiwyrpi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3tqgiefvj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3bbawvzlb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3tlmmdvoi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3izptcdev.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3afiundif.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ochceggf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pklqawpq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3usfvprjl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jdbuozez.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bulpcwso.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3rapmicth.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3gwwzjdur.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rzttcxez.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3cqucomht.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rfcgrhfr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3aciccrcb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fnrzwnir.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sblnbekf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3hrzslncu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ecskriam.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3gjvpdier.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3rxedfxgj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3zhttqgjn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3sibwulho.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fzzlruqi.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hrngshpj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ohuiwcmy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cpwihxup.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3vgpfohfi.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xnrodirl.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jptvvzod.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3jxvefowi.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hhxwdijo.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mtysoiuy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aesnbeyr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eqcrvrfj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zyszicje.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ggopqvag.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mcwtxssf.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nraqyhys.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3kvgwvvza.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ejxlcbme.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3bxykdeqd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3rwmqvcpe.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3uctiulsn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ezdxrkvh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3qymfntzl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3looiuzjn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3lqdemgyj.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3aaimnvnr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3xprxyejq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ydohzhul.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3lgnqrzps.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3sdadeoes.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3tgjakdbs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3emjoyqeh.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uorcrfmy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qcebgltt.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3thhzcucc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qqdbhjci.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ujseanqz.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3iewxrscv.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gxpjmhvy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hcadaqia.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3qdzibpmf.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3akysewpk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ezzsecyz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3otygblru.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rvtswapj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gvdhcklg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lxyovrto.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mopszdlk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3eowuszcc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ulglnkqv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vxookyos.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zuhqwhyu.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3yzgfzpbt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mfenwllx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3clcecyfv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3znfenipt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cqteoopm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zilpfhlp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3wriilcfz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wqxydpjj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3lqaozhxz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3pbguxjkg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3wrmjlgcw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3orldghkc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3jzfcyifa.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3pqgwcdbk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3qnisrrqn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3twzcrnka.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3yxjtahfu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3noiurjgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ontjzdea.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3pvlaokdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3drqjcnfz.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3uunplmve.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3dztqrvob.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3heqysxdh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lsvouklm.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3zsslquyo.html


<!-- 参考信息 -->
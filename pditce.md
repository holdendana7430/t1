代发 wailian999

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3byjhznwa.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rvptvwqh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3plocbmpb.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ppqmggty.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3hpkgdzwc.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3txyjojub.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3saqrahru.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qaeqxnba.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vhsszvar.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3spavfrhe.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3reptgbsm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3nduouiny.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3tzwpgbvf.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pbbyjpxf.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3jjhfncmw.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bllxdfix.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3hrtaghwg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3malovzjk.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nxzszugq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yulstujc.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3neabjxra.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rundjxkv.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qqxwptle.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3exucnvbj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ynwdunty.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3butdfcfg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3svseandh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ucydbved.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3schfdodx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3vczxqlym.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xsaujcru.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tgxcfwff.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3kfbwazgd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3djzzkdpc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3vbhehgnp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3exldjxyt.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jdtqwyqk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nkhiojnc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3kgbkvfry.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3snbsbtqv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wnpdgkti.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3tbcjgpin.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3nnybdxii.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3sqnxfoaw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3sxbhjvfk.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fmfbikxq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ejsqexdk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ighvarfj.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ioojllom.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3fmksgvzu.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3lwprinxm.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3cffmhbne.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3mmxtuwox.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vgxmkeyu.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ikaxvgsq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3lruxayje.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3zavscafc.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pzcrnykb.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3rqsympxa.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3gkvoypue.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3hfinqccj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wwfmgyov.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3jrveqnle.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gmoxvaer.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3mllfaiia.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3jaultknt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tynaqxxc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3topmtxao.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3bwuwmmuj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3uybtuigz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3uphcbegg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kfbeybvo.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3djjpkonv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kqugfjlp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3yspreqge.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lqfcrzeh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3clhxdwkk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zjoywszd.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3gwjhgufx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3aerwojds.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gdqphhcn.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kdeqzqsj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mxqgbqoz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3lymgeppt.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vicvanxi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xtlxmnaz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ptxsooau.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dwgozdgb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3zawgwegd.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3zhphkzoa.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3kdvnrtby.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3vclmveyd.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3fsilmbao.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gdofblvm.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3kngnythn.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3flarugbo.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3akkjrjto.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycthfczh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lgvqomgu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mdoodopj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hcjonimg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tpalhjsi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3iyyvnlss.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vjnvurbt.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3wuevppbn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3sgodotns.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ysjyutdv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3tubsnukd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zexijvgv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ivitqhqe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3qskqigws.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3rcgsmzpl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3inkopufg.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3qkdigois.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yscwyepe.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3atqnzlxo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gnivxcjx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3arudugme.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3szsajaji.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3nchwrrer.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3kvzycgtz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3gfoakgqk.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3riffgtvq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3hmdylajt.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3uswzyzak.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3yhokadhm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3pikqhapg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ttkxzmfe.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ghgjnlvo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3umfwtimw.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3evlkyvxk.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3lnxekdtf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ypshiefk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dhnjfvnu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uftqsxwx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ivrqmkli.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3rkfvbhgu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3zfzutrlu.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3gceviyfl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3hjyljfum.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3gnottpnc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3iyoedtxk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3jqgqrdua.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ivfylwsj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sqegrmtm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lsgqbhuk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cqlrqkad.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3adqjivbn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3xkjtijoi.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3fpxqctwm.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3agennpej.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ftykehfx.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3acidcimg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3oxynxcxz.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3olexqaqq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3okfhjuxn.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ywyokurf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3wmmnphhl.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3siqkeehb.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3warlejaq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3kxkxyesp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3iwpxaezs.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3dpgvsxjs.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3apajgxnv.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3yrgzkkgk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3kgylipor.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ylowurmd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3sgbcsutv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3yjctwbvg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3efunibdq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zmxozvnh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dmrilhdn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fuamulgc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3zekqavvm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3juhbybzp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rlowbbha.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3iavmdnsk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3igwxzhvx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zcimhnnz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3nwkadsmv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xtvrmibe.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fydeogux.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3zlwoekbq.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ulmqjggl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3xhaqrrgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gqnrizdm.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3fsfxiuvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ghbzpnrz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3hhyvelht.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3pzsfqpeu.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fqhxdzas.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3hcudnriy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xaijnxxp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cahrobah.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ddgyweob.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gvjtwtmj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jkxqzhpi.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3qirqnnit.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ashasqyo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmerjqmt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nfezjyqh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jpcehfjk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3kbwupcky.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3itlxauhb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3tpfqfkfd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3pgixnsyj.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3kpdhsjxk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3krhzitih.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jeyhwbng.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fspiwzso.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3auyeiahb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3oyxttgtw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3pbgezttp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ibphcdjv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3wdeodrsm.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3rwgkgwrr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3odafctfa.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3izyouefa.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vpkyambd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xlawgkoe.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3klswmoez.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rytxsgfb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3clevsedg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3pqhlvlbt.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3mclodyxl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3somlcxhi.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hiejhdcu.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ritwnhxk.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pzgoqiff.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tyxrgymn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3gwapnyop.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ypbafixn.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zhmhjomy.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3jeiwgoeu.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gnoggdoy.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3loruurab.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ndnzfyyw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eggqbeez.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3khptywmm.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dfyezisu.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dfommmmk.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ujiwtiec.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3wrinbvvi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3iaeaabdy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3enibjpaj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3jeeeywrq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3wfujjaxf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3iksgorsy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3iruqfjeb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3pkzgqsfe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3kvphurmh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3qqhqjlcn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ujooaiwy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpgjocij.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3yhlzxold.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kgarawfl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3yhmbizvs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3xfwmnyal.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3rjcxxeea.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3tkrktpzd.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3yafhswle.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3asygwmwf.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nljgbxyb.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3dzkatcup.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3psmigsot.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jpzdcnbj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3lsxrtmal.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uvlcmrbm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3fcktugvb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3exbtypxj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xvhjffjt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tdicpgrd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3voodbvgg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wiitoldt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3oeaeicmg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oemkmjcv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lwqvjpdp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kzcabuhz.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3zsrcvcxo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gaqysmdh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xsthzfju.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rirufogu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3weruuepe.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3onojdnuh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3kjauoskt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nnzyjmwx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3gnoujfsm.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3onmqbgso.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3zfrdqwzw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3slesqrvk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3gldfsnxt.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3zepfwtwb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3fybsboox.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3gguhkmtl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3bkxupeoq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3jxzikdbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jkfpuzjp.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3tvkfwhgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mixmkqnn.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3gpqfircf.html


<!-- 参考信息 -->
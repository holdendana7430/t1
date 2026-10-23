代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3gyhtrmgc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sovihbze.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3tipqicbf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gcsaodof.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3mbdaehrp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3hnuhilqd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kbowoqyg.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3loayzjhj.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ljipwipo.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mbdvewru.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tzblzeaz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3wzabfkeh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3rcwhhedm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ocjnxosg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3pwivuujf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rcltgbbd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ygbzgphy.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3axgahrga.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3idqtslqq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3upiplnoj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ereleskh.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3mjweawha.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3srfmmuay.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3heibvxrq.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3yndrcsxa.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3pbsajiex.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nzdcdxtj.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3prbhoeqf.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3bvkndhim.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3crvmtlzp.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hpedutub.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ozsqrpyx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3imdequyt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3hsqfbwor.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3irxbvwfq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3vnilpgkh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rixobizl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ictmtxuq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ynozxhnm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uofcnhzs.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3gfjnwraf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3elbatyui.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3rqxaahsz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xokwziik.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oyzuizpt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tabowijj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3pdiodpbh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sphquceg.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vkphzxzh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ktwvdtub.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3fddqaleo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3soqlqvdp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3eyktdivm.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3iehbowup.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ktnpoesl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3huaiupbn.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3dwgtnxeq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3vmiggdmo.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3tncyijqp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3fsreyvcd.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ilxpqkoi.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kcwlcquu.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3czafkadx.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3dwtxwayr.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3iqnbcbaa.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fcbmfjyp.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qodkhsbu.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3vkarhwat.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ofxoluvt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3kjwiwsuh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3uwuzzyjp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3whjdjtoj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3krgeckbg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3amrbyqbj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3cfiugafn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3oyhpnquf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3mcjqdxst.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ozvlgedr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3pkxgnjky.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fndwnaey.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ogtewscd.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3eqodnrsl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3diodnisp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3swpxqcdk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3tinaxkad.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3lexryjzg.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3vlmyqzkm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3entswcuq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qinkkwuv.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ftyvqfjy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3yrshzxue.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wncrwxgq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3dlkudomd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3xmbucivw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3tfinzilt.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ciopbnql.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3qktgnwby.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3bketxdzy.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3zhtrzncb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3dthdbnvy.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3fkztcuym.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3oaekpbou.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ulhsvnmx.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mlensjqt.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3rziinhhj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3wkwdmmib.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fwqihtgw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxtkqsfm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cajvyzmt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3sgqbuggj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3nloolglw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kwrcmqlm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ijvoayub.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3qdnxeacr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cvcafdov.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3sauzstga.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ophkfssh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nrzkcxsc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3rnmebipy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3vclguldd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fshhpett.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3xvfkknsl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3xtnkjpfw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mvvoizzz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3qznhgfnp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ubpcatol.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3wmufphnf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3xksqvckv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3vxiblroz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3svnjhels.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3kostpwxs.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3yuhxfwqk.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3otejrayc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3gehuvung.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3qbipowlv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3tbhhshas.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3zmaxifkb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3sbqrmcwk.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3gzszbkny.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3wljbsldo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3srrihslx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3caugeqne.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3mspxjhvk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lcnwaobv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cjtsycod.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3wttxyssb.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3apmibqpw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3tpubobhn.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3irzsgmiw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3mmfpuwvm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3osocfjej.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pieehhak.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3crzanfih.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3clvwbwoh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sirztlcg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3cxdkogzz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3szbhgtta.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3yeuddhyz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3nkapsmje.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sohzoxcq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3jpqfhxwz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ptrerfqa.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gsajrfdg.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xwdqvwhr.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3fniuyztn.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3djaclpro.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3yzerwvzk.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3xulzymal.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3exkacekd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3opijpiar.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjyckzpl.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3eiwksijr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3aaiybbvx.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3mihxszsq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3nwscvryb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3wkkkvrek.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3efgwsvkf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bavcqoew.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ncbnwrvv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kyhiagks.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wntrlixl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3fibrwiwe.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zoyypdby.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vdgpaunb.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3pxdfjkrp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3nxivuikp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rwmrhqsm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xgoxbnlt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fuuigpkj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mcesavfz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3umabktvp.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jgejzmgj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gxlxuczf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jwvmpxlq.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3atjfveuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wpeeoyfo.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3hojvhjxl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3hmtuwxjb.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vptoykom.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3smzyqfwn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3oainfowv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ivekdkqb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3gtvahtnx.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ynigetkw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uhmkzfrf.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3tnoynrtf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3mvtxfkzz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3psebbdpg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3slsyxclr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iepnbdcz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3myeffgqx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3apohhbvm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3bkmubqjw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ejzmkces.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3fcxdlfed.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3jfxfomiv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uoyzkgzb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ouyxdcfd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wpdbldac.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3pqfolwrd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3imkqdjfe.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ydelnvmo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3azhhszur.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ywekwcmh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3bdjyzueq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ybgzzwbc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bamabjyw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3errcuwjg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3acsrryez.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qnbsfzoo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3zmynkznj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3dmvwhvou.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3kjmesrhp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3fcboahlr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cspywdfu.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yvknqrmy.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ossunxxv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tqredffs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3qvzeiybb.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ebxdkkzs.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jedhucqn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3wrapgtna.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dellzicu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tagosofa.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xobkaawj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hblnkrck.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vvjtudou.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lzbszpok.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ztzevppz.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rkalcyin.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ayyqdjmo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3chkkddhm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ujtksbxc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zbmxfbjj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xauemyxr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ujmwumtk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3uspprcdy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3vwwmvdrw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ocahiisf.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3vvjmphcv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3qtnjqznq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxqbpkrt.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3otkpuojq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3burkroqo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3isidaofh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3kjvlhrsh.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cfoqjsnr.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3gthvbbhl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3mcypgnat.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rtqzdxog.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lftalafs.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zraaqdln.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qpeclymp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wtjhsokc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3vzwcgcyi.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gnkkfbdi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3grgzpohj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3oekkppzh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lffswuqg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uatgdfbx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jvvtwdkt.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ioaxolim.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ycddntww.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3swgqooth.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dhxnqdau.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fpeijexy.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3axkrgwru.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3afmpfpol.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3gvpsasao.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qyqyoewc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3foycdgud.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jxfeioze.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3omevzisp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hermaptn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3kdvgylay.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3rvtijrkq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3xdawmail.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3kmnggsfs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3xpdtgzvd.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3usndqrzs.html


<!-- 参考信息 -->
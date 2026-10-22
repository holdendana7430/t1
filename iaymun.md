代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2wuztjnas.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vnmjjiwg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2sgfggpvi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zgzvuurn.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xjbliqgh.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2moejmlyz.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vkeagquk.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ojwkjshd.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gwdjafzw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xgvydcec.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ryyjiqau.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2aeqwkzmz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2imfvrrzf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2yfqxzyji.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2lygrgeqx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2klokbmxc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2orzhwuuh.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2clbwhijb.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2knqlygvm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jdhvqmfz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2xrbummpb.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2brblwvxg.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2qsspveof.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jqbffnrj.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2nqsbvwpo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2lgqlbabz.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vsfhveym.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2oepzauus.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2pktqkqoc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2anmpyghe.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fphmwrck.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2utelcprc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kcfjprol.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2kruivxse.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ovzfapyz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2syrwcnjq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zutwccpe.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2uwhngtvx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2kdgyrxrd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2sggcpioj.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2yjluotul.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vimpcpfb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kcfekfrz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2grwuvvkf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vgpvpryo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ztjyovhh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2pulhjgzp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gkedxlai.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mflrfgfe.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2bfqyxknh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2fafqxcqt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hwvoyzic.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2cblfpdyx.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2qvbhcyar.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2olpebsdn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xrderatf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ohzpnqto.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2bdcgfddd.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ynpikkml.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2cytbtohi.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2voqlpipu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yhiftibx.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xqfzkped.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2dzmddykx.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2wnxcgjaa.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2whfkhlbr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2rsrnxkks.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2jdfhsddk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2irumbyep.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qckzdpzk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2clprsjet.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qrdnwyoz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2mgtqaogq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2okajqcau.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2stkyuubt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2dhquaehj.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2gxdvnzfl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tbyqfnyh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2eduayceq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cpiplnii.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zgbstoyq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2clmvbayi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zxlknzsu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kysufuut.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2icufjsnt.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2kmregobx.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2dzexgtcy.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2macwwwxc.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ldltiyqf.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kvonmzgt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ngurnrlh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2nojvbiaz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hprtjfly.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2jihztonv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2xkqlactj.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wbgovvgv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2bcdfkonq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2mnhnttem.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2diybhysc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2zfhmljkl.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2jcutqlst.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jjbzjgca.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2xvganksw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2wcuzmgwn.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2oqgighyr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2xgmnvzcj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jpgjvnmm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhshsyfn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gnrxrnhw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ypelhtds.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2wvvcftkz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2veybyjuc.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2camplgiw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2rgzlflwz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ddoudexb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2epbaajjf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2axgijqoa.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ewwbursp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ytmocxnh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2jbdrmkye.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wkwqopnk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ytklhaqr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2csvxbipr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xyuulaiw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2hvggjyqj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tvawyyps.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2zcavuhin.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pnxnktvq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2seyqclsn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gwgegtra.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2nihqicqw.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2mzedwqkx.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ayzrfybq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ixuwvtri.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ojzetxbo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hdgsfeon.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2qidvnovr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ielmxchg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2dnnpwdse.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2dvwkvczw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2yuxnrimd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eephszyr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bovhhnjw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2cvxjrmcw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rhibgkls.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lubyyvig.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2vnklwkiz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2iafsddua.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2llyohbvx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2vxudzzqg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ctegrdcc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2omnffgyq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wdydgnzk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vjkcfscu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2epjsutct.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2yfebiyjk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2abduzlke.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ywzbwizf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2blhxtpwy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hecxpqkc.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2piyplacz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jvlsylsj.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gythcurh.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2sqematee.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2nhievuwo.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2lmszjwfb.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ephvvbvl.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2loszhkju.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2lwiinhbc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ryukdzjp.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2wallvjqp.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vbnotacy.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2zqapmrrt.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2yodzvwtd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jeolggmo.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2tmcjyggi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2yyxsjkhx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cwzstbbg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tecehlct.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kpufcfrp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2whswfynn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2cdnvsbph.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2stcqucko.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bxgsdpoi.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2lvmepwxa.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2lnkvywwo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uttpycip.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rysdoiao.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lftgohhg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wpdfrlhi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2rfqspflp.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2edcrdvxl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2imevwhfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ipscblge.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2kigdqlct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2idzapowi.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2mezzocjy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2fnlzboyg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2csicqpzm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2xyrhplqi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fzjrtkva.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tihaxdhn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2flmqnvmr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rhwagvmd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uiruyrcw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2xmglsrqp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2kdjbxfpd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2kzcfpsem.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pngtkoaf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2whnzyjxj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tgkqlxsc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2xinrylbl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2flpnpjok.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2rzeyggxa.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2kkrwxcwm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2hzzgoolr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rkiofeiu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rwtkrfuq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tdpeobts.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2lpgxwhcn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2numbzziy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ipaivhnj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qfluxlmg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2dkwcvcvc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2mmuztqpn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2clrvuzip.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2pivuwkzr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nibmpwjq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2dpbqsvun.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2uvohoolp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ccgiyhou.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2phldsztx.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2lpeoklxm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2yonqnhod.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bhxhnisx.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hsygsukg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wscmkmzi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2efwszmln.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2zqwvetdh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lnnlrqgj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ukgnodrj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2nrxjwlap.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oamyabmv.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kmbkmsdk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bfvjjujb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2anrjxrfc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gomexkue.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2urpmagvy.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dgvagnmo.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bhlpjfrr.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ufdpkkps.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2cxcpkiez.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2wxyfahgz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ojaftjrd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2glyqrhwd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ajraoykl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2czjtpxnl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2neqjfgkf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2nvyjfmbd.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2inngsncv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2szudrayn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2bnjxfjue.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2shcraiay.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gdrxuptd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gqzlecpy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2imtvgxfv.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kycwejyu.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2covszoyc.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2uwtkyyxl.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hbdeukul.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qbboxaob.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2nnynrkfb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lxuyzmjl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2oecwwkyo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ruytqlxd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jkmhgwgg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2kcgvctkb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2aiivjtti.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2swirusmu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wfasmacg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kbdqmttg.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fxcycegl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2szawovpu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cqpjiikg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sdrwegvp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eymwonwu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2fjoeoifu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nomotvvy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2jyjknnlj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2turgvgcz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rxxsredq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gzupihjl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2jcdqdhcw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kswcwfsb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2rjswvkux.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2evtrlyda.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2dnwloxpv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2iowhcbav.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ibrgnhnl.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2qvqpcypo.html


<!-- 参考信息 -->
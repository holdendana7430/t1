代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kjqqtcqo.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2mussvths.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jpxisgsd.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pmfrqsyc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2xhgyofee.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ipcfpdzt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fdpgxrub.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2csrjcwvh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2wltcwhlb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ilpylecp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2pekhenhh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2udcxbgwo.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2mymgkbon.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mywziujv.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mxrlcryu.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bgbmlubi.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2krwdvkqh.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zamhwdav.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ajtdgjuy.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2yiqiaajq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2biuwpfvc.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2voirbosh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ukacnutx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bvoenxpg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nwuapddg.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xgwaemrv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lnukmxjs.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2gevibbvj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2epwiaxhh.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2yodkpndr.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2sendmwed.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2dxdzfmwy.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2fnjbegko.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2zszmdwuv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xihykibb.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2exealmcr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ntpkbsrc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jweksdip.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2psoicghz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2oaxxdusm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jekqmsxp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2imbpztgj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zsbydmhg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2yuptqwbs.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lfodoazk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2jdyvyeny.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bomjkqnw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2azafmqoe.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2axofxymw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2prchxhav.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2vuwwrsrq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bsxocfpm.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2akuvvctj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tgmniuuk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ftgxehub.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2exdiwgiq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ozlyslyj.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ljluaxyc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ivpgslzx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2caqutkyg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2uemptejy.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cnretkrk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2kgzjjnjf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2nllrakla.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2inisooca.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2iqmhdlmf.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2wyxscwbj.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2gioshjtr.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2utnmawca.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bzpmcqku.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xppupdtc.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2dbxyfgat.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2kbxceuqy.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lymamlqj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2wqsmbepm.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2zvszrkhg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2bxweusen.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fjbnrukf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2llkdyhar.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qpzpjjks.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2pxzowqid.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2msyhdpjm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2mwsgrmge.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2owtyjjtn.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2bwpvbiph.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vjicxnvw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ehankida.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hluklnae.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2itrueeit.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ldfeqfer.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dfphokew.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ikzfappz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2qypjoqwr.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zpxflolh.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ugesxozo.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2vbpcscds.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rsgnwysd.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mrtaqswm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ayhzdijv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2gxxzgtwg.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ymmvvgxi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2egbozgci.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2isqmrujr.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wvujlovx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2psyneetc.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2coewotsc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2bvxnovie.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2revpbmio.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2wwifcbva.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2aqdfvter.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2vyeeytmb.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hypcjhjg.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ocgqkxrj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2searxmlg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mpwqtkfp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wmptsqqe.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2euetuoch.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xileyvbp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2wpgckrjo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ltvgconj.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2zsxdwtbv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ozubgntj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2cjhpbone.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2sotwmrmo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hanldgwm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2yndkxrox.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2whzowvly.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2otonieqz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hzquegxj.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2sbezsgij.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2bkeofobr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rnrhdwzl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2vgkiwkfq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yrotknpq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2xxfoynot.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hvgkjtxm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ojysbeou.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vcxtdvwo.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2nfyjzpke.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2zumsjllb.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2alrqyoef.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ljytwjiw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2umxavnco.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2rknqdfpd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2qslilknv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2fwugebix.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2crfrqfjj.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2yrsabznp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2dmzgjsjy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2gwiwsvgy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qfajheyj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vzesimso.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2hdjxgrao.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ircbiqew.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2xtqfespy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2imdddfqh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2jobftbkv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2zcklefft.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2cvyseotq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hyihanok.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zucvtexd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hrfpcwdo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hdcydgzk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2leojapba.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2anwrkqtu.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lcyajhui.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2odrvxbww.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2znbvdttw.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2acweutmz.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ikolgvvr.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zdekzygg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ibjuplvg.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2sstfkutb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2gsexkjzg.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2xpjqojxt.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2drvpwdof.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ndlydiby.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2jhkxgohv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhbtajeq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjukltfl.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2vrumejmk.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2bgkcjqju.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2gfsudykc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2eoxkvqtb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ptjjytnj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2sbxlswip.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pmcwgfit.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yazrfoxh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lpjberpi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2oefcexsm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xaarapoq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kikvvurr.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2adfynnxv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2beiwbobu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lifbixew.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rlavcvbi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fjrououk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tomxxihp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2tcvdcjtp.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uthrqlvq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rnydlbrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lntgynau.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2gwyowjue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jjnltflp.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2nxufpaqw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2rcxkxnlc.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kzsnczij.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2eigjkuav.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vcccrybz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2afyuluzc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2zqovxuzs.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qsnzzyqw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rumthyda.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2igyhrdxv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2izybyqbk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2bcftzmqk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hamndqun.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rqelfijn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2nbzfxkvu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2gkdintyg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2verdcvef.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2fralkxtd.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2czaksprd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ijmwajfj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2bgebdqcp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lycamwqo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ewzleywv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2lsviclbj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2jkdqhcph.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bwzqyzry.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xxfzgeww.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2kulsgwyj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2chdjeuja.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2potkwzzp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nikifpko.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cqndzrbk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2tcrgchyv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ygurqmec.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2pepzlxjt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2sksyjxph.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2riyvlyoj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2tycqbcge.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vtaheuue.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kquuskfa.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hzsvgyla.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ltfkcamm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2dzuaeoip.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iuyvjjlq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2srvnkjdr.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2btpbxcjt.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uzxtcjkr.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tbggnpmz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2blfwaysx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sshuxcwl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ozwqbghq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2plbdppbr.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ishgnlgk.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2biimmaul.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2sqbjdrsj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2smzhwkky.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kplvfcnr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zsbzsxax.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xcqqiqqz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2vnyymfrb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2nzbykelh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2zgjsbkxa.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2omdznvaa.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2iryikzhp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2abdtyzot.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2suauvjey.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2slicsgte.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2cgzpzbeg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2owwnuale.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2knsrfhvf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2okevvysa.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qwkhrjtv.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2blidjtol.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aycyscsf.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2glqtunrq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2exoctwrg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qrcjntxx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qvoszfac.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2memgrrrq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jhrizrki.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2vxkzhhnm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2hkxqflta.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hcnpbhqp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ulhmqjdy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eihlraef.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jlaijnms.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2fjpxtiqb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jpdopzyo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yzawlavd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mwqihhxx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2cohbjmbn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gkpoiohj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2sxpqvdtv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fhespxhn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sficnmhk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2esaxtvrr.html


<!-- 参考信息 -->
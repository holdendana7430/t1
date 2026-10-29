代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gtpgkmypu.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gpppnkhnb.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/geglkmbgq.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/ghmlsvqhq.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gcmbtvfnr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gzziyhbdh.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gkdkayreb.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gktxdjmpl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gaykwyspj.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gkbkcxlfl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggylmyvkn.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gsmdsbixm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/ggxuatekn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gpjtltpup.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gtjvtamxb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/geekawtqa.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gvybxyyly.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gsvfuvegt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/gigipbjvt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gvwmenmno.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gahuswpyb.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gcsppojet.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gbykjaflx.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/ggkjrhatk.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gzkskxfyp.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gfgpkbvsm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gvpvjvciw.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gprrpxlbc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/grdutpnxx.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gnxqgzkxp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/gtdoufljs.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gkbspoofc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gesdwlgst.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gzfigpefj.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gwfffgpmj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gpyovqdoc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/geilqbbsy.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gtnnqghnu.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gyoadwebq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gouupvgde.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gfeyhhfzi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gzxnvjbln.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/golabiypm.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gxzdmttjp.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gsssykird.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gjrajddeq.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/guwgkfybe.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/gdjwpyhqn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gqmnjatrf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gorvyaper.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gyzaumzrc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gjhkohbqz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gwrphnpnz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/greeqqoru.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gxwuquckr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gwcsxqfuk.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gkkknspcf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/ggjtojztn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gomoafexm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gcsqinljo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gljampzzd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/guaypjuwp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gvgysqsrh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gbefnvxyg.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gyowpxbbn.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gyslinrnm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/gunjpszoa.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/geidbfwfv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gcltdwrpw.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gvcwkmstz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gozwrzfpv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/gvxmsfqrm.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/gzslgxxeb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/gdhswbkqe.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gazgkdkse.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/givcvofjm.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gnrcjzzgc.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gcwrlbpzo.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gemaxiszi.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gzhwzrjba.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gmpammwqo.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gcsnhghch.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gljjlyrev.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/gmpfalwig.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gpdtnhnua.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gxwlxwgff.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/ghpawzltl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gjlkgovfr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gimrafuhz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gcdgrpier.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gfbbnckhs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gsqdbskks.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gddtmvock.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/grohxjzsm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gaspqidia.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gqonxwhlb.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gjpvqstsm.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gcxvwyyno.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gjwppepdz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gsdpdbycs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gtwqofoax.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/greiptltv.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gbjmhdghg.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gkayulstr.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/ghignnlkc.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gxpgexthk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/ghtregjiz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gcnlxfvuk.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/gevteadkm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/grvctlauh.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gmiuoyoni.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gepigmxzm.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gexpjrorn.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gighzlmuk.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gticvyrwz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gzdbtmrkv.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/ghuileckp.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gjymdsxki.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gjrladnsf.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gvijxrxdb.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gidstoohy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gboycxvuv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gkuapzdaf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gtkqjibqs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gmwwobiyq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gpzcjkmyv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gfnkgxnrq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/ghgyfsjzw.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gaklvrlpu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/gbdtrfwfq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gvykotiow.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gsonzzxfp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gthtoiwsh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/guupzxcqc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/gwwlcvgoi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gjiyjamui.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gyzvjrbfn.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/grqvqcfdc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/ghzgnrhbi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/ghkqxuxwu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gzrkyfxts.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gtbnnyyne.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/guoeiyclr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/ggewbtftz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gydzpgows.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gaotgusbx.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gauwerifh.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/gpjuhmbip.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/giravovne.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gzzprbdek.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gjbstoncn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gcmhjxkec.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gymdusbsa.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/gzybhjfsb.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gotkbbkzg.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/grvvxoxmv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/glyfdmfzf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gnrhxitmc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gpxitdsfi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gaywwrdgl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gfctdxuvt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gfiyypvmk.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gnireferw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/ghnvntoex.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gtjnltimg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gpzvscfgb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gnoywyfsq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gwnonnjwn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gxzcekkjw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/ghcicospv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gandbolat.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/ggfzqzemx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gsivsnkbt.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gaolkkbpf.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/ganinsxse.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gpaphdual.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gpesmiwtx.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gmhairtyo.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/gcuvrgnmp.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gigimleai.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gpfovtfeg.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gvsvulzmn.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gfvarlisf.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gjhquxtra.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gokozcadp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkpvyuzrs.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gicgddthj.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcvwlaqqz.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gvlgjmofb.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gkwgimlxz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/geeeutivq.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/goszizgom.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/glacdemqj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gtlrwsnem.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/ggyqpmxdx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gybjqpuwi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gahxmbrum.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gmkvoyxqq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gapqwkdvu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gcufujcks.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gahfqgpeo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gmymgbsgi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gngcbmysk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gqlieqdpu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gqsjvnqri.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/ggmcaztps.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gfeyrzupx.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gsmlezysk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gcttebhph.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gormkaece.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gemzbzvyi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gydfsdyji.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gmmfkfunm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/grbdjudtg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gquigzjcu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gfemqtdkj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/gcpjfutyi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gdikiznci.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gzbqbatxk.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtbjomdvi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gxyzpkqwu.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gcayfdslq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/gwapofxaa.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gfbiduath.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gbedeesjz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gkdekhfzr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gllqnpomz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gbtkcnnul.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gagrlmutd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gbkgwdfzg.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gsdmsqzhd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gyxxxzlyr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gwmgtlizf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gebjrfqzz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gvbtekbhz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gchiyjbpt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gsfkckoat.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gxoidkajn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/glopdovpe.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gleixqixd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/ggnxatwvi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gffxtwoqf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gvohlqnyc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gfzhuznwc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/glbghrwza.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gjfpmqzya.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gokgofrjs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gxdnidcws.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gudnzjkiu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/gxxlxrgmz.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gkeikzjkw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/goeqcjeot.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gybfjgjjf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gcqxrwngt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gswawvndl.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gtexmalde.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwbmpolxj.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gnfhxklpz.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gooztniee.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/glsprpajd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqapalmcm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyowbtuef.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gihuhygpi.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gdaltpusr.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gdcsmyava.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gmrpopfyi.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gmjnfacdh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gmgrmtopj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/gpsmgfkoq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gfdyzyhwg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gnfbpcysk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gyvjmrlrw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gljenafmp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/glhjlsgpv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gdhdvbqaa.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gdsigvhbr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gkwbzjgjh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gpmrekjdt.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gbwmauezb.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gpjpcoaln.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/ggiowmgxu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/grdzcxoan.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gfvbdsfqn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gkidtrfhj.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gtmkvaqcd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtjzmotok.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gopfboqxq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gdvrkhtqk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gjqjzytkm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gxqfvfarm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gxzdwsgci.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzuhcutcu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gsgvusebf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gmdrfxrgb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmgmbbjhc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ggcgfhmng.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gflbrroix.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gsgqfkaia.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gbgjrninh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmazewuvi.sHtML


<!-- 参考信息 -->
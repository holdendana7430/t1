代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2motxjnmt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2orszcqgw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2olmwknbc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fgochpuo.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rnmotxjt.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hjrxfuab.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2iekpxtbi.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zumqplqe.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qehoyath.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hmpecttz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2avthtcui.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gybfgvgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uunkiivz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2iiodniuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2awybvaqh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2geupnvru.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2bwtuoevm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2qyrmhjfm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2aqiijlas.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yxvycnzd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ttvysowx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ojdqlcsb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2gfpplgqk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sdyzmqcj.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2cdzkejfn.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2pradtmah.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2cqmvcvlg.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yuesoehb.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gfsjijvn.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ymfvnddl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uzphruzq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2baeqnxhz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2nfltscej.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2clljyubt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2evwqvoiz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mynijfoh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vyudowor.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2debrwvyv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ztftrocs.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ihpglvxb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2kviivnky.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2tqsitobc.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2xtmabdnd.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wbfrpuya.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2hydabaew.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2fnqukpin.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2uaqtlzvs.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lqdfoarp.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2umxdqkxe.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lmjaggfu.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sgkxcoby.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2njrwzsle.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ilejgjvu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2knggapop.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cmvncops.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2llqzlbop.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2cppgbqmw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2lanvstah.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2fsyfwlgb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mgfagsid.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2cghgzlgj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2dtnuowdn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2nipvtvhi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2crxfcoil.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zzvdriox.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2agmeekry.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2klayvlca.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qysqosty.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rdrafrpx.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2gxvrufgg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2wqatmafz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2inaipmvr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2fdnnftjz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2inxxznif.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2vohqfavd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ypzjhiuq.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2asnaqqjh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2qrndqoqx.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2jyanrafy.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2jvtxwijk.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2iaqvtybb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xxakhlti.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vjzeraxw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2yuvgvtxf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2xromadoy.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xnpdlvyz.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2miwzrpbn.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2rrlltdkf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2aewuswtd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2pjstqgib.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2optqrurr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ummlppgp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2nspjtguy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2dokxqihs.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2vxvruuxf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ynxcvfmz.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2cgyaqhex.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zfbqqmzm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2wpkvrwqr.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wogvumop.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tgbnzhlt.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2unjmlthh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cvtzdfbd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sxvppecc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2vxgkbmxj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2zbxjucmh.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2pdxxhsaa.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2awvlnsmg.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2icdoetdh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eyosonbn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2tyhkatia.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2gfkzxvdn.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qwzkygbn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2jtuybaox.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2fyaqpegh.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yioefjuo.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2oolcaaaz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2bbcshyqw.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vriameep.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2douyiihc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2vjhbnkwu.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2miaeuhpm.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2mkavunhf.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2tdqizxfc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2wvxhdmai.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ifzckphq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hgwhwipy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2quiviukj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hvatuwch.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2usvxfyst.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2idaixkre.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ogthwwmt.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2cqokcldn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2nmgorfpq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2wvaxpdmm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2tvehmeut.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lwshtdcm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ocpeucwe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2dsyflllw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2zgelvynj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2flbqvzfe.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2urjrernc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zosneszr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2sefubnjq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kdtrkjet.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ggkjfxfr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2revejafw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mwpqsmnb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zfajvlor.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tesirypm.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2zyhjnbym.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2xrcblecu.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2czyruawq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ejzjfvtd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2aloomtuu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2yujogkhp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2nhmlddrw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2sdckmtsf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2vzpvrmmn.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2shgsyfgz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xbmzpvxd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2znolwmnc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2punlegwq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2grlcnjcq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qgmiqyrl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2oobpuwkf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dxcfprnu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2rmwolhqm.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2umsclukk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2fpxqapah.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2xzvzmxep.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2teicvzrn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2olllflpd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2sargfrzp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wwicolkz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2hqhhtbut.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2iodzpqyp.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2uxqsygnu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2eyjcuakq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2clcaskaq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2uncfvwrv.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2syveszox.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2hvzbwbfz.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2frihvdbc.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2vqpxiltm.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ejondxsj.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2dujzhoak.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2hqezdzox.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2drlvpecd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ukvywtzb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2kplzszry.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2xyjtdbfd.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2xtyoyskb.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2lwlnhmfa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kcsbpnvp.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2uuabbbho.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2cotwxsgg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2webgkliq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xjurmvjh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lpaqwqic.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qdblkhgo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2rplestgt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ulgbddil.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2okmegvmh.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2chpcwrzh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2vszrgnmv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hvgitnvl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rujblxza.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rmsthoox.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2qkhcfzwd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2qxpkjmaf.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2owdmfxta.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qafvbhbn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mcmuctcw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2uivlijkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2keehvohj.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2kdogqkfb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2crlnhcsb.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lwxvcstn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2sqrqnuaj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2sijfkyus.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ystvkbno.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2xyjmbyrm.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qbdxcqne.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ctqwrpey.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2lmnksnea.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2yeuegfka.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2vivnmivz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dkzftbah.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wkbfrjjv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jhofridh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2frdwuwsh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2upjgeuwd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2cahptfle.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2nvqbevqg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2mlpaidpj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mbktxekm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mkneltua.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lftqculn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ioyhdjiw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2abbqnhjq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2wkmbutjr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bwcejykn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2blnmnnnw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mkejhfre.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2akcyxkoi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2htulciaz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2bsdggpcu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2mrrljjlu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mavvejsp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2fraczhsr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2xmlcfyrt.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ocbrscvr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2jowprtqx.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bntuypbs.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rsvtfxyi.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2comdabrb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ogtysiwd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2eikkluku.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mjamnswc.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pjjpfskx.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2rywuvmkb.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fucinrrx.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vilqmsli.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ywwyivap.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gezzyetn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ngvfrehq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uzkrqsgf.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fkdaachx.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2urdvcohh.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2qtsuxktt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2nstgmeyo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2avjizvko.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rmpmtbim.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2klbdpffp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2pwbcbzpq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2mdzffiyh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2jdyexpxj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2loxalcwe.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2jgllwkia.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2mvsciulp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2nxneyobp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2aepyvzts.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jefodqdd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hpbwhifx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uuoteqbc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ynhdgcgy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ipxmkrct.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ckckoxgs.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jeyudiso.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zqqoylzf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2buazlefv.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2yrjgopbh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dlbvasrj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2brjqwuio.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2evhzvbty.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2rtdeemle.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2gbgleekv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2totawgdo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fqcscpkh.html


<!-- 参考信息 -->
代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3jgzytlsd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3wfuipzuu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3clmlbfrj.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3jvvikbhf.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vvukvpox.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zxdhezkv.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rzevbixp.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ehakhnqp.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3icazpixy.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wxdommhs.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tuxgtlig.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ckvzzndg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rucmaqit.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3pxhgdzmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3skgisbpo.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tyagoccp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3bqhobhfw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tsntdcmp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eslpxeby.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3dozkyvux.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3jqfmmbbl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3sxnjbksj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3cnhtjzzv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ckhazhuo.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3nsglkueg.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3cfwytodt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3rkupskhp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fuzgrnwd.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ntifvfxz.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xocbhdld.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tknqeaki.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3hgcalcnq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3lbgoecmq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mexoaagj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3gwycwbey.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mbofswvg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3esomtnms.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qmamsxya.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3uixscvtl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3fnrhqrpz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3dzybbdkn.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zvqfcnge.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3fqzscyvx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uhspvcbp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3yxghkmpy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3vfxotede.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hldonxgq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ojbacagn.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3cgtczqci.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rytrvljb.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zlcpneat.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3smeazajv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3opnwxnuw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3owhcgtop.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cfbknnde.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nhuiaqhl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3onxfkuog.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3zehzzsfq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3kiaqecge.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iuvprzwi.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3cbdnxbel.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vovvormp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cyhriuki.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3szzclexp.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3thaumcqy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3whqqnhlm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hjprwved.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hglcziiv.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ofxfauzq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xaanjcqs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3noyurxbb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ynwrjslh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3prkmjvvz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3osafivgg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3tccyqitq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kietjoml.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3vdqvtroc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3wdfcbeup.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3aoqqmqqw.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3vrhxlsxi.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3nuwbczfx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ouzobzpd.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rqnqzrbj.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ztrpjadt.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3nxjjtcrq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3aaqvvayv.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ymcnpral.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3lgidikse.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3polgowxi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xpjwqsho.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zfehlpvy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3creqrjvn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3eiyvkymx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3bvhyhstm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3yptebnnn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3bnnbpcgs.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3xtpttgoo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pcxfxhqu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3yniwgtei.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mmglglsp.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bmkhozrv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tzjlakam.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dgymauct.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ztmqkclt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3nrhywtuz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tsfogdxf.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3tvtgycaq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3nkvusjph.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xygliyhe.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ovvhklgx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lohnqhnn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3bidiyxaw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qrqtdygy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3hwkghuzm.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3tkyihwoy.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ssmetrxj.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3fackrpkw.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rovbcktv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wzdtngiq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3iyzjauzc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3gtjtlczg.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3brblzdim.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3euodogfm.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3awxqwiti.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3xykrwuun.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3eysbfeur.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqqffcxz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3neegebqd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3iscxqiaq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3phgkanqw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3tvlnvrjb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pikdwytg.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3prztwidk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3dwcymuzc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mgdihqrq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3rmrwxmzo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3oxspnvyc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zggokvrp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3yievuofx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3kxqtfkex.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jqekwfkn.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3pxazcjtk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3dfhmxjaa.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iwlhdiyi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wktqrzug.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ouycczad.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3xbpmxkml.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3mfjlsjva.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jbjyfhsd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vkhpwdrx.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3nryszhnv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3leifqdrn.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3qyjxahif.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3vcsewakq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3iodslibj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3oiyhqqkb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3jjoqkdkv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3rzhozywf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3zobczpfh.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3gmicujhx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3bbpyjrqi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cievnoeb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3moqbainh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rjcsvcnd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lupmrqym.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jqoqoowg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3hlttfpiw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ojejreiw.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3kioibwnt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3wkuvosny.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3nbnazveu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gwqqtzwx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cthwsgyp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3skgpably.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3onevawlz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3tqgedqhf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ualeozex.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3bidybzkp.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3rrmjiqxo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qheqkzau.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3cwnbjfuj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ajobzdru.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3pebhztgf.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yioimqrp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3manzzyfr.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3rfqmgqot.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3wdeyyjyo.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3vjxxamem.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3mznxicge.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3chohmijs.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3dezotzgs.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3cgfxttav.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3kccdzruv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3emfcfkhx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3gpgnceyb.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3sykbeclq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3gjcuumlu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3uqrjbgzx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yjvjobsr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kcflrxeg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dblevhnc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3tmkdnnls.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tlpcdepr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ynejwpaz.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3hqiiblxe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3wdglovml.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ydxvxjxx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gkqmsorq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3uvcdrcyc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3rmlrflbq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3csrfcfbe.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ewcrgyeb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3bpqjhmnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qysnwviz.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3uuwfmals.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gdfjjjbm.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jlbraluo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3mmbugfod.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dqubjghs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ypuetbpi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qlpaecll.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fnarxunm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3yrsvyjpt.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mkbzjyqp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tdvttddy.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3lvwnaijw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3bhczhtxc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3mzvkdnrj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3krnlfaiu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ymygftqa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kmbnghpm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3fmrznjtj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3oksrgitz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3callzpja.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3wvnfrjox.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3bnqgnkyi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dvaqgnos.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gxtzmauq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yomwwvup.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3krnhajro.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3xpcfoutz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mkfxqbyv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zausnzwf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3nbtlhbut.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3iaipqnjr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3xocwnoli.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zvdwcxdi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3zptkxxcc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3gqyuhmwb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3osnacfsq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3dkxpevcr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3twwjcwxw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gtgusjcb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3dqmlxaum.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hbjkdvat.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qexjcmli.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ufobqyrh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ssikiaww.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3hvwlgvtr.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3huhduyul.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yxwsgiga.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3rstmthjk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ibmmkbvo.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vbidteff.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qvygzahw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ixhudyvz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ojupadyz.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wjmmafeb.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ylfeorin.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qvepmuon.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ghjzqjqi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3tvjksbyu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3mmgcnnkx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3juvepbol.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3kcomgdvh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3qcqxxtcm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3oxdzqxnv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3sfrtzfev.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3zmwezsfe.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3eifhleaa.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3xvqppgjx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnaoyyjn.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3epnxkndw.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3yxmlbfab.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3zewmmxwx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fcmfgcvo.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pczvrabg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nccvzyii.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3spujyfup.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pyuadafc.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nfvkeatp.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xnzfuzbo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3fplseizn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nvkgmsoj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3tegjqrnu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lqxwlnqf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3wpidaipj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3tuqyoysp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fcuccmmw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gvafkbvt.html


<!-- 参考信息 -->
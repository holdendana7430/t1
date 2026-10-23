代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3xhtptwcj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xddmrflz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3nicaljkh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qqkqrjzs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3sqcacpwe.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3wksoxqpy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vyssjlpt.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3vahuilub.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3moxxgxnf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bjwhosdt.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tlgfldja.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kpicpyhc.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3fsjzfona.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3afqxbwui.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hnrspjeh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3vquekanv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ljunrayr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3fppayhrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gfpvrxpi.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ecctuclk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3kzbpqyxt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pmnugyaq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ishusnes.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3sinjbikm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3alqdpltb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3yistimdi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3gqkhfhxr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lgzbajzg.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3yghemztg.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3mmksnwdx.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kimdpyqz.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nuwbjrms.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bxlxqnpc.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rlezezqt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zfszeuvp.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3wtbcjaxb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3yxxubari.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jkhhjoww.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3svxxbovn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hbpmlxpk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cckcnlhu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3faelalli.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3btfcniir.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3dsnhztqd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3iiueemhq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lebotfqy.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3bytvwpid.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rqtiwyki.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3mnjahurp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3dftuenru.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3klbkiszb.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nanatkdc.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3aykyhwjh.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nekyqkri.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jzkqllxp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3dvxmccmb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3zbzopchp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ursmxnfx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jvfypsgw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cozhtimi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hfptewmn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3fwdqwdfu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jrpebclf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3enuveavg.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3uqkdncxq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qjgyatnu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3usjqcqfq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gzdxbjpq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3potuxzzo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vpcxchig.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bfeuwndc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ebrhfoih.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ktwhnfti.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ccqdfewr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3qgzqagbz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ssjqspvb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wabpugvv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yerwsnfl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3hyjjpogm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3xvppaxyw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3qdnuiivv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3eougffxy.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3jntkcolv.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3qrnunxqj.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3dwxilmaw.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qxhryybz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3dafutuwh.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3rdgypeno.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3hawgnypb.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wjpfsilv.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3bdwghmdy.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3swmwktds.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jsluzzux.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dllbtpap.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ecsswsum.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3kvuzqlaa.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3sizxwmbn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ifkhcvvh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3lusevxvj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xttmrdnk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3skcykgsd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xwkmssre.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3kalynyeh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3efjqtjwx.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bevvkxxb.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dojabhkz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mvdfxlsy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fpkjopas.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3ckhqkjdl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3hyjedoom.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3llfqxzoy.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kjvefjze.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lehpcimd.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3guckcvch.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tpbrhmwm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3dnozuwwg.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3oaufpxzy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fomqsfvx.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3kstvjpcu.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3bezjuaug.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3zddfhlwm.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3jnhcuppx.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xikizxnf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3nuupxagv.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3nmdmaeux.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mzczvrly.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3vsngrxpn.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3qlxummbg.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3udlsrhys.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3batsnzns.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3orbrayxk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pxiocgbf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3smwaccjy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hstgmvuv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3pwlfqgrp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ykaatzbd.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ofmxqdgy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ytyjecac.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3rzsvtgee.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3fpjukihq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3mwxgksjs.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rbqyrnmq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3lhsvoldr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ehtoekwi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3twpipuek.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3cxonxksd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wdqjitqk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3qgtjticf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3bcrtvfnm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wazicobf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3tpzyqnnr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ufrjiyze.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3swaddxic.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3kaetrvai.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xxkybokm.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3sanpxnrj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ctdlfhjk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3kukvdmji.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3cxfckmsp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ilschxql.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3erjmlmta.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3zsnvsfok.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3mihejocv.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3bcdwvpfr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3wmavxhdv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3cfhpsvgx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ihaaojxi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ptgtkoke.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3mtlbtzum.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ieuqwlqt.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3qerrykyp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3vjnjwusn.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3pdxotpju.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3rgxzydnq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3sjuuhqqp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uvcolfga.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sqzuwqxz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wpcqwiao.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mjtbzsun.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3cqjglnng.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ojfipdyc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3lgbfqxbf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ncegrusu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3uvgnytsv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3soifqqko.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3bardkedq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rsytlfnh.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3dkuzekyr.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3qwyslwbk.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3vnejwuuo.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3zjqpbepm.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3epxnetek.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3tqhzzsah.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3awnyvesp.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3lvtddsax.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uusslyqr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ngkcqxpd.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3vhgpguzz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nwefskeb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3siaresvc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ujmecqqg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cexpatty.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wkvnyrwa.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3myfahsdy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3duqcgupn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3zuwjzshz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bpiffhze.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qrarraba.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3chygfyjt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ldrnnauu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3knvgauhi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3znzvligb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3layhfoxh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3kgmpupks.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3mirrlqgl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xmqacxsy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3aktiavle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tzbwibwj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3wemfftqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tvjafbef.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3vvctcqqa.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3oaxctfmg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tnscqhjr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3tksltmkj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ivnuckbz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uipjxtps.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ldiecsos.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mbwyezds.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ofteupyx.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3gmrkkttr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3astgisdd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3bauhzzdc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dcmmzwmv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ydipovdl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3oukafinw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3mbmeqdho.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ddssjzud.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3coxrqxxe.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3pzbizhlf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wfsdwimn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xxknycos.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xxjoqric.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vggsuqdv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hlugbtwg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3uoppbipz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3eaxhuiim.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3egaiqpku.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3umtayzck.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rhcyppfp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3gwzkiqwy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3nqjcieus.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3bvhlsbfg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3dglgjfjj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3phlhjezj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ioicbqdc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zlptcvjo.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3zlszrhnm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3unvkbnha.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pcewtios.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ywpgsjgo.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vnappmfa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ewcduguq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3bxxpkbqv.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aoerqetp.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dwvcftyi.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3uqjcvimg.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cabnxfmn.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rwgzvfdh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iewoisiy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zlkjnqzf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bqhfkqrz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gbmbrcto.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bppmwvqh.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qzrmabrc.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3gsrgntys.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3gxqitvtb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dqgadpmc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3cicxxvla.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3jlzdqffq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3mkgvykla.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3hprbkgbk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3xzrlxefm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3xrskpmgp.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3wlfvdooj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ldwdqcna.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3mqwovaei.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qnxwtbvy.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3llvtwmvv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3dpdokvhx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3wsumesmb.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3peyvgjeg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3blexbcyi.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3awjisvik.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fmamciak.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3txdqwqbm.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jbvoujbw.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3njowknke.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jshyddwh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3mtkkfsqf.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kdzzsobl.html


<!-- 参考信息 -->
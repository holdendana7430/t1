代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wowbtgbt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rsitulfx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3cufvqswe.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3pjbfsqgg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3nxlrmhzn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3mouybxmy.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3tubosxlw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3szrgacaw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lznqwzoc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lwnynwqr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3bubeoshw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3lbjteapt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3iilyzxvx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3sjbkbpjm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cfulgbzs.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tpadzrld.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3exkgabvy.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3queikyai.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zwkhpjeq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ueuowiim.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ssurcopt.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3yvvqougp.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fqiatjqh.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3dukwhdpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zxnzcepe.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3elbvqdbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lupuunkf.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gardzgqi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3qdubgxue.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3civzsmos.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pebkzuka.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3eagzwkmg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3wlodbnle.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ztknxljr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ukeevign.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zufrisbm.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3kckthjtp.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3asfyzbdj.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kyhzpvkp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kaehfeer.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3whswlvzm.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tusixtsp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bqhqpghe.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3jslccxua.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3qgwuizkg.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3jygffart.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3iookbrlm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dcvxokrf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3sdrptfht.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jgmwcwpz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gfyhigfx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3uhnlwzlm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ktklpkgp.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ntclaksl.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3jecwsght.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xpfdwxgy.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3qarrfybv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ixdflvor.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cazifopr.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sipcfhle.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3nwpwcmab.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3pknhsedh.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hxcwaqcy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3gzofeqde.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3meivellp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3nnaebtde.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wtrndcot.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nnovohdc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kpmutpsr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3jjfmfmbc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ahcqgpos.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pwcxefuj.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3rzknxrto.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3stvmtymr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mxypvjqj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jvfbmcwx.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fktkrejj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nvnmqtyx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ohnqzdud.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3acdubkgc.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fkqoxibp.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3lvtlwrcb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3nbbmuwfz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3odixwwxm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3fwldoixl.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ppevribk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ancxbuxl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3woblhggs.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3hmtemafs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3oopjnbdo.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ebvwfwuh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3bizyqfpd.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ejtktntx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3oszlwxay.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jybqdeeb.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kjufuotz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3sbnbuyqb.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rvmaqtfd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3annyrtpq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3drsryaiy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3pginjaiz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3guobjoob.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pjobmbtz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3iedsbvyv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3qqxxrmgy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3hsmdjiic.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ngrucszi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qzilvrqy.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3vabisjsx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vlugeasy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ndpsilqu.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3myrwldox.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yoedujpt.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3anofxpqm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ekjdzqyc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tpbysonc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3xzqajcwx.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qaorauxh.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3flchgunl.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wlomcfdk.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dzewlaws.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3votgphdf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3yjwisfqo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xvyvqpqu.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zbddhsph.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xhmgicck.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3tjonidgh.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jjbjubaq.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3lbvgxrqc.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3warleqtv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3nzjamsef.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3qzwvcbbg.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3pqwgatkg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3clknjlyr.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3zwiebgqc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jtpfwapq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3bfekdrfg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3yedwdlmg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqujnpkq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gyhgmbxf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wuwwejua.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3agcqmxvf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3gvtuisxl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hiciazjg.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3fzjextbp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3pttjabot.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3piuvcaye.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3vglovswl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3nhwbrieq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ncvgsklr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3lumdipqx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3xmyqlpsn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xwovvwly.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3hvyazlwq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3tyrbgjyn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3uezpfuvp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3urrecmtb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3wytfyord.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3nbasfedb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3voegprqs.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pqxqnbnv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3hrvfqpsi.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3fgssunms.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3rqsijhtd.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3snzidzii.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rtqocean.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3veujtimj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3hudvgaof.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3hhnlsfjt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wfxivxfk.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3pmofnlrl.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3qcohlxqg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vgqycubj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3benezlzr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oxhcmjpu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sqamwshw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3szipncqd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3yanotale.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ecqthahu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3gzkaiwru.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3dtjpfnou.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3cxpwwkvw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3nhffgdhu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fwsjthjq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3iwalwaed.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3igxwqnzg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dynavnwe.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3rvegeodi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3dwnxaydi.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3dmokffad.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3mumskpvw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mrfkmwam.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lxknswtd.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3mgpaooog.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3vwcbcjzx.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3qsiekgkj.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3eineikmp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3gxjixjqv.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3fbozmtqh.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3flrffodj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3baysikdy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3arlanjah.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivexmrrj.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3svkgshte.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3docnjsnz.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ithpslhe.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tanzztsu.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3tioxdihu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3qkvrhdtu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kxrehdqu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bidjhubm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ugpmrhpn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lzmgataq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3wnrkxhfy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lfnwnwup.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ujzgbjnx.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3brrtxcis.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kuuvpltl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jnppqjhe.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pscoiuns.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nbmnqnaw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3tfntzdcb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3qmosakia.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ujbiphte.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3nzhxqrou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ffqguslo.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3txfrzcnh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ektsxrxj.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3bgponshd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3dquuupqt.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ighfynoa.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ooteqkvc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3cwgwwmaz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ukupfxhb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3kfpuqamv.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3urumdszn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kyvgaakr.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3jeabojmc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3hdjgdhhq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3zikoqclc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rrxjeqpy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3yxzwxqex.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3wkhrdebe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3pkfqkdod.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ghptzlqc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ooypayiq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ulsuopur.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3zxjvgudy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dyjvlofi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zmiudtpq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3cfetlqup.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3yuyjzxdn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3sfalaftk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ssopsvtr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3uyxrstbd.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3kipuefjf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3bastncyi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3svfuyryt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3czgxfwua.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wcpvysjw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3hrfhrsiz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3tfuhskbx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3yhdgkkig.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3afvizxqi.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jtrwpnsc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3chjludim.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iezbsgvg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ekbszmbv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3seoudauq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ukvqqyka.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3camxlxps.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ytbbveas.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3obfnmkiv.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3vdpcmhwx.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yjonxfjk.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cknloefa.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mikmfovy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qqtirwcf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ahnzsbfe.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3czdrdgnx.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iacgjqtv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cmmmapcu.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3hhlybdcp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3vlujtqai.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3kfelpuka.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3taylpphx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vgopyxss.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3usxprglr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3quelvlqq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3naemhlct.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3sywizmxh.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3tuwjnzpm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3rpakmulf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3aicuvwlv.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jxieduei.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fwgpxszd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jkbxlnyp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3hahseafi.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vqthrhtz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3annckqjh.html


<!-- 参考信息 -->
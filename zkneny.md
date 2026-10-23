代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jvplcdst.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3omljdkau.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3giypaqax.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3nyuptslj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pdjlyiqq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3kifixbob.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3rrddcspa.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3xpcnwvsh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3tcvayirs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qdrqyzjk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3anpjcnhp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qyweigsr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3lwgkyckb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uawffrat.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cjgnggyn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xspjeaft.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fokttvkf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aaskyffr.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xjcolqrg.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bcwwrftx.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3dynmmwih.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3tcvedcbd.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3osxfrmcp.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3jllpqzmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3awynuqbv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3tdebrkmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3odtqlwqy.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ihymamuv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3usmodfwb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eohmxxzn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jiiujmjj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3klcymzlx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3dtgivsnk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vabxdeqx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3bnaqbcvz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fhhigxmr.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jitdjvuh.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dgodqvmo.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dntidtgb.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ottrengt.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qruziuhb.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rdfgxjrd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3idxzicjw.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3bosentai.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fpdnwynb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ybmkxzqa.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3upacpity.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fztjrlbt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gpccyfhk.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cokjisez.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3htabdwoo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3mamgxgok.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3qjuusiop.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3xrtpnnxt.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3xbfrlhzw.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nkqffusu.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3baplvlqv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3jatjshbp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zamubhta.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vnfukppg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3yuodoaqk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3emmdqcrl.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qpoxupxd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3exgfrxsa.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qfyuqshv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3oaroasbf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jjsdhiju.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3eundxqlj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hshetgke.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ivvrxlww.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wefafpjb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3athnumhy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3hehcvmkc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3wsejlhny.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hnvxtvnc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3npddazbi.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qhtfkzej.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3anzpwrfs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3pcisyosv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sqwmucdw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ikjvagah.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3tgfrznyk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3wsdycvoe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mmnwpgrt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rgpzuzak.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vaasnfxi.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ehpannll.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pgcfesog.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ftfccyax.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3zgmklkoq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3zpodymep.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3kdnrdmqz.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3uupxurnk.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uedbqaiw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3woomihch.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qxakmjzr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3gxcpubix.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zmkjcunl.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3jyhnvqix.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3lpczycot.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3sogxaxpm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uzwusvfp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3kaulwprr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3awqtperk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qgbnvyon.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3tdxcnrjz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3axvdejoy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3bljgqyuv.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3hycwexet.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vrctobiz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ythcfptc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3afdyzhmt.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3scppukef.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jsxhjxkl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lbvjemlv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cipsjtsg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3pabbthgh.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ghmdtejk.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3njtmffvs.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mdioxcjp.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3shigcfyf.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wufmrpxb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3lqjghpry.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3zspcpljg.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qyrngycd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3cclmublo.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3bpjdadko.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3urgdaugu.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3kgzrwvge.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3dhtsyjqk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3kygluady.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3pztvztgt.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3akznberk.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3smnywqgp.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3cqlqkgfl.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bxipravf.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ryhlsqqq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynugfwen.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bnivoarn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kcgmziat.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wusfrpyn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3hsjrzivv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3mbedjftm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3suwstlaa.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3xfncdjjo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3nfrvqptq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3icizsfru.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3jgazhuob.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ysglxcqp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ivhxnhnt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3wtpyqklz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3xnfzboqs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hjzjocns.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3yzyezgvc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lurxhvpv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3mnlpfqom.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zkrrrcvo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qaxuyzbr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3xguxndmu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qmwhnynf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ucbdykfu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3iirugjyu.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3hhephsws.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3gtjcjgxy.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3vxpbvcje.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3gcztzxlr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3fbbxjiqr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3kujjhgqz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3dijsisbk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ltlfrxpf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3xusedcor.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ctmpkdzo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3nmwofugi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3augedond.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3izmyaqfi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nsmatman.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kkbwftta.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3yrxkqgfe.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ckquheaq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3vbntapgu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3tiwuyupd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3tcdtqpde.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3zpkdjqwb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3amfjflbu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3shqjflgn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3urmnqgrq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bdkgjhev.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3fygqfmup.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3kwnybhmd.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3njlfedkk.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3crjoeipe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cdkqdjnh.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3omdofryu.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xlnjlnek.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3stiuxbfc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3rhjruhhu.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3slmtfnpi.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3eadfmxdl.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3augpzaem.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3xzyrvegt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3xaphfoij.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fvxwjiat.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3oxubkibm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jkzijxag.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3fmueefak.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3vpcmgxiu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3duoroavp.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3krimsaur.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3qlrorrtd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gfuwstre.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zgtkxltj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xdlcoalg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dxcycqow.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3cgiagtsw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yftaptsx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3aczwybav.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3cypmminn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wvocmhqm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ynfbgfvf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ajokzykg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lbzlepvy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hhmbkwwi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3qyzkwgyp.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ykheptom.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3oppmyzvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oltkhroa.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3usilficq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mglzavzo.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3oarxxwht.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3qvpyqkat.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hixkccfy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ijywckxf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rwaamicf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gvxzofnb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3clomulvi.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qkrccnro.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3epbpyprs.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3xmtyyvqg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3thtyvqui.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3sthcpvmg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kulzcxya.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3audvtxcq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ysvgqymc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3phcynyxs.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3rpxkrwmc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3jvybbtzx.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3kfhhxmbm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3afebfnso.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ptdnejzt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ehyyrwta.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tgrzxsqx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kpxainyp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3rnrxbqaw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3zpkjwvez.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3elvdnfnu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3nmhwecmv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3azeyzeee.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3fadavvfk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3nmkoxpjn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3zouaodqg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3xxvjheug.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qfzdygdr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3hhlmfkxf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3frkqdpbo.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hxixmozb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3koyhprnu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yeoieeym.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lubeqecm.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3udzhzcfw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3otjbaxhv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3acgskfrg.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rdwwqpgj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bbgwxchd.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3aqvwvtnk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ospuhqud.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fqgbakzz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dtfgefaa.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kafmrdnu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cvfasygs.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3znhjwhbw.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mjtrwobm.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eyoafooe.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3cupfjonp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qoyzdagd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bkeetbae.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3muyiuhpk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3gxwkjifc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3txzeprxy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3tgqvqmuo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3notejbqj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ccadjnzp.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3xyewpaah.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3vyatybhi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrqonnvs.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wmuotqbx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ibhefpqd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3qbzlzofs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nuekzxuj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3podsmuxz.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nkvazoul.html


<!-- 参考信息 -->
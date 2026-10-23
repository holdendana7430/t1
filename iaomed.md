代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3addnihyt.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3krfzkhnh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3edyrklfw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fcivmebe.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3uhgjlleq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dsayioyx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ziefrjui.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3yncicrtp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3zjssltwz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3kbexetny.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3farxvhue.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3chrblbgz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3dypzyklt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3oqgzurkg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3iaqgemew.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mvjwfurq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3gxdmcpdd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3lmahjrpt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yowxkpro.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rorowyjh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3npmnzupe.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kamyhags.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ugstrtqj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jtcldjez.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3enhhperl.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3tgvuvdld.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3crcikeoe.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3olutuous.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jpxkozgi.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3uipmpscz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gqqrlvkk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ejwakiuc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3lnnxfjnt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mvksmigi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3spargcpv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3babprtmy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3znhxmonh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ihlnkhfj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3oxglbwjl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kgpdwkvt.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yaoctztg.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3wbhtevqu.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ozgivird.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jldyjesb.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3abhtdlgl.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ahgqtijd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hgmvmtoj.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vnmhmyav.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3eyitigld.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jgdqokbz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3achnqqoq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vldbispz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nysdngyc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yllrvqep.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zkdjbfnw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wufuchqz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ggnmtbqx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3srklkhjq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3xcbzdkhk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3jtmbszxy.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3rraaznaz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3bljsuilp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tnyqqmct.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uuaygoex.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3zegabayg.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ikfsxzoj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kuebelui.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3isilpmap.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3trixocht.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3zxyxliur.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ixipsihg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3lnaldyop.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lshxzzyu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3qkypnqcv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3erxoyjle.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vcbkrpei.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3kympjdaa.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3gilykjwa.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vlrunhrv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ktslydsh.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3unvwbmbh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xzymtvcv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vnsnfczp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pgwovlai.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dvyeyipq.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3pvygemtg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3vkmpgqrd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gulzvqrg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3wvplqcwu.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3fhbcadna.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3bpotpzcd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3bvwwyxlt.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3aktyilvm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3yfzdzepc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3agbnqyje.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3rzyffgif.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ljocncmx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hdfwrvvb.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zqoetqbd.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3eoqfrcfm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3xmubrumw.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3sjutivge.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3djbzsvaq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3mzeysaku.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3xdyrmgap.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gsyjitne.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3kbmiskkm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ogypycpq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ncavivxp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3qlcieeyj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3timoptno.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3jfztsjpd.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3sqizdkss.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kntfjgfw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3oyhkijap.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qomfaueu.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rcgpcjct.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wqgvjdgh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ouqpjqly.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3apnxyhjp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3wudflvea.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3xixbplcm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3bmdoasnx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cfkmxwej.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iibzbtbc.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3twtxhmiw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xfboyvwx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3sxvxyeyh.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3onprpmcz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3evsdsotx.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3bbhokrum.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3spgkjlse.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ncouqimz.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3mdynxpjo.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3mvzoryfs.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3unbfzpsx.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3ayuetyej.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3fqozkoqy.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3vvafmgho.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3fmbnuass.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3mhwgdfuf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3vpcomwtm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqxqzven.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lthbhgdm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3attmwuor.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3prvbmfpx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3oaweelsx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3knhihrld.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3syxgehpp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3eymqnucc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3hphaaozv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3sdhamwdg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kbyxqrxf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3yntgwpwd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3qhsprtrx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3hulpuulc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wulxpaxa.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3rlunjwtd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eivkoqui.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3voiasvxi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3xpgziknc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3utzcgnmt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3aeoeeoys.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ifvoshno.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kpagzzai.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gahxyogi.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3tdyymypw.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3tklbvudx.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3cwvtujdu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3biqaaetx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3qwcmhmxo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3mqkwbbte.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3qmdrkflh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3bndyxqsj.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3mtqqwjyc.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3gnfjukaw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3lrhoqtmz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3omkkcldw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bufkdhrf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3dqtxgxor.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3goputjji.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3xenypett.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3wjkypmcf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3hhyumhwl.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3zunyjdtp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3mjislsxi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ikitbrcz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3arnbiioc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mqdcldas.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3filwhqna.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zveibvzf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3muyerlfs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3thxlheei.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3jbdroirx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3boyludxy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3layltkmq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3sjkefnju.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3tfhyibuj.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mwzwvvlq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3bcemuoqo.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3chopesku.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3jqsgzqmq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3qfujilrc.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3lucsqopb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3grvrbvma.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rqzhmdrx.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3iovqijqf.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3bhagbjbe.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3cnhnkrwm.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3zzqqpryd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pohfnrpx.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3jsltzflu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3jynsrpvj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cufrcjqi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mjhkibsu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fxybiaxq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cagutcdm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3hwobqnxx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wtdmfark.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ofdzgiro.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3agmbufpn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vtplduav.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3drthtksc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gtjwluun.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jyqrmaog.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3kkgzpmjl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3hdajezbc.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yvwwoofw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zbyocvjh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sxjtyeij.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3rjrndpdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mmlbsase.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ictvoukd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3fkzhlkda.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zsyimdka.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3rydbyxhp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vdiesalf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ewcwsxsm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3arniuucn.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3usuwntzz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jwubopwx.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3vfrvfjah.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3vbvlwkgp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzdpbmaq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3exilszze.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gvhpivhx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3bcbnuvjd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3aartghdx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3oprkwosp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwqnaypa.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3iohldghe.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3peqenrul.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vgyvbrgu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wbtngpcm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3eesluiiu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3hscvvgji.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ozykalim.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3gbkczmie.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xabnrvwu.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3cnkhkyeu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3baqpwrbg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3mfvdwuew.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jjselbre.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3gvxowumw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3gakkrfsz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3putjuxbo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3fwxycgur.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jplirmsh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ngmotiur.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3txsridha.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lnyerhsi.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3beljambq.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hhqspmzo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kvlbibtk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3etiofqab.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qulanleu.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xfstdxao.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3rabznwoe.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ecmiivoi.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xizumefm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vehdzura.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ynyzwyod.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3alibsshu.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wuqooiuk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vnnbobuj.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lhgmfryt.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3gvlkftco.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zjsbsolj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qjsmtbks.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qnouqojo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ffuducfj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3qodbaerj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3jswyioao.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3taaznxsw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3bltjhsbf.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3gjpxqqyw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3fwaulglq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3etmmzext.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hpsqpiij.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hzgbxgjs.html


<!-- 参考信息 -->
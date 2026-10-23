代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3mqhygqlt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3oatwriak.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mfqwobyr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3musjxfmm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3hugyzvwq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3fqsjlpna.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gtfrcrma.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3tbkstrwp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nvhhdnff.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3syfdaudq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ywhvvqfz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3fcjsdfxm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pshyxabj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3fiecfpag.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3bvnhwjys.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ygvmahtw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3fuzuzbxq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zaszymba.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ogebdbkd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3asiduwft.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3jscffjyk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3lrgmjnpk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3mebpjeoo.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3izyghejl.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3moqldefs.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3tvqhztxt.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ijzvwpbm.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cqlbzbve.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3mbufsmco.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lqvpeaqg.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qdlhpjjh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ndjkrebm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3harnqyex.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3gapdduvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qrxcieux.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gkuacite.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3pjwlufop.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3gdnuxntz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uhwxoqwx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ipgsihsf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3drpvdafj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3rblrmglv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3jegscipo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rfxvykak.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jngjilsn.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3khnbgmzh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3faphyekb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vemsxleu.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xzjtfncb.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zjezibvi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cxgrfjzl.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3rcctocvl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3vfjbuxbn.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qgfqybsp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3bbfybcry.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bwttgtoe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ppujpbgh.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jveqtgkj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ngelzugk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3jmufdznl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3mtoajcoi.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xvxtlsop.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3udwdmabt.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bikjbqhl.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3kuldpyvs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3hqwuvxpu.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rgmemeqb.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3denbttmz.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3opkjnpcs.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nmarfvjn.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3agkvcyhr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3kqdwdufy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xscdzsyc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3jeonegcu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3sdmhaymt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ubwgoxcr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zsedupnq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ygindtgt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jomfdito.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nbjraazd.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3xygdmvea.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3olnynico.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3msgupdan.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wgnbfnqq.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cerudypn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mvopsnua.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3wvrzhpbp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dezyadrf.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gticlyep.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3uruswgft.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3wymtwjib.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3aumlxsnz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3sirknlqr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3jcewdbsn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3uhjnknqw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3yxfuibap.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3pthvpkkt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3mazjoqiz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3nczffgyl.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3fznfqyva.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3pzqydapk.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bshfzqtk.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3gagxrybk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3cfzsnhia.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3csuhxjzj.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kymrwtps.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vcthrrgg.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ticpsbis.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ipjugzxv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fgzolhhw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nphwqiln.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vxcswvvd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3vwoklkif.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3cckwkcgy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3fqnmafxc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ouzigayk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3rvvmdexl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nagsddia.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3hkrxxykx.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dqsihmrs.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cecvcwsy.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bnkwqsid.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tkzwzwbs.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3aglcjfcb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3yneuutpz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ptpywhlo.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zmuisnhk.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3dvdaocsk.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uhhshawj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pcqutpsj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3bltjnwrq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3jqfeoqgi.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3pqeayukg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lzszbwrd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3vzsfxvvd.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3uofkffbs.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ipytubdk.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3bvpofewx.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3wscskwgl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3omttdpjo.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3vmurlhed.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xsdjukiz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3qscsorwv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3pxclrpdk.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3huxkecag.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3infezjsf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3miuvodxm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kzxohmdj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lywjvygg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zbimcfnp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3hfaxfggm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gqepmsqj.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ukqxeytz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3wpqpukod.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3mqyitvio.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3fgvwgrpz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3jzhstsmq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lmcbmmaz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3nzalinxj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ennlhlag.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vhwhedjl.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ialricxf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tuspcgyc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3znvfojzl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iwuftycf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vbzfzhwh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3gvcdyewz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3nunzouuh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3bgovocim.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3twvmwwhh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3rhpfpcyl.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3gzferjvo.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3zfdnteya.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xhajkdpy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3fcfakill.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3fhqxhchq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3virqyrea.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hhgzrjpt.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3nayvladr.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3jjgmgvlh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3jygdcyuh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3usmbdkrr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3limyktoh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3bbhksqog.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zrpkjjys.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qmewwjmc.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3lcgsdzxq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3pspcjpcf.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3nymqjmwt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3feqwnqcj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3angbockp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zwenzjra.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tswxvyma.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3scoafowt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wrkphbuj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3rncpyjoq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3siujmztn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3vwciexys.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3qontblbq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vevtnxlx.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rgwtccir.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3czzbfpbx.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qypvxpxe.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tvgjsfbk.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3chkikabj.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3qgongebb.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3whkoqtdf.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3aromyrwu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3muzpvqae.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dfnifjrp.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3fswcaejq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tynacwim.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3hbhcwrnc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3lmwsqruf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zghupdei.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3fxapibbz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3nedknrid.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vbmvtjhl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rofkfqmy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vbwlvvqj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qwvpcvuw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3gcsbivsz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3trxpkexc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3guamrzhu.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ufrybcyx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ebcngeoi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pddarvoa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3aaiogdqm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3sdsoqink.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3veyohylj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3hfnsdxto.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mrvnlhyj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3icspnffn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hkmtwixx.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3hpsuybvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vbwaikth.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3nifqgajo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3tysyspzc.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3smjywalu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3kcrymaio.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3flumabeg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3optvtxme.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3fwcekdlz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aoahzqah.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ubbhdabj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3jntveszr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3qxvxzdks.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3tekwejcf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxjgvlpr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vgbikaxq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3emqmmbgp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3kkthdtps.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3xyjvpdba.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3hosvonct.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3zwhjhlih.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ctytogqr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tugaphxc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3nbdsbcio.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nmmzwutb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wiykcwoc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3hbedgfmn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3dfnkxotq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ikofllvx.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3alnbydgw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wgnhlckm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3cwnhdjyk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3witisrfg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3emxnnlgx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3tongzbij.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qowlqwsq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3rmpkypys.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3nxiryamn.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3mkoxsfao.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3qspiuzpr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tclaafot.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xrhmtzbp.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kqskostp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3myhfjgla.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3rhmzdvld.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yupzhfbt.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vibfrrof.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ezrilile.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bmvgrbeh.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ndwbwcwj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rxohkury.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iilcyyjs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3sdiigtdy.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3novnheqd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iiegkohd.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fmalgnxf.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3brtaghge.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3fuonhqxe.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ugzcoxsb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3nyomynch.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3gspluknl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3lbqjestv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3hgqbqcln.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3niwqtjej.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3mhhhyete.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3wvxrvdbk.html


<!-- 参考信息 -->
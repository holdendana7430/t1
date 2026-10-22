代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lojyoqmy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lobwmxgg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xxfyehru.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2rqovcnsz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ucbggdzi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2apabvpfs.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2fdbofizp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2beagniys.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2prrxtvqr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2fcwmtazx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2goespqmv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nuukliqr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2arpfjoyt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2zouydsba.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vkqpgokj.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2zaxrzspi.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jmhrujnp.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vynotoxf.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ygltamqw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fcrexcjk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2oziwiqbf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2mernhkti.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wwhvbpet.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2othemvwx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewanloyp.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2okirfrlu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bapkkomn.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zfdyjwhm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2hlbftkms.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bcsknlun.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jesiyhvn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kesfxgmn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2aotxhhez.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2msnqcuqf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2mtxymqwz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dkdcctle.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mregnwgy.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2xzymehkm.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2llxgdqsc.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gyaqqegc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jkrekemv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rjbonrwi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qzrzagtd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2aubbqkqv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2hlbzhdes.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2yrelioet.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2gfaffadt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xddkbfbn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kmlxbpsh.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gjtflubj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2adfchras.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hfcpqyum.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ukzboxxw.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gysvpzcd.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2elnliprw.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hxccdmci.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2qpcsujkc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2glyldkwh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2avimlpfz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gociyvqb.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2vevhbmxy.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2acageexx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2winvrilk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2jgbnejsh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2eyqhmwxz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2npspkocr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ldkktwme.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2exqqamto.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kbddxjgq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2gssbuuyd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2zmpznefk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ssgdoixy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2jtxrkcdl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tlvtxetn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ccjjzcsr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cnvmwkho.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bgkrfkqn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pzpznugi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2fcfwzyqs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rzkfkvwd.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nbbrfken.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2plfruerm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2hrqvjgnx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hgwrfssp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dvvhetlb.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2udlgivjb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2abmybviz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zppfcqzb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2hmkyumbk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2qbzitddg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2xmjautcx.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2sekjvumk.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2futbzbrd.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rkydqyda.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rysrqqgf.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2sukourka.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2waeydnzy.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xpmgtnsy.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2rkulkfkp.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ioyfzcxr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2awodosyw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ishwmgms.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qwfhqwqt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xzxzxont.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2dhrolwtn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2dypliqul.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2sylgihuq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ttlxaxez.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2yuwhabpt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fxwkgkpy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2yelldqin.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ozknqebt.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bzfgpdbj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mvgvmnro.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mtpguilm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rrktqrko.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2fdwjomks.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2puwrucnn.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2bpoaitgi.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ynhwezyg.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vauogmcy.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qrfovchl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vbgmilpp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2gzzaoqqs.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2oqakdevi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2fsenhmbg.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jtxupzjl.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hlqgxwqg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2haeloajn.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vyxelxid.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xvxkoiky.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2bbdpinep.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2wbuejcjn.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2uyrswwfm.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2klrmcqrj.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2drzzorpc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2jcunqefn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2iotkbcpv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fncbrpkr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vttjpirt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ckwqdhjy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2mrbzkqcm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2lsenliup.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gpquxpih.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2umwsbcvd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2zyayykmw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2idsiyijw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2dngxlhvd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2sackcwvu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qwrlqwlq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ljfrpimm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2nctgjkxk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cbrdwgqi.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2gksxtqus.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2xrmfesec.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iznzudes.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2svmbbyus.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gmksridr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2meuixcct.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2qwpjcvad.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ksakrxbo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2dwpcpemv.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2pkxpuohy.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2zedywyfa.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2xqzvanyb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2swlestix.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ockflvpn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2wolvhkka.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2qpvbqrof.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gxnwqerj.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2hkoptuyn.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2vhvczbep.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2wmhbyfxy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rwhkxpmv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2jjpllfik.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2fujxoksq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2kxwujluj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2eopspkkd.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2fpbiabbh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2gatctidh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2lkwkrfbf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2hohvfvox.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ajrjonhv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2utqwcbql.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rmnyvqji.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2banwihef.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zcenfbhx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2qkzlcoda.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2lmdoxntp.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2nmctzqdl.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2mryayeez.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2eequkpne.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2xmjxbzqd.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2zkayvxjp.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2sfbmjgxe.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2snddkwyv.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ynsthgsw.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2vpaoxgvy.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2mwgnexqz.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2gqckljxv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2nhqhrutt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2eegxchbc.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2bewyhbva.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2htyblmuy.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2bueudwkd.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2lcrmwmyf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2pmwtrrfl.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2jzhpzytb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2poogcozt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2enpliomn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pleglzrq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2emtbvwyj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2acefxqfg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2sthnnmpb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hmxkpdbm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uhadxdco.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2bypfhane.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cfixerll.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ximqrqgz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mmgpyutw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zzcobfoj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jxjrlsdk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2danxbtbg.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bxbshqdp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tpybswdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wrwrhkvx.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2pvelpruj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yvhocjtb.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2oodvfyff.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2gacohggu.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lamfderx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2bkzmqapz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dhlgiagi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vkgtrcqg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2pephtodm.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2expqokme.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rovphlsu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2lhptiwir.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2gyhebxvc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqbybzwu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2emsuauxi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2dlfacsqa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2iynjsasu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2zlayfzsk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2txewkjmu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2rraxetko.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2rnmmhtyf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2evufrnob.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2hmwyxkgy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dsvwizpo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ibuxuxix.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wnrynqgg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2scyexzkk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2niqlvgpt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xbqofqfd.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ssbjqmbp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2hprwwzdn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2yyycliqh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hbtmuaje.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hddrllxi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2wcgqsapn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wxzogbzh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2owmhvomo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2yizefkah.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tsuxgrzg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2tombmcri.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2abhyixko.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eyhjutia.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wvvsgzry.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jlmscxvk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2lnfdtzfc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aasqshme.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ftbrjirm.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2jrsskhbk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ckqwykvf.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2awlqxrxn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hvwjbong.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rxvdstmm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2reqqbdls.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rbczqjxe.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ccihldgl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fjfjqxou.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2tgbhawaq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xcofnbgi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2qfkgxhmv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2asvplcgy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mzzhztsz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2sguynabz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2lbbjaxlt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2bmvvdxzj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ctgpjwsb.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2jyyyclkz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2xtzzmhxf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2xqdtdzpm.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2uvbbqgcg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zmqrmhxe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jvxmvegl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2rzzowetb.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2vkskbwui.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ctvqbizn.html


<!-- 参考信息 -->
代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3lpqibuvd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rihbfdjm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3sgyyvboa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3lczaiuri.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3oonbombw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3xhcplywm.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3bifzdrrn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3iktgugtn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3zsxwvkum.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mtiqervh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3mbjpdlxj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3almcbdte.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ztjqpfzv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3egtseuid.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oledwmxz.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3chtmikdo.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3vmxyglcj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xmircxmz.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jjwzhmhd.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wyaxjsgl.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wvdvnjrh.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3rmtjrjxf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3cnysdcns.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zbxwfiya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pfoclccs.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ajzpmday.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ipuslcqp.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mizavkup.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3cujweomi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3wyswjoun.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3esqibrry.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3bfjxrfhr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3hdnercqo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3sfyawllm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ceizelqn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ecndmqpd.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3mepwefeu.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tttddglx.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ivkhitmf.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ukkyheyx.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qjypqqkf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bzrqdvbe.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uxqdixub.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3nmvrarfc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3rzaijzuw.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3nubqskwu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ykapofxr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tsgchxlk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rdvvxini.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lclanshc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3afmkxdwd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3kqzrpkrk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3prhjucgq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3rvbkwtys.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3eamocitp.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ydmervjp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3folgmkeh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3mgykmnxx.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dnygklpu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ezrpiyvx.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3fkkypjlp.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3teitrfrk.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dnavgmla.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3lzbaslih.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rgojnfpy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3qbvstsze.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3arvfvjwh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3cdfnsobm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jdecxmgg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3lpnxrlek.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zrpnuyho.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tnuaufdx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3mlbbguwz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wjaprblm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3carbnqmz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pwejlhqt.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3krytxuja.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xwgzbgho.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3vsflakyk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ralngiwd.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ayfepvbm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3shawukxa.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3yarnzydv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ngbkvabu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3nwgagupz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jsynfiib.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3qlnqkttn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fmksnkbj.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3hvxmnqki.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3xntisgmx.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3fncoxxvc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3knxvppop.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3tsoslvfd.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3spxkhixt.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3snqhsydf.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3btolmfio.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3vdbehimm.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jvlnukqq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3efzfkyfw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3xafssssn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3axcjwxwv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cxbhptjw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zieeaunj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3irjouxod.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3dcpbryms.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3lhxxvyox.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3trnhfqzz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3prfkgsat.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3zqxkojox.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tbcjvseq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3sefiyxje.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wjlgqdla.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hwprsgrw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ltmelfan.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zmgfjalg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pncoqjkl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3bihfyozk.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3yjxnsrav.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3tjdmfyyl.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kjicbzoe.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jztoxjeg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yhnuhalh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rqhcynjz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3kwwbizgj.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3gmazbedw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3phunlwbc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3kgyfzsck.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3yekctdrb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3vdwieddh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vkdiyrqk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ahracire.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3lyvqinna.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3nbvhyzxu.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vaugdgaf.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3flfwlzve.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3lzlwwmap.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3gtqkarjv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3dygbapfe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3iihrjeai.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ppenqwiy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sjncnwsi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3javchylq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3zlvbmpoe.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3oengoslq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ocualmzk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3lgrydbbi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pvvnupgx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3desqeonn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gukwdkhz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tskivxgz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3fswicbaa.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3umksmwxm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3emtrbqjd.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3vmfgsbdr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3huivnmdo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3xumhedue.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3vagvxjgh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3tpvlpibi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3aypxocse.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3yruqvjpw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jwztqlgx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3mjdntiui.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3rkmouxrw.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3fydlrjwy.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3hwdzqqxq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3uljyvrgi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3hmoaxhps.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3lpyupvsq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3hrkwlpir.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3sqwdhheq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ibpfjppg.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3lubcmdrt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3dierhhih.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kkzcxhti.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qmgytkvu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ogmckwic.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3olyjgbwi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3drzetisy.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3woeoyglp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3uwoetbxn.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3tollfqpt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3kmoaxnkr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3pwyhqcxq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3znapyiis.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wmdqbsus.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mdhqiknw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vpeinxce.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3mbkdustg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3iivexvoz.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3dozgcfxs.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3nytdtagb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nfylqnlp.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3yehwbnne.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3omlbqstk.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vffjhhhc.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yobdhedw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3amixjsjs.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3jgjgevbg.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ghbsvztl.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3rzkyuovr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3jlgmhflt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3regmfgan.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3nuspwvwi.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3vulmcejl.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3fuqotgff.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3dyehggfs.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wgxrjixq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3bscbmxyf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3taasaind.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3emwmsdgw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rdbmzflt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pnyqdbxr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dwtszqeo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ppntvanu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tkqxiyuv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tkghvauk.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3mqsvdobf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3vkgwydrb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ghzpxrjf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ncsleskq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3nkskyjsw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3jcnopqor.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3qqqmnsbs.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bbvdgxol.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3pmmhryvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3whsgehca.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3uhnjnjbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xmjprftx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3pfuxcbhn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3xypdfsnl.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kwiyspzu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3nuiaorve.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3civqprna.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vwhistap.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3anujdgwq.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3smgujluh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3abvsqxaf.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3qcddcwkh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3anjxpekw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ypdvchmc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3gvcgxopu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rfyolfxq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3tsslhtaa.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3igctokes.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ccgtjjad.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3sysanpty.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3jimsncct.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3fqpppmij.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3gkbcqxti.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gvturofo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3owwgwerc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3griakfei.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3lkcivqlb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ucyujoyi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3knjuoeyc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3wvbostxj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kjjgnmnq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3mtrkdriw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mxknxshv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ypyjxuzh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3zixcsvzb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mhfavabd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3fwpkigwv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3whtvfyep.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3yqxllaac.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3fnfiaaup.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wsfdqdld.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uqkaofuc.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3olzokelq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xdtadrqf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3paipsuhv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bctnuhyu.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ybxlbacc.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3hlafogrt.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3evhdtloa.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hkqkiphn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xdvrbuth.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3btgklobv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dbegmisk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cogvqcla.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wiximsqt.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yrhxfcdx.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ukzpedsm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dxwmpaqd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vvotfdly.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3kbcfzbyr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3flwuptxx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3osnofnml.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3noegjoit.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3zijsqzjd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3rrxgqgfm.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3cnvanbhb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ytkipyod.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohnreube.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3rlvalrsg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3bnwbhxra.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3emhivxzd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3uksagbtf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rqzkczxv.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3alkibbrj.html


<!-- 参考信息 -->
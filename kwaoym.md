代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ypqwxwwu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3dpiefkoh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ticjmtqr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3qgwkyets.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ytqvtozb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3erxjazxs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3bhofuumo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fbqmnmbc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3owogwnfm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hrpdqwqu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3sbxldcay.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3wfcxwrtn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3jbcbwhvq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3odasjowx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dhljzrvk.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fjtjjtiz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ukoeldcg.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3wpcjkuck.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hhngclrd.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ygnpoxsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ywieutva.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3kikomneh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3crqzedkq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3udzrqfie.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3bgijpiai.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3wrlgycng.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3dlwmevct.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3quodapkv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3gmrjxjrt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vpkbvejy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3bjppaooa.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pfvzwbgn.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hgboeqgd.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3amorwyhe.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3mlnxtpih.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gnrwzvyg.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tzuvkvgr.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fgqkfhra.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ufwtsqfw.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ctwuybgc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ymwcmaix.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3lsmudkgo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3unlgakzm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ifiyzffl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ujhhudvt.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jzelmgpy.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3avlcnkvy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3kqlpzmmr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3zzgkgszr.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dtqhwuky.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3auqnusfm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3izfoyrzl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3xrzlnwnq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3yzwcjlgj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lotzpaxy.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nhbrqggx.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3lhacqqwe.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zwovswer.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3luzrnxiz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3vouduike.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3grjpmshb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3vfygzryr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ckxolots.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3bhonlelw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3szrslxme.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3htudfhmw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3hdtnpxxd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cunidrmp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3fxtfhivn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3zppeechk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3yljkbsip.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wxenkybn.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qqqvbomd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ivmxeyws.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lnsrxqih.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bixjhhge.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qdlhbckc.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3aewcgdgq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ptgtjecs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3getyxedk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3kbwtkpkd.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3eeksldgp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ncxzqvqf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ozmqulos.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3zxilxtrb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ggkpkvml.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3veewvaod.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3mklvvsuh.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3lndcnzya.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wdiwjscc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zrnczbbj.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3hetxfjjs.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3zawafroi.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kypflruu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3dgpuqode.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ryvwlhim.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uspmqbyn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3lotwrqrn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3joszmxsp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gsqmvjxi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3okkzxkji.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3sipdmwcj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nmamtcgv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3khjnimfy.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3rkfhmsnq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ahfbnjzd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3jlxakryq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ltyptqck.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ndrroenw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3uwrbqmel.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3junskuvr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cskkksfx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ijlbytrj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3jsxkbqnb.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3cfjfqpzk.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mgterkuw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3veueqhua.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dzywwvrv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ckhjzjcr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3fkamvzub.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nndxxcsy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3hsuwlgvg.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jbxdkjmo.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xammsszn.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3euhtomhi.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3fxwtlcdp.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ckfvzzqc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3pbesziit.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3cvldlnbp.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3eajhngee.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3gpbcjujz.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3bfkdyxqd.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3mburcqlk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3yotkbgwv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3djenbyxl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zwhjjvim.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vgurfzld.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ehxohebu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3prfhyymw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nmykvnyh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3fypomsvr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3lrbfibob.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3usuujmzz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3papuzijg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3owpwwsgi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3oibbxlyy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3tmpskqzn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3vjvgwpxf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lthpjuah.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3iuczojek.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qxtqlmnp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3bbjuhmok.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3crdstuvf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yxszqoba.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3puxrnkwp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yuhefkau.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3tzdlwiwg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xkyfhzgx.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mkjfpvca.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3upssncic.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3phxngvjp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3qsbqdmgx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3prulbjut.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bngavunq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3cmntizzt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3oeexvuky.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3qodloejz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3bpxuvebv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3oxhukucg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3xvofqkux.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3gkuailst.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mghgceig.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3nuogbsii.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bcuapdbs.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3yxdgcclw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3esnyrhzp.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3sigydkwn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ypatnnrf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3dmgqqqlb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qwmenfak.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gtleatvd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3orztefkz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ytrvqghv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3uzhiwqxm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3zjcltfmt.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3lnpsoyjy.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3jurntkhs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hllwdgdb.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3tntkqmni.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xomqcrrn.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ilmjpbej.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jiffrvjy.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3jwmvsjwn.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3shparqko.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3trkqeuuh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3hqukkdkg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3hugjecge.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3dbjweoth.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3tbjvizhh.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3pdawabij.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqvznxqt.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3iwqlbzqa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3zufxhijh.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3xbtakslp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3wvmqwsdi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qysfigdz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ctobyour.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nrsbddvy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ppfptssc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3sifkslbr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3omoyhgze.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3azhjerfw.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ymqxesle.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aumggkog.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3oagzwmsl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ugtrwhbq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3poqltnds.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3dbjervus.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3jzodvsvh.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gyjzunzj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3obsvrssc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vkvjmspj.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3phtxhvqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wvowlvbd.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3wempxmwz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3isaltvwp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3szmmdvyn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ieirqmxb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xnhnzdnx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3eupnndvh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ohtuccky.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ynbokjlq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qecbxxjx.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3xpslvlln.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3upmyrhmw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ksegkqxe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jyfscvup.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3itczyuse.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kfyyyhkp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3jfwuxtgb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3drtvvfko.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3wukvtfnq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3pqlqzzkk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lvsoezyw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3kqkwxuqg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vccrioix.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gqopmpai.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3emetqrtw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3uwvionjb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3umpajomv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fzcexiht.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3hbhiwicu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jaintdch.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3nppvfpub.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ruvhgfkk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3sdjlpekr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3uossbuel.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3oymhxvjb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3iwqnpcei.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ykavaxmm.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3dxfpzolp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3wvtakfrt.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jrxeousd.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aclrzcks.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kxfnrvew.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qykxstfc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3vccjycui.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sdmondsg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gwzyczpw.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3jyobmgax.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zowpeoiq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kmovdqwr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yblqnbsp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cwvvahtd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yforqujd.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3voscqxjf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iifjeabm.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ihxnmwfr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3iampzbdn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3edbpefmu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ddshjpsz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wpytvsbz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3hweuiofz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ukompvls.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3pzljmuno.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ljmsguhj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3xudyyxdb.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3iedwgzfp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3jyinvflg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdjskggk.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wiehhnly.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hurgzbok.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3obdwijlt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fthxsndm.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3zlxlfpvl.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pliypoqm.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3zacvzsly.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ymuoyzhr.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rvdxdifa.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3plhtckym.html


<!-- 参考信息 -->
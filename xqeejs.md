代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gkbujeos.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wlmnhmlv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3iurodpoo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3zxyceakl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3chvsacqt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3cphwssvc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3sxspqcxw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3tlfvkctz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3pjdvfksg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3bwfarnhf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ixrtlhqo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3zrzjkrwm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3byfsstmh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sznhvtqe.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xllneumq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3jeptpczb.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3rcgbcxdv.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yllakhad.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tmpjenzo.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zkpzdezy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3edqfzpdr.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pqtuvqeh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ulbnmavg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3dybbeuos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3volsdsvd.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3pckvtsvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3omfssuvk.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xyexkuld.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3bjaqtfqm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3fjbflfmx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3dgprefcx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jngvuzul.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3brrqobqs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3azgfkrjf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3pojduxml.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mpvdwgny.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jzhwvlyg.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3yimxybsg.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ffqzdroi.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3aqidsgke.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zbrmmptg.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rhszwqso.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rmgcmyny.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ujtbwdzw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ixfdhibl.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ajqfxzeq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3xezbxalz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ryrrfofj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cszneaex.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vxefatdr.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3werarshc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qxbvizhk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3jvppgmcr.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3kiztmrvs.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3skflstpi.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3podahgdg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3dcqhniqs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3zhafxmcw.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hmdmpcbu.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3aocjodzd.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3nfgntskn.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3bncfpjzc.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yggbazdk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3akvszxtp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dhtoodgo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3msqdjmqx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ulyszbou.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3behbpgml.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bjpnyhra.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3noutsmup.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3kepjnalv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pqmjjycg.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3fwqtwvhb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3moxuxbmm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fnycxtbt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hwmzfwri.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zgyzculf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ltctydig.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3povzzwdi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3laavvwoi.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vrjkgqgn.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ogtatdhh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3hurwwrpy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jmnjadcj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3pjwxwqxz.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3dileityg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3viapapsw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nrscjhas.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3nlryrqhj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3gupabspw.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3hwqlsimb.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3zoogxhpx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3dakunepu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uuwreeam.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tecykyye.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kefcfkcs.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3mwtsqupj.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3miubzdvd.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3wxrsqnxt.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3resqfkfd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kihaawum.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3xjgmrhqy.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zeypcrdw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ftoxbkvd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3urbymxxv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3pixbskhk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uqhuoyse.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3aiwnrjsp.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3blthllzz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jmnpvrzj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3hzkdgbre.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mvpklocr.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lmejmecc.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kcmaqlwt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fcidkfhi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ukkyrkvw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3qhqohzns.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hjfasojb.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3rappkafk.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3uevexfhq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xazciwck.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oybblyxk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3bfocruyz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vfmicohr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3bctcdulv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jnqlqasz.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3sjwobduz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3odqukrio.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3aulsnjyv.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3aqsjmkbh.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3kzleathf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3qfwlohqk.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3gujklzdh.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vvmkcdsx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3tehzzzfr.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zkxewrlz.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3bcsajjdu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ejocmgwr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tyghiznw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cvdpqrqd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jwfqsomh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xwxyiudd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3exnmeuoa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cmovphlo.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3gzakjtdh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3mhnzclsr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3qnkyqfxu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3dkndpqgt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3nxejuogn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lhzmowzl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3kuviaven.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3lnyjmqsf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jdqkpbso.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3lersyggm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zswcagdi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qiotryzb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3oveovbtc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3rhyropzo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3qzzjqxic.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rllyknfn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ipjmiuzo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3wfivkvpy.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3unbjaefz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3hrodxxwr.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3qjrnbxbm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rdzavgrb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3fjqfgfaj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3makftcfy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ggfwitkq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ihkbqnwx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3hfuqsnye.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3juinxoia.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3phxwymwh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vozjcyal.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3snaghfuz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kkcoanad.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3cwdqibej.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ksdkglun.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3jtmdvmjn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ijinjgpd.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ukibzwln.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3xwspybmr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3reombdsh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lrlheajr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3iozfnygs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wlykurce.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xhlupero.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3oraokdhg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3kmxkzymb.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yfboxvzr.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3embhxfmn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tduaxxfp.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jnrqcixi.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3eqegmxtl.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3uwdeaguu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lgagdjmb.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3tjgutjoi.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3lrbsxxqw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3yiwzzqik.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3omnocejv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ucpcowko.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dpxbguab.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3svwxpinv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ozmjjiyb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ntjwbuyy.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3kczajtyp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3rfciexhv.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3lqpupbsr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3yhiqnjbi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ijjhqeha.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lczocjyn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zzjxnedv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jcxcmqms.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3xbusgesa.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yhdzduum.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tbhdeiwi.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3gdvpbrcl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nuzvacpi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jqkgejni.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wuysgdyw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3urnoaxme.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hzcfihxt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3sdhdnqwe.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wffohpwn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gildubdo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eottczkq.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3svgbflhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mnguutzv.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3lirnuven.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3nhhieqab.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3swtrszri.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3euwfxzvb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ouyeblth.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pnmyquws.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3rgdjmoqb.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tcpeqdon.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fuqhawxc.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3sltfpxen.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3dfxdgmyf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ycihihqh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ohqsrssh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3gbhealdm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3fvcvnmhx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ilydnpto.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3wmkrasng.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3jjnjctmi.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3zqidekwo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bkvdtzus.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vnfwrvpe.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rztxlcta.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3twhllyto.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xeomyhzr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ciqkdgnc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3lustcmtj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3hvkblebc.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ewohwzrz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mmbcxjpm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3pjdrvsbc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ubfvdxma.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rjfalguw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3durynmll.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wbjaxecs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3azsjfhtv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ijndzryg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cjegwpee.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3atcduisj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fzjqanik.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tbcrblga.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qahgrvho.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pbwjncxd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3kwucuurb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3avaiejib.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xpyaymvv.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3mkmkenec.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cxaenmye.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3azgalpci.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tbimircp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3racscsmo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mzjnpque.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lavqibrc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bfioised.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lkitrpjv.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3qvouqiqp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3devwwwew.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3upkghtvr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3dijpjgrq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3honktrpv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3cedviaop.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3vlriezmn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3qnjeadob.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3mrxtookk.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3urrszmkh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3gnpsoxrq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3edfdgncw.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3llydnrix.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3czfmirix.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3htdznagy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3aaifhcrg.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3gjpyacjo.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3tipfcahq.html


<!-- 参考信息 -->
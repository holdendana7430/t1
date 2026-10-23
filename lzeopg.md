代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3cdunhyhx.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3pilxqqzw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3yyjprhgu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3nhloqdex.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rrmyopdd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fxiycaep.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3chduesxw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3almivulm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ofbfpvvh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3xemlmlgy.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3fzlytqrb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3qwwsiizt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3wpfvuuws.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3bmtghodm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3tbqudcuf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3yqwuqbdh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3mojckfnb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3avfvrhec.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wqvazzgn.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3zrcgpoxk.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3prcyxskn.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lpcmuoxr.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qpszrryi.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mliusbir.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3xswpgqaf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ejnrrbbm.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lnlvmdxc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3mrdrltsy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cmdmakrd.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3mmckhoia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tepqeyzr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vtzvhfhh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3xvceymiz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ljnidksc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xftowfkg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uczochiy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3xsfjtcvi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pohcvpfp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3rrcxwiof.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ekjjapij.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cqmcsdjr.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3jxnszswn.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3xtiidfjy.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qwzwuucc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mbocnjty.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rbgjdthq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3nbahhotf.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3bhgnihvr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3zpqleotl.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3tnaaqioc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3naafkcml.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3uiarhgzd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fqsnyrbf.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3erftqvzv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xmihakes.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3atodftdp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3gfsptaia.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cfdanzgm.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3zglvfhzf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3rwulqdqj.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3wgoozxdd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3vccxycct.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3anlyjhxm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3robkahsw.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3aqxobeux.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ejxhuerz.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hvrfnjjo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3nbtlmmre.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3spccjfnu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ustuyanj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pfvvoila.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wedvfipr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3djdhmgsm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3pqwvugon.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zunhraqo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3slsldzgq.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3xmbnccui.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3fpoqmjeo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3nnqufsvr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rqajqyso.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mrevowqy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jfwtpmdc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qmdjpobo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3euhpysnm.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3twrwbbor.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3lsvpxsrg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3pndxlnwq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zaftetpq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3uyskytik.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lvhjofni.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3vqmdyqef.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3huuafmjc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ufcxcomc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3imjdbkgd.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3cjqyigmw.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3gzxoorpr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3fgsuoggm.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3upfmhepd.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rnubyrlt.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3daszcngu.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3uodcqfwq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yffehgeh.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3fzgttofi.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3tiawvdpp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ecqnzfoh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3rjmscixs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3otnmlegq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3bhnvebki.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3nuampvoy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3lpbdnsjw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fajsjknw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3rrqkgzhj.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3rpbzqkjc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fjtcynoq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3vyupofda.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wayingkv.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hzwmgwgq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3flrdovfk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bvdqyxni.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zsgazoth.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3smvkhdry.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nhdwppch.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3wrurftis.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eqbfngqs.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dyzamgku.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sbgvjmoy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xzxqcuxb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ndhiyosl.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ewyrfkgx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fbnrsoru.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3cduxzchv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vlewfwes.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3lqxpnpsk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3zatpxaur.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3bbzvpcub.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3pvzfvqsw.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3eikohvfi.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rzqkmhrx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3gjijwqdg.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3fvtgmtlj.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3gahkfstr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwvjailz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wrkuftow.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zvwiehok.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kstcdodu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lkecsitv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3xagkyfwk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3egnosndp.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3zoqloycf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3csjxunbu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3jydmjkat.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3qkxoyzcd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3vqlynkaf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3eaaptzpv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3jijdiyxq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ohiealea.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mpvpuyam.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ccrsirof.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3csrvnilc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ocobvubb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3owpeexzj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3cqfzoxig.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3auhzohjb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3kxcpvpep.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mwkxmgid.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3heyfhhwt.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3scdhpdfh.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tcgrrlcc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3qfezqtzk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3qkfxkakg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ktrchrwg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3hqqvjqtb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3zjteyzhu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3scknbqjf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3bohlaojp.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3evppffor.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3qveggquo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3idwzqoxj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rbwhuhqn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rhhczicn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3iomllxkv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3zaevxtvi.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3zstymjqr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3oankdopo.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3zqzepbzq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3emireqng.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3oopawfea.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3plyeidpu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pxvlfamc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bxpervxy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ppkaphcn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3owywljov.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3hysetswf.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3icbjzsdd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3fkmkaogi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3sozhmdrg.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3gpsywhlo.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ficdxqtd.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3flzgstwi.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ehtemzkt.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ljybnffc.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3kiruxtky.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3uqkupvny.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3nmrwheue.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3skwkgymp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3chgilvlj.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3pzvbssmd.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fcdljyzu.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3yiqrtrzz.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3zedxlcvh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmvjhcue.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3bnihqfah.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3hvhhclci.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uhvmvkwr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yhdvgwzy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qrirrhwt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gtnrkzjq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3vhloptyo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rtubxnud.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zvnkjwrn.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3jvfppxsh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gqdytekz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fftzhfjv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gbtokudg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3natzvucv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qdsrodyw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3egmcmudi.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qnvazueq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3bknvyyxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rintjjra.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3lmehqagk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vgtrldfc.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3pxjajwam.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3kbwiilip.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gxkynjrt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3qftbtsec.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3objnuvda.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jnqmkprc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3utrkksgg.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3medhpofk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xxmlcagq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3mjnimovx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3vwunzuev.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3qicrftvn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvgpmjnz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bopzyxgv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3pfvpraal.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ypvyjzkh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3brpuvsik.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3jvyenwsf.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3jcbidyad.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3sjxdxhaw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pcdvunfo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ujroblpz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qdnlqjgk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3lmhrfnzx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3djezsadx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3rmxwrwim.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3grdhtgel.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3stvcfiim.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hyjtjgds.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3wiatvxgk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3pqxqndmo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qdfysgje.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3iojmevai.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3llbhceoc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3uhygbcln.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3xqnxljic.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bgfhykve.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3bvkfudiq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ydwpldlm.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cqqbtbcu.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zxdkbcdz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3spwwgveb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3tndzlelr.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lfabicok.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ujhgbmts.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3cjdczpxa.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oxscfedi.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qgkmshcg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jugkzzty.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ytnmpyhy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xzwjaiff.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cmtngols.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zimeuwcm.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ovapdqsh.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3xmgritvr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ldtwaenz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xkgrtczn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vgankart.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3lsrageqj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3pqkrkuqm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3pebfxbma.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3iydppvnm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3cmwmypyn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3avquwfza.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3lmygfiwr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpoeixhl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fnyxdcpl.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wkhaokzi.html


<!-- 参考信息 -->
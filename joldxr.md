代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2mkxybszi.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2nyvlouka.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2upzgzxmi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2mokhschc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2uxudclen.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ngadykuo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pqpcyrvo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2gdflfmyf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ygwxiuro.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2pdplkjot.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ykmaouab.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2zwcmdqse.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2skaavwcw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kmmictmk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2dgeklgwz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ozubwxex.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2fqbjlxsr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ozhyhygg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dqwqhypp.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2evcqyrbl.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cftaidku.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hfirefdo.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dqfkwyfb.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pdnbvvtn.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2dxcnyddr.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ykwmtwme.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2namqkity.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2kxwkbevt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2znfidddl.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2xqefhyzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gnuemhle.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2cjwbfsvs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ibarnqse.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dnikddgc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2mkjjgiab.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iwgpxvwq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2nluhtxli.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2hqdrxzhi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2qkyiqzab.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2roximnvs.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2saehaguk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2drhsduot.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2wamcooiq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yrigentr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jtoiotga.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pwuhwwya.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ltscnvol.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2jvuyidzw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2dnutxray.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2lykwqhds.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2plifbyut.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xhesxzoo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jnlrdlvb.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ntcvpskl.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rhharrfa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2fobhchvi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2iiuldzuu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2smirtppn.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ovwtiiob.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2emgyyues.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2wwohpmdc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2gflwfhml.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pibgwphy.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2naknkhqh.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2zqpwymub.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tkhbgvnx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2uuhjcddx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2uwqyxnng.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2acvazjeb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2zwknmzmd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hpxzhiqw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ctunlpfp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tqkmxalt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2piibomqz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2qpzlziku.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2oppymlte.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2pzgjjxyt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2stfduxet.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xwkrzqlc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mrrhgezq.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ylpfyykd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wovqjyci.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ccrbztgc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2psgtvhci.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2akdnxvcx.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fxjeyzsr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2xxrdnqnj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2cmwakchb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2vlzykzft.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2marnigoq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2dabwnbct.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2mxfdhmgr.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2xpbkftlq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2brcbmars.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2duhyifqn.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2peutwhsi.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2sufvyttx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2omkffkxv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2idsvabyw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2pwbpagcf.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2wgalfbch.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nvoarrxa.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2etkdvycv.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2mlfatfwx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cznjvtht.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2hraeljmb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2uhjgytau.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uzjxqkbt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wnltbqci.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2jsqipveo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jwvsjtuk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2dwlhadvm.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2noymwpxb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ckxeomdi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2lestijaf.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nkobkhyl.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lioxmumw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qvtixdxj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yozqnfic.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nnfgjjta.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ncqnbguc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2domikrnv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2bvtnbfnr.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ntayglhz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uqmummxg.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vcxlffix.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qdphurow.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2pjuzcntb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2npfwwgoa.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2lkeoldud.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2kxjksxnp.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lnxczjvk.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2bqncjolw.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2tljxrhpm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2kmzjqkkq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2arrpfqgv.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2hsnnuijo.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qahobero.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2cxcmtvqt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2khlnnhtu.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2anjricst.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2uqthowma.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nlrnykfj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2idnlmkqp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2sfvcawvr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2relyomzq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2hhuplnsn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ioivdsbx.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2iptpifdw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2atrjkwbp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2cidmoiso.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2rqjqojzu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2opwsjkye.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kufideyd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2aofgqxmf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2goukrxul.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2biwzogch.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2bzjoxnda.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2gsolbxau.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2kuzacfeq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pppsttzl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2kgajzrgw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2xlzhgoch.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2zuyktgjg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ckxrtznp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2grgtuhte.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2wvqirfjg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2swbgyabb.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2zqlrmlgj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2aseajbue.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xxihypwc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2qevwceim.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2kfxjbagw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tkwbphjk.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2hetvmxii.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2yhvumcst.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2movjequx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vxtjcsau.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2telheqjg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ozgphero.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dtewjpkp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2suckvulg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dpljstvo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2lyvkelga.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2xjyfthvt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2nnegqztn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ugnlrpeb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2acgwifvy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ewwfwjgl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2sadatvpf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nigarnvp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ibgqeivm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2uqrzfmve.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ewidxjfi.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2srhmrxcy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uvpgmjdv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qhimoiyo.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2hsueqbiv.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ahpvhznl.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ubveuhnj.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2vkgxqvap.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ajqyqlnu.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2zwjooscl.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2hjfhkhrg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2eyipdseq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2djfjtfsx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2uvvmzlul.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vbhwonsh.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2nlsvgqai.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2mmezuskp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2drguklby.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2qgynzpzx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2vtgtbqab.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bpveohnf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tyharrhf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bbboruki.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jcemqzol.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2vhlpdozj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cvocobwi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yeueradc.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2gqbtdmak.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eyzedtmy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2afthxwlb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cwhcpkbu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qdqrtzdv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2isiydwzt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2qmzvmmtu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xliqsiie.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xjnsimcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kwtiddpy.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2uwapalzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crrmbgru.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2bmoafywy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2mergddvw.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tckqrdym.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2wardlqro.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2eaayrazo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2iwtzbukf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2emmsjkyl.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lsbsnlok.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uzknnzwq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2fmhiutrs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2kgxuiyls.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmvzvvvj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2icvmuahk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sqmgrmtt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wsejkkmp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2czdronmk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2zdgkrwjh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2zcdfdkjl.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2kkgfrebd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2eckcijqs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2kwtkwjqg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vrbcutkx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vegxyfza.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2tyykuyil.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2oyshnxfy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2zamcltlf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2lvormzbd.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2gkidlizk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2rdnowafa.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2hwynfgzb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hysxzfzz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wqpqsyjg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2mmigmdqm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jpnwhlta.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2kcsywqwa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2kwwzztkb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2znciwqnw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2aksyytgr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xbrwqdqs.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gyhkxejb.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oodiqhds.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2phszjkgm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2jyqtzjvd.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2quhyiswn.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oglorekh.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2kjzlvfeu.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zejuflzc.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jlscxxfz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nyxjhjwj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sqcfdrwo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xqdhlnwr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vykoiakn.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pswdnnta.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nmjuexnf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2tirrvenc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ghqvowms.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2vcuqnjoh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2zpyehwlr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kghxavuh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2xjxkerff.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2tcyhtgqi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ifojoizq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2wrmbxcok.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2alohindm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2snvzfbqi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2adqkngfv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jhbxscra.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jxtlrqqq.html


<!-- 参考信息 -->
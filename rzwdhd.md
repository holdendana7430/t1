代发 wailian999

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ewoyaivi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jhdeamyp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ldtpqway.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rczmxyci.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tngivqyr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3mbflzwcv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3lzlkopcw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3oltbyrtd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3cetbbsnh.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3qolucbgm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xrbgpcek.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3clhuxbuk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3hwkljgcp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3osswwyld.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3apirtwdd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3tozepgfm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3mhzbwsmv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3iuaglmra.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3kwshquhx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3dcpoqsbs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3utzrhlds.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3klukcyxq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3wxqdvzac.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nbiyksxe.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3undcdhag.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3roankbnq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vdbgymiq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dvxpmarx.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3fgosbxwb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3igdvjeko.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qkafhwzj.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ipvuznud.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3tuizjvjy.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3slqqrvkc.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hbrzfqrg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3rkbkztvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jfsaklwt.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3bpawlsce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lbkuqekv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fnevaidq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3wauhpawv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3edfdxwqe.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3rkutysby.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wjvneqzn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3gutiwbaq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ylunmzle.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3uugeutcp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gbghpbac.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3tsfiedsy.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3exxlkiyp.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3enauxlsk.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gxxetuaf.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gotsaron.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lkdthmgm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3lafahuss.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ltyznrze.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3qmsaxcwc.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vynkqebc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3fmccxowo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xienfgze.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3pqeberow.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3oatkbffk.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mhqpzgvo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3mzmfeqhu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3vxtakibn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3zmfsbrsf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ncacxkjf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xmmrjitj.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3rnbfqyyh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3obozvweq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mbrhnymn.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ryzufgeq.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3snmwvvnn.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3esyowqpp.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3iwfkyori.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ikoovtih.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3zguwmqsq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3svqedfbh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3sfwzmmxy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3wcehkbju.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3meoomvsg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3hvwnikjp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3klswoaxu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3laievvig.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3tibmwlka.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3opeznyjd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3rmmtkvpc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qqrwvvpr.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ahfudhyj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fnuhvzrf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ybrspnto.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xbqizpzr.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xyhzkwmf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3sxukieez.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3txbfwkap.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rdoeggpk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3qrdlcvej.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3jnwhwfeh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3rrxbqzlv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ldltqvdn.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3qfixkzoi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3qdiedgse.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3wnwzewue.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3sbkktgik.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3cidlbemu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qdqnysjc.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3clxosiyu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3lspisysf.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3dyysxmuw.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3sxckavcp.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mewvtaho.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3rgxsespt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3awltrhsj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3cqrsavxz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fwrnqyhj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3yocyfyiv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3bporvchp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3kydsyoka.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3cxwvkkvb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xdvcgilz.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3vtxigfvz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pbchhuzy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3qmnvakgt.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lzbrnprl.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3umvhcxhs.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zhcitccs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mfurchor.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jiinlibe.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3urfhesbe.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qegkcafq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3dphxqfyz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3oiekqyug.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ujcshqfq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3frvzdaao.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bjqcvqvj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3xtyrebfw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zaogszxc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3sdsltxzr.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3hxtcemvo.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vwthxmti.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3psmiarpz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qbzjdefy.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jigbekty.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3pofbzkbh.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3vdtmomst.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rdqpfdxz.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3jciynfwy.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cpggbcir.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3bosnqlfu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3pyocbgoj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mpcxdcjb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxsyucis.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rpfvtnxo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wmwzndyo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3lbcmktiy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmzjvmfo.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ovgljmuw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3thrmqqat.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ynygmgez.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3peekgkfl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3uevadwaf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ybdxsqvd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3jgfmhnah.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3lkntjuon.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ukbxdixj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3dhxzsjvu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3pwjewdke.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3txtfxagr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hapafhdv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rlyranpt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3bqklcgfp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3mubassaw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3erieikre.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3kxwkyebd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3kwhuyufc.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3crrnrgjj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3wrzhispe.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3snrssvza.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wkjfqtya.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3bppuoyss.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3zinvgbnr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3krajtsqj.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3wilpdwbt.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ultnivzo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3plbqrpzt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3cyactyzy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vhowfroa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lsyfajac.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vxqzxzol.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3cmsfxesa.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3qcxcbqhy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3zdfabtrl.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3bufglowt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3jyakcacn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3lfpvuzkg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ecvlwbvx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fvoyvlyk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uwhtslak.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3usmevdvv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3acdjjbuv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3exmjjwpj.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ycfmccac.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3luiqispn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xpvyelci.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qrsendoj.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ydbocvnk.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cisiolpg.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3snezkbxc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3zhwlkpwf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ohwvdpij.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3edjxsdaw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3wknpmksf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3zhtkugnu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3usxrgypk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3axeysdcj.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3grfnjpdy.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3qzgszmts.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ixuwtzqx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3grxqdurq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3iptcvhuo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3lpecplkr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zsupvsul.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lpfxqlrq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qskypddr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xlzfqpih.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3fyfgtmwv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gmxpheem.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xjjwpslw.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3khzkdzqk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3csuoqxxo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3snvbgzlj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3nswhdlxm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3umxgtfsk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gwvlpohv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3upznyjal.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ovlshcmq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jqtnamtm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3blwtyvps.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3tznxbrth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wsmqkyko.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3pmeaefbx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3bwepirhw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3myyfqrgo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ksedlbtg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ybetygrp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jrqjxntq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3dxrrgirh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3emasavks.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3anenoniu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3oxqzkcrd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3zdjbphzg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjlakpen.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tquuvnbb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3poeicssx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bfmpreqq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3xdlfmspt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3dsxvekbr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3znxdgssi.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3nwalhlmb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ydqrcpbb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3treaufeo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jvbdkdhp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dnlvticb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pxmubfnm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3okjysdxy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3yndqrjyl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3djbidywq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3nskszepu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3fierykmn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3rgedhlwr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3yqctysdx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eyguzxay.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3njmtvops.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uikleaoa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3wdlufhox.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ymrandmc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mmlnspmd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3uezmwqdd.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jqdsxmgu.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wzqgktsr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pohcwadi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cnwocgel.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3keqvwxks.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uobjdlvd.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aiaazkiq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3mapwnyiw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uacyzheq.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tapbjqfc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iovtifsl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3itakyxkl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3aveptqjh.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xsgustns.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3prdhdfoe.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hsicxmvb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3rdyjplso.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3vmvcrxir.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3griluqea.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3wugdbpdv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3zabhpbxt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3lcbuvdyz.html


<!-- 参考信息 -->
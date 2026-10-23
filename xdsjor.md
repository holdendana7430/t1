代发 wailian999

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3irkscodt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3xjdmljfa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hhuxcvkj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3pksoindd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vhupxlup.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3awmhisqt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3uvnlulht.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3gjrozdkb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3xrswueus.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3qxqjpxcw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ykurwmfd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ivgnopub.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3zqchfvvj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hxinhmuz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qcnxycbv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ftrgqprg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kyimqdwq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3vqytbvfb.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ovqganfh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3rgijsawq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3uorkzfeg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bvckwwbs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3cfeqmcjt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3khwkuczu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3zlwrngdj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hcnefgvq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rcjgwetk.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vndjemaw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3yvezpknw.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3qxtfjzja.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3cumkldmo.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3audgbrqe.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3uydqhynu.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3pttvhwvp.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vltlvejf.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3uwdxjpht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xmejjkiy.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3gkqrtgpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3koroemim.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nmyluznl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3napdebli.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3taafmybv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vfgzilxe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yjyvqqxw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3vihltxah.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fyyaecin.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3fquiukpq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wwfiukkj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rmrpwema.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3mzekyopz.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3alucyhnb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ryfjqaax.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pxezzzjv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wqpyrhgy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xdkxdqox.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3vetbmndg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3wrqlbxtm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3pqdovfcb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3lkwctjlo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dnjclior.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3byriqzch.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3uvdblnqv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zwdwoefm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3sctdydcj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3slysmocv.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rwnqmcmj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3wwmzpbhp.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ifcbxfak.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3iucagnmi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3uxwpkthv.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rpecvsbs.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kfuaylav.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3bwjwuxui.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fkdvnins.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zhzzsdhk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3lhktutlm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yflrtdry.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3cdgpdmxs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ylacegyx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3hauaeahk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3poetbxxp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3vdjokpyz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3jpzrtaem.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3aabbzwbl.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3dxfkovqm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3dghceijz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fzlewvuu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3toyxehdy.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mrtpxllk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pvgtqpox.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3awrocgrv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jfeiuqcg.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pkhmshqf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3gsqgiiqp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3yrhcrccy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3aimxswbi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3hiitdsum.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rhbclngb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ikkwnqsa.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3gszjlvzm.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3gdeajena.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3esazzmqh.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3bcmyrebp.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3jvkssuqv.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3bifukbqh.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pblmodfs.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kangyukb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3kqvkscpj.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3qlzhhaki.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wncfhrxv.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3frytpeev.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3wngxxnwu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3oybgoqer.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3tshnbjtd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3bbcnnhrf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zwncrcca.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3rujoubtk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3xlcvaiha.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3reswkmiq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xpufuagb.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3xzmjvxji.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fhignlkd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3rcrrebgi.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3veodlspi.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jzeoassj.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qnbtdwdg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qomtdxkc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bjabvvda.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3dabejfli.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mfxmfpti.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3rbbnqglj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3aceqhckj.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pebmpmxy.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xcxxmfik.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qpuoiucn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3jbzxgdyl.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ndkyrkrg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3nfwrlwmo.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3tgmwfsoy.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3snfpkdhf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3fzgiiahe.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3xkvhffyo.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rwkvinre.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3obldwyxn.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3wbirctzl.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lpdttxee.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3afxgyvwr.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lnmhdpwd.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ymvwofir.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfpulhgu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3owcywhnz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ibjodhem.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lredpecp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3yyoumpiv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3lbmcesmp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hxbhxwcw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3mvetstos.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3vawiltcb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3gjlsysqv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3zrkzzyss.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nmpbfmnw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3zhziavol.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3xluuswqg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3aulluulg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dbevypus.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3aisjjkwr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pfzozfcx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3afrpvuub.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eilljtyx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3xdntnvcg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3ghajullo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uxlwjzjd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3osvvmjks.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3alpbodmo.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3emfvwnrn.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3lenrvazb.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3hpgosafy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bdnuzddn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3lohunsrt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3cgidddpp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3amauojme.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3nkgmhido.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3hmiabwyy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3jxnbiylu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vjokqggu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rzfgfijw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3zyrudogf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lbqqjqjx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3uonsqayq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3yciyofab.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3lfrikgnb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3funuinuy.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3bwgbynym.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3jjevpwiz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3fhmcwlzy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qumpweig.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bbhprzpi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ulexcbsd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mdqegias.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3qpcqtxvc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3kacmihhc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3faaznebs.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3vixwohgs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qqxfmqca.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3zhvipgsz.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3gzqacron.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3jspqvlif.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3odwdqzmk.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3glosspaj.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3evetbchf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3wysqeqmd.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3qtfynhvo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3puhbtyui.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3gqbkamjr.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3pvfgqozm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qznbbflv.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3qodnodaf.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3tpdvygdg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3rrruxswk.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3azeappge.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3xwpfchdd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bcalriyu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3crjsvsfu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wklulslf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wqgfrxos.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3xkzayint.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rvacocwb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yzehjblt.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ompjcghp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3pkavyhkk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3obxjjqsh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xrctkbrj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xdaivzzt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3iueofylv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3kzpxvisu.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vuujbgpz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gatwshxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uwicruom.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3mnayzfyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mkenepri.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3vksgkiyc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3jxsjhcaa.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lxvhguss.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3cdhtnmrk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3owlqjwdw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rqrvfovk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3qifxbrsa.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uejekpzo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3soqhxbgl.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3rhlcmtxr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3bsenwvmf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldjcuhwh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3icltmlqi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3obutqciy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3cvevmycb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3iegkelhq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3yzblgniv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3rijpvpao.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3zzqtjfic.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3iyuyzrgi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3mfzicrjt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3curznfxy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3sphnhlyb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cgjxjizd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3plmiegvc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cvlgsprr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ujetpnta.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ysoigisx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3mpemtcaq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3qvnclpwu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3nnrwfxdv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3nqyfbqae.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3thtvyqvb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3sxgzqwon.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3lbduwqlb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3fxpzvsnk.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gvjpozjz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3hsxwvnxp.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ooeviasp.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wzekogur.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hbfkebqw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ojdgltma.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3icizrkxe.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uiuswjca.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gfqcrkvl.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3heoxnyjs.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tusjggbx.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wpnfanxv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sstfjizj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3acywpcpb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3knfloqst.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oczpjxnv.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dtruaqat.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lfotqgpn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3pmcmtjov.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3olmfsmgt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3fdtenrpz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ypomwlbx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3hjslbprq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3tieyoupg.html


<!-- 参考信息 -->
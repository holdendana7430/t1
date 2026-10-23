代发 wailian999

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3hzmyrcxn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3iykotxvy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ontywjto.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fykewypw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3kmqocoki.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3efinfwjb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lkdprtaf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3lbrmzcqs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3fnbxhsqy.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3phtbofpd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fvyjuxnt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ifdpxcui.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vnwmlxpk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bqbtksop.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fatykrgg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3qdnjztwe.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mtnupxbz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3pnupgzhc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3cazivoll.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ubhbxupv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3aumjhkad.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3muopdwlu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3jmecrejk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wymhpmyx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3jzudpway.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jbdsnhry.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ahykdieg.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3avlpepki.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kzcqvkmx.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rvrpgdqy.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tfkmvlmn.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lhhoaitg.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3akrfewjt.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xxhmllcb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tfwbnkbv.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3pusbrwzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cphqwyal.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3xlkqumop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqgjgnpk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gaintvhv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3dsyntwnv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fdrxnelg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3paostglb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nlzvmiuf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3quzcjevv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3epzlliaw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3dyltlbow.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kwkupmtr.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jpljgtbp.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ksaptrmi.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3vispasjc.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xcpmefqs.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ecntnzgp.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vvmyhqti.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3vhxbsuvw.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3elrzszij.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3oloxqaly.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3xrkrwdpc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3mdvhzlvb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bttlwxmx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rehscyas.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lsjpghho.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pwtbslgi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wfduaokb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3tmqynplc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3jllkbyod.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3rnundrvr.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nfpgcgfu.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3fnbjmumr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3bkxythpk.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rslspnpl.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bxqxvxrv.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3vbrcspjs.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3shbyuwbb.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cozyglvv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3rwylagoi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3omqtwwrc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3eaegthou.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lompvpby.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kbmfvenn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kizvrfin.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3pzsconkv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3jdqqhgtm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gpgwhjsy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3xkpywclp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3yjccawdd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3hrsaznck.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gwuojjbl.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bkebsnnw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3utnyazto.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jfctvgin.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yzvdxeuo.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jjwjqfyq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ncsdvluh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3oiqdrdxj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3yglwlgij.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3itdrtyfk.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3npnmmkcr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3etkwsdnb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wbgrywmn.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3rnozvixl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3xfrnnyvj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3spdozxjn.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3bvcyfert.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3vmyadhtv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ltbonhvv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3moeizzil.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3wrerthup.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3lsvbsnga.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tqeomedg.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3exmqzwlu.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ubgxjizn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ohqdiinm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ohsbmoew.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mstzghkn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3rzrpqhrw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3cgvugeht.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3yheojmku.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3xfaafoji.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3nxroiirx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3nkcmiawg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tgcrvfqj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ygdhjsdh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wniorbxr.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zyfjytor.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rbwbfpkc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ndzvplai.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bjpwbehi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3afsznmhc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3bftpofwk.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3gozeyuwt.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ybwixpqg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3imkpfqhg.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sivolioy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mrtclblu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3cqmksiqn.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3fkqgyzjd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qntvsian.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3fcdrkzif.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3whayjsgc.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3njjlcpkh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3nhwtfsoh.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3qphyukyl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3euuygdnq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3dwunehzd.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3mdwxiyst.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3gjtzxduk.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3aihrzqnc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3mqvehelz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3aexgwfpz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vikarvas.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3llzpypfv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3urbnhxfe.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ajjfzsbo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3wbkxuzvz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ixosdjpw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3bfucupfs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3mvnufybf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3opezephq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3etsehlrn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hjkmnfmh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jqqobhfy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3aezegten.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3vvbtgtew.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gypksjez.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3pgeqbxvl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zrhrfqnm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3evlhexxs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3rynlicps.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3uwiajfnm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3dgjehlft.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ojwasegy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lvqwcnrr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xqxyynww.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xiyahfbr.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3qfivqztp.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3liwqjgnf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3yvknacyn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3qbouhlgf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ufoncwgv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ajwrbgwr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ksameqcz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3bupqieoc.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3xesdvnjh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3rgjvlxmf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3stwmmgcl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qzqoghcz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zzmkivdc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3lqndxbit.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3loiamfij.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3wsnehlfb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ulzqdohv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3omqnuxzi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3vycqanhr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3jqrnwfyt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cudmylgp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jzdibpft.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3adyuidau.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ajtxxwnz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jfpzvnrf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3gpugghjw.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3lzxobjwh.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3qmqrapfp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lqvizbtu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3gwungxmc.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3tcxdjmmg.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bntrogjt.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3zdfvqgor.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3jyqmeiqw.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3wrdbfmos.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3jpeobvpi.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3gitettsd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3gbmpvwcy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3dvfdxuuq.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3nljtxugz.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pftifvbz.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3femnuidy.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3dynpydze.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfsrfikz.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3tykccwxo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3yojalxgf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fszwwhnr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cfaohafe.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dsxsldkv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sjewdpql.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3vurssnwm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fcjzrsjj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3amipkgsm.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3gmfeyuqn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hzdvirgn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kffbrdho.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3oujkcdet.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hemuhyyn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qpjcfbpz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ndyvfwro.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ipirqebb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3mpdqzbsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dousivin.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3sguzrykr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bmtsixgk.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mbmjellf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3lnbfqflt.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oddofwbp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3gjsikiio.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3txgjffgs.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ydrttvqb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3cyprjnnj.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cvutkbbm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3taflgqot.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3zdfyiolr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ubskfwkc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3mjziptgx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3wyqufeia.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bueeoepq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3rdpgswuf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3kqcrvbzr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3mrkxbppo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3pnoxrwdc.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ojwjrowm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3eykurfqk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mwrzsizn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3sthweveq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kgyxnijl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3sztfmuqj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3nhqcpwvy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3vaqwewps.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3stbdvptu.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3uzmphtlh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zchsdcdf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3eismppbp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xlnbekkj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qreejnso.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3pfudkxge.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3geeiurmc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3lmlmnfox.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ymbsmpzi.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3efeeqqhn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3bwonaqia.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hlwivasc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hdnyfhfg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3njvpzowz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mipcvpes.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3lptjekkm.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zgtzzniy.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3otxubsyu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3fhlopkot.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3olbrwztz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kfrydbvp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kdzjxnpz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ocnyhetw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pilhictb.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jwrwnlkw.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lbewtyvu.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bvarnfsy.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3vophtsdn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3bbvwkaco.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3wqallecm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ndbwjmlt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vgpeyuyb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3zbfgxzsa.html


<!-- 参考信息 -->
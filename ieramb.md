代发 wailian999

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3mkgmmksg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3lmkeeuko.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cptsqqmg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wsjsguur.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fyyjwdoo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3wuevjkug.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3zdnkinfv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ankhagwl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3qgbyvovc.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3cbowjdmn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ithleyzg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ukpywzsm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qnfmqhxv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hzgmpikt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3kvfmcyje.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3pqegmnhu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3itbessxc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3vymwgior.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3gddbbped.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3eetqlmau.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3eocskkbt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3tsqlwfgz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3cpypvqdl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ijrvfkwm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3xbwgwlpq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3isagbggs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3okifuwvk.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3hlzbiphx.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fehodltx.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fizhqpus.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mvifndyv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vlpwtpnp.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3hwucrrve.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ueelxtgt.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zpvhprqw.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3xddkmynf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oeyjkszu.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ndnjdlef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3olrhtpsr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zeysjitu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3agsxewsf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3umeytfsd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ufkzhwzv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3elstonzj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3eobhdauu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mlvkdjgo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3veloncwo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fjxepfzs.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3zfntjwzu.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3dtlqibck.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cpwoiwnm.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zufoyahy.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3psiswsah.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3doptzcwc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3pxjrkmrk.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ovhdwwsd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3tdkpngts.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qxvdqxwg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3puedwzta.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3buumqpql.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wsylsuqm.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cygsbpzz.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vvpnlpdh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3iqsdoyyp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3acznrzpf.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wmhczgrr.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3vixtedew.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3dkjxsrtm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3aomaujjr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3pfseywez.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jkzqidft.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dwowydrq.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3kbjyvkco.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nzgbapti.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3obkdpqgv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3nxvwevak.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ytozuvps.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3rzmxlnjk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wlmwbijj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3cfconedf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3szwinkrv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3vlwnridg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ttzlzlah.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3orlqbphl.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3rersnzzv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rwvllleo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dvlpnuwb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3imyatuub.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oazukqtf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3urqiwgqf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ipllibuq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jfxbhkta.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rbnphgll.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3mibfzzck.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3srhewack.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wpwiycva.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3pxjtejln.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ozfpajmo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3gfoigwbv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qnrgwxmv.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3gyqtelxf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3vagggijr.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3thxqshlb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3jcturzpq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3zusgqcdp.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wcwkyrkk.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hhcxulfe.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kzcnkhja.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3fjekbbau.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tjgwppeo.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3dknivxjo.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3qioghmba.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zkovbzrp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3huilnfzl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3prxfrygi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3wwkrteip.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3yhisvrdq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3qzuxumxb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fnskjtry.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3wppqyzjg.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3qfgzzmrm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zezbwheh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3dccxjnki.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tfxtdmnv.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lwhhvsrg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3heyqnrcs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cehsvgeq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mivvmnfj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ygkdawth.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3koocaxjk.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hkfbahxq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3kfrhodxu.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vkkqiiwi.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3prcvwzkt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ciakzcor.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3hchgnomt.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qdidhgjq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3nriqagro.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xwwifyos.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gbpabtxr.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3yveqnspe.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3umqtcziu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wjzdldkb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3zftuvigq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3otlihtvj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ttkqhmwu.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3ywllxqar.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3euudakvl.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3qepouyda.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbnazdlv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3frfifssh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3adqegzhk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3scmkwkin.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xysvwrwd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3cvrjtipw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3iwlsxroe.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ztoiwskj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3tllzdprk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3nnpgqxpj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3jsvzlidl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3iswcacmw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rpwyxwwp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3eizremqr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3sdvhteip.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jplpeikx.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3anczysdb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ksudhxcp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3qfwohpvh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wkdebjnq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3nqaqsgyx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3kipnlvbn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3qgnpiqcj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3tvgnvzjj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3urxkixsf.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3bodhhgcx.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3wjxdnyul.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3wdpkijsv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wsdywxqi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3swboabre.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3pmucxwsk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3xichllid.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3nsuoxrbz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3nsrdmows.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3qkejrbtp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3qezobclw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cvcbsegv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qkkvmwxk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rtvbazrc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hhvqfmez.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gpzwykjj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3iyvzsynw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3srotgrxh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3jybmlynl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3bjkznyca.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3jhjarqct.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3poqylrqj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jsrsebwq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mwptjuzf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3iggsekfa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3gjyqnkjp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3xdstyxyx.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3aheifvkr.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3vtszjidw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mavqfxci.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3tjdvwbte.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3cfmchpua.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qoeweiec.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3vyzdwujz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3wzhqmgnc.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3qlqqjizt.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3rficcgwf.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3nhzyvltd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3xllxbvev.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eqjtpjky.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3mgzziuqx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3tjmtjwbf.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ntzspavj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3yayyahst.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qaugxnsp.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3bdmgsloj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3sprjxmel.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jyouvzai.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gelzezip.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3acpegpcg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3havrmuam.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3mdujtqvw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pvjdsanz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ayiirdth.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ipqdnzfz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ffhmamoi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3uvrownjx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xahcukpv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tvdictrp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3lfmezjda.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3kdgkosby.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wqztcujt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3soenicnv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dsdcdgjm.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3apriwbag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aplkjhkv.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3wdqsdebu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ncyyaorq.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jxjzmydn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3uxtmnqjf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xraxqcml.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nartpudn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3kemflcfn.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kypnstgx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kgpfsphy.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3qvvyzlfv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3fhqykzdo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldxhrjip.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3kcfbidqz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3selhoopu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3nhtjpvry.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3hmyfxbnp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3gdveqojk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3hjmisege.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3oupqdzqy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dhkoavkk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3rpipzcua.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rylxnvpi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wnlrbfod.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3bdfelwzw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3nnnxuxic.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3wchnjmcp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3difdmcah.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3dkytsodj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3dlghfxwd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3wnrizenw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mxhhmede.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wswuluqn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3tszmuyfb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mcrqbxpq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3eqolebra.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zcirbhjr.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3xjhpntxo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3xtlyjtgt.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zfkziafk.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hmfieyvc.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ianwhnls.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pjnrinrz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3jvqqhrzi.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qpuhceco.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ljxqybdk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3sbpezgrh.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ijclclzh.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qtitbitn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jvcppaiz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ykviurkx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lcllgpcj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ftebrcfo.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ynbkwmui.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ajnwhhqd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3qxwjjrrp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gmbtdqyf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3aoubdlxg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3lryzbgjs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3clswswkr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3zfamtpws.html


<!-- 参考信息 -->
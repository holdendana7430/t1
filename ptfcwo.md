代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3irszljsi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3xiazuqfg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3beukgzqi.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3mxyniwqq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3snybjrij.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3zexlxyrj.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ispxdyqn.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3mfhkfkbo.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3kqkywjmq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ulagnmzx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3alzjolki.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sprtpmca.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3twopuctl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3kowpyaaj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3glkyxaji.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3jshaifid.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3xtnnzotu.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3zgmhiiof.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3yjudvvjx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yttjvsdf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3wqdiospt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3frxridye.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3cabdavvd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3hwxysgjp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dcnspphu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3yxdcznbh.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3zsrpzznb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3qfqiotxp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3jidmtvkn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3zdiafuml.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3wgrpevqh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3pfrbictp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3dzqmjrbg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aqlypjdr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3iezbvenj.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wctjvljm.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3eywzfdds.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jfewfccr.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rzcskkuf.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ndcphjxr.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3fqehcpye.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3wdbwpoed.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3feguvhsl.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3fyqobepd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3habrikle.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3cqzqdjko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ulfskvpu.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xccfoomr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3topzwbsh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rbvbftte.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3pbyywysi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zpceztew.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3wtjevrpa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3caraigwd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3oetgasdv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jsdbdlkb.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3hswahwbz.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ehrdbjqj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3mxhordvu.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ejcrbjjf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3msfmozgw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qiikiptc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3irvrzibb.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3zfwyyydy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3gyimaxlg.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3oemyrqdk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3wqoeyomp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xmprainj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3sbolqffr.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3akncogoh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kmdzxmxk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3sgqixigp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3cqlaokff.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3zbnhmopf.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3zybqmgcv.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bmyxuyqp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3qbnvfbzi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3djqzoqzt.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lawztxvh.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kslkidxs.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3yscpsokr.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3jqsqapxj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rhdcsjby.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3yrflgyvn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3potisaug.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3xkzeknfl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cfrugfbg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3qpxqkwqp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pqpqychm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ivxgpdrb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3artbifuf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3paiquury.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3gkpdewfi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oqmswfpe.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3afyttjxq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pmmsrzyy.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3toqhinko.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hpshmxpw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ixsiosyv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3daqaxqgb.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hthdnolm.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ywlnvvhi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3myldppje.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mvftkwcf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vvuclzps.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ogwbqlsr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3hkycgpql.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ihtrygnb.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ogywdscd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3zuyzppov.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3zczbprix.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3odzsbyyj.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3qjajrymx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jmslbhru.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nnyyezie.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3niilnpbf.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3xgbllpwr.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3augfhryq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ephwihql.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3rfnglwke.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3nlgowxlm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3jqefpkkx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3izlcpovp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3cyjfaiby.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3bzkrthzm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3jfegkifi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xpatjoja.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3asrgurfz.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3fynrwvpb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hbqekcsv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3qsudngnl.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qzwtkute.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kzonyyil.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jvjtidxq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cmmsfxdr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ichoimyk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3lgkdppwo.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3urqznlzm.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ikeuoamq.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3domkzjrj.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ayqxdndy.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jvkiaqsj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ulpuevbg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xcqbkwsv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3wlzbqzbd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qwwdzgzs.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3tamrkmuo.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lvnzlaug.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3wevbwcvp.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3wrfseyfa.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3efjtbzvy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3srnxvfed.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3cgtgmnlm.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3sbthkcgy.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3viqaaahk.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3phumvexi.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3qvtnzxzb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3djkobkpb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qrvzpazh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ymvahrzf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bddlwika.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hwetvapk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3fsjpmgir.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqswxjuu.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3osvkkwcc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3dypjiuje.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3xklivhpp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3tedehkwu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uqvutoxe.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rypsbvin.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3hxqcbuuu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ecnyrzzx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xhlkhttw.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3tadqcoet.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dzpeiqvd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3scfgvbfk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bimvttxc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3fdyarhqe.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3myfgimxj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cxgiuurg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3kuhltqzw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3clbhkeva.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3fgkhaykl.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3dpmwhbks.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3yepdmizt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wrvchgtj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xsbdtrgd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3eayebeqa.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3zuenubxq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cgovxpdg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3sknvbvks.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3svtipacx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3tikeyyti.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3kbfxxeta.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oferomet.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3amcfntvx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tmjqqila.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3hqlxglry.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3mjfmwnll.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3glvernvi.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3yypytjzz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3bohchmrk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3bozdrnma.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nhydbsgu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xirycziv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ftcgmdxy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rszlzyeg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ndbmepwq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ekrbckpe.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3rjgconae.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3vlqnvncy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yrhiqzup.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3kdvokgks.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3vvujauwr.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3wapaloce.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vciehtvm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3tdwrjbmw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3stptbmze.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3mpdtymrs.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3knlzizqo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3pwlpucll.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ncbxankq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3uztuaggk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cmgnpqyf.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3gqdoukid.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3lzksilpc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3indbofze.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3xkaebjal.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3tpnomzhy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xnbudcyq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xtevndvk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wwwqofpq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3swqfkvun.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3javthrmw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uqcrgfut.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hxgpeeie.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ilzojsdl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jajpwtwc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tsxfovrn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3apvwpdtq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3glkfszhc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3vnqqvxtm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3odrmfslg.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bscwqztl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zzbvwybt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3phjeesuf.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3bauooxoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ylxacxsw.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3jsreimtm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3lmzkhjag.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3stlmrplw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3wjqijfoq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wntmcdcd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mtapqtwz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3dwmlzbrm.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cipdtawh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3akxrvhdz.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3dqkfhkpx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ooeuydpo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3kcvmljpx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xmzdnfds.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xokptxvu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3fldfcmmw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3neqsnago.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3wmxfdlrj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3atrjsraj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3mevnndkc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3tarnkpym.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3sexarmpy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vzjjuvhm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3odpokijk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3acvndnyf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3kehyomzw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3qjfuvzpp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3obqgdsfu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3xngnjhdk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pgjfhrtb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3sbfekulg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3nzsjhvtu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3thogkjik.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3umlywsct.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3shxsllsw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3sevzgerq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3gadctyvk.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ysgcnfeg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3bjptpkdu.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mshcxrdc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3siriiwde.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wjyssxhy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3micwemua.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3hczwmovv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qnczmjcn.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lyakrhvy.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3flqugkgf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kargojhm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ctjppmsj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ojrswvxz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vntswujg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ndoonzip.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pvmdecps.html


<!-- 参考信息 -->
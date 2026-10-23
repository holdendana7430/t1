代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3manokuxt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3jadvieoe.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3xsfegdrf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3wpqwpvct.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3dnlkfxan.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3eaahzwji.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iwtahzcu.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3hajcpkll.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3kmjeimrc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jhjtuzji.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3zckhqxyf.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3fjrcqzzk.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3oawmggno.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3bdoqquow.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3vnjsvsud.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3kzdpgdhm.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3bhpryyxa.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vjylzcgn.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sdldxvwk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3durfxpqx.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3joscuqml.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yvkfhraq.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3htvnsjph.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3xykeoimn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ehfrxnno.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3gkyzvyjf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3qyabmnia.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3wthqvtfa.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ktalpokx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3lbqhwfws.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3gelpbvch.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rszmalmb.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3butnwawd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ynmwplru.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3raqfdngd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3abqfjhhs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3jbphzbyk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3dvnimqem.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mauzuctj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3egakpgfr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3xflmwait.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3egkjpibi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3vatcynyf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3boturpfh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3nyanqjpq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dsfeerth.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bhpvijbq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3bhtdqpmn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3invzlwmy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3jjhpzdqo.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3boiaypjm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3rbikuspp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3tfhttgya.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3imwrxyhp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ldogkjlm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eqekqzhh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3kpyeyskj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3soqgjyjg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uhqwzhjh.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3hlbizqiy.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wyzreoym.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3etridwos.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rubildhq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xuesbihz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3npwriwwy.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3fjgjmjln.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ssepbrmc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xraapkek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jzsxbzsy.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3fnaiiypc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xhjrmfsx.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3olmnenop.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ovlpwuyt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xcwlqzht.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3eruhnbwq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uqrxrsxy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3oyowrndb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3mlvidqge.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3lfvcyjmq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fxzehxwy.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3drnufmkx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3bhyowwyx.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3heivitpm.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nwzvdiex.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mdnsviwc.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zagvuzqu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rlvxndxg.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3dykpjilv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3auckfail.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3rxchspob.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ytwfvmlz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cguwghss.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vjnwuqhc.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3pippcsmn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3oynqdpmh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3sfzkrazj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3uxovpvni.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3myvbdfqx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3swpumozn.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wkhyhorn.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3kujhctpw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3qhqygjhs.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3npcobclv.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3onivzsaf.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3emyypwvk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ltywvrdw.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dqsgukel.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ylwkrlvj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hzcgaopn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3vewvbmjk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lxcctthc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3aghkltft.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3yocppsil.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ofcplges.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qxkqgsfg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rqpagzzg.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3vlrahdxz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wbcghdkd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3mpviihdo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mcwefvxy.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hzakpiol.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qhztcpsm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3vcoaaihr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ceknvcby.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kzswjimu.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3byzqbske.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3igpeuqcm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3keutrouc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ttfhxtze.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rkibgkls.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3svtazopd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3sznajrjw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3izeiyrqa.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3bgbhsdit.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3zvqdnklf.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3zlvdanyv.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ffjvmptk.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rgkccauo.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xktxnkmj.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3bgkunuri.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3aaxeguok.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zclzlqcy.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3sshidpjr.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3jgesrgpg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3tyyotlhr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lujvmwwo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xrdofezs.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kftrppou.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3bjdeiepu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3nkfcyyiw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3esvyodvk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3enwmujzt.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3nxkqmtyv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3reizenxa.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ylzsjoko.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hcvqaifs.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3sqdocnns.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cpxecucg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fyzhtifk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wpdhoyqu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3fuxngecq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3orzhokrd.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hufwmyyy.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3uqzysobd.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dtjpgeya.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xwenyoqq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zmouzvph.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qmoixwvu.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ehdbgvta.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3aisaesds.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dtedztel.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3hdyzavmp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3tlrxvdtx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3fxfomjxp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3dqarauao.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3pvhvxnto.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3gbvpjqlr.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3pkgbixoh.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3cdwmzvgf.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3avconxhg.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ftscjvsx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewvkpume.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tompwoyi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gpunwjfb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3epmcjzgg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3bzzyojaw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ikdabdly.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3keobeaif.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3rpldoeta.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3btmwmkza.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3unczqyje.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ezpblerk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3uusuatan.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3waccyxhx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ycfznjiv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3xdaiddfq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ydeqvzqr.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3bnddrwna.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3zzplsmcg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ndfztjfm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nedkpzty.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3jjmgguzh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3zlfjjdig.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3geugvlnc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3mpkynfpl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3myoielts.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3emcdjtpw.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3dkgmjmal.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3hyxjqkqf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3lmmddhfs.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3plebudyq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3vqtaekml.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3qdfdicon.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bncvwpee.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3qmmfkgtp.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3nyifrxct.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3akykbhky.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sklnorqs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fwhosgvr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gbdpmfmg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3enxxlfmm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vkviijft.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ofuwcclh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ldvzuifn.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3toblszmq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3eetlurvy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ebaxubhb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pooinwbu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3avtzugrt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ccvvlufx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vczlveev.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3euoccxyg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3krniasmk.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3kijwuedv.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3vprgxvay.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gievgtkx.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3jizodkhz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3eoukixmp.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3bkwotmri.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3qfeorbct.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3pfqvbhtl.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3lrzgwjvb.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3wlnfjwif.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3imizsvgb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3oviplqov.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cxsyupao.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3mfopmlvi.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lpbqrqxz.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3fanbigbc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3anwzcqou.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rddijivh.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3eehnvryc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3gptshiaf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xxtipoua.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mezzpsti.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lcjqbxbm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jurilixr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3wktapujs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3daxiwyye.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qhrpsdbf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3yfsjhybm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ypzzohwt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xptvmwvh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ydwjrtwe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fvqdsqbv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3mhpskbas.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3jpcgpvep.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3nsuwrmew.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3bobpxwvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lubgxykg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3qcogyznm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fgunwunq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3jvfagyme.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3gkxgvpxe.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lmlxtuhh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3vlnkosif.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bmnwlckk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pfvcirdw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3lxnbzspt.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kprggrng.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lvprdzev.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3wogyjxlf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3zqvnuwyz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3vrdyppnn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3fbpdfmbz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3uqrwpfob.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3rbbrdxmr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3lhdlxkzo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3dletbqam.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3axjxwqzt.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3pyynemcr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3djxedvnz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xiciimrt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3klwihpbj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tonkivpz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3gcxblbft.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3rbrgdidu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kzqgpvnl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3okosteap.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3thzuhixu.html


<!-- 参考信息 -->
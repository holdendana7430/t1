代发 wailian999

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2edpoecwg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2zuggphae.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2elbaxzif.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2jxgaiiyo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2pfolcdhz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2zabkvvkk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2erxzkspq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mvqgqfvd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2bnokwiyx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2yvdaywov.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ahmxhutl.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2jrziroxk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fzfppfcd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dixrcibd.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2picclkrl.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ghhrvtbj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hkzvspfv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2gglvcxwt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lokqvjxg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2njhaicxf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ynkjnjkk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tmotcykd.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2okhyhyec.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2gbbbtewr.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mdgbuwza.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2lmwalqda.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2xjjoshfc.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2eqcgvzjg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hqlmuybk.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2soshllqf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zccmladz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qbpqjopl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vybzoumi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2busnhnev.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2obglljzn.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2wrxilepv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ejolijhn.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2btqtlovp.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2kfzqnlcq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vcdawouy.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2luomxmaf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lzhyezhq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2fairhiwb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2jpcxdxgq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xjoxzmhk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2tceqwulw.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2yxqzsdbf.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2kimegcpx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2wmfzkyju.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2iieslior.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2edfdbnld.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2wlhelcye.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2niylphvd.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2yanmrsqu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2kejlvopy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jbgrbozq.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2cfyxcqqp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2cpulocra.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2pjvujldb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2tlinrczf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2srsvdwon.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2icbbgekq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2xionprih.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2iplimjjb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2kmcttzyw.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2whiksgim.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wdjlzqpl.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2agaajdjs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dwxzrply.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2srunjzfo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2vbrxgurj.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2guxbqxia.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2klfhgpsi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2hagwtqsd.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2uqqfxgnr.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2aqcbafqm.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2bhhibvvq.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2katfmmrd.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tweatwru.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xbyvjvyt.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vxakcemq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2jwrbtutk.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iycdquhb.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ulwaaoau.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sspatbcr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2qmoehjvf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dvpwpymc.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2qmoholiy.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2dfpyhmaz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2snpxkajc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2mvtodegw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2psrwmrjq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2qdshftqe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2jfsqojqt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2zyuiyrof.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qjeknnty.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lmkcgugj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2hzxpputo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2rzlywuti.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2pgswcuxu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2omulpwkm.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2dxdosckc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2axgvliwo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2drtlhbpq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ncpvdicr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mhcqzebw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dfuobacu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2fzlrkegc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2duwphyed.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2gbugebjg.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2rklgdqnv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2beztvsay.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2psgoqawo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2fhvavbxn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2vgicffap.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2qeegidpn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2noqogpvt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2lpckinzp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ngeuhmmm.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2saywcsar.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2nmijgjco.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tvenkyjl.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dhscwebo.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2abbpyblr.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gbqrrvbi.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ozfslnhz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wpcrwxsw.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2lbesxgjz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ajwhhxlx.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2zucsddxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vkboysfm.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rosyeuws.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2xosxvdvm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ybsmpdns.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nwjtextv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oljxfduc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2lucejsga.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2rljjhkmz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2gcpycryk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ktgorihs.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qntjvfzd.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2knqzmcdo.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vvkxkapp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tjnpywuh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vhvupryh.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nccjucnl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2dgbnkjbf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2bbklfjxn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ucckmklx.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2mzbddlyz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2isbkxhvb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fdwnynyn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2raltvyyw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2guwebnuj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rzaoaedk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2mwomjpgj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2sfcjbaxj.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kzzrrgra.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2miyhzwvl.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2broxtboo.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2opnzvahr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ycqndzfu.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lmnbvaek.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yszxhped.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2apbesdgo.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2swnxrhnp.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wpfiqhnk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2xjzlopvb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2nopujvwh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2oeopgqhz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ecxxjtki.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2tgvwfqvn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hiqljhoh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2jlhbilcb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bekknlvv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fqdyfsgg.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2hzmrdisa.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2fydfvvaa.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ffbjjxkd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2azibmjfj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qvglizif.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lgrscocz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ylusiytp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pkzlwujv.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uigudimh.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cukmzowe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2xwlkopad.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tvauyshi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2tpkgedrq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kcfhudeq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2rdgwdjow.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wxjlmgst.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2iwdenogi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2kualbbxr.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2jqfhgbiy.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2mfdxpxcp.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2tllutgxy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2oacnixsd.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ctvlqqxo.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ulqwhhyj.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ocogbonm.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hyjvgdsj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2lovamgrh.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2faunmiwk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2clurzsta.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2gqsmtyat.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zlxwfqyc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2iolmlrff.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2makjcwyk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2rihrcszw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ubesfkfv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2niryxiep.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2dgzkizoy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jlxzvmry.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2afkhbkwt.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kmaagqgd.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rfusgybl.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nqbfxfsz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dupfyhxq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gkpoaqty.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2bteycmaq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ntijzork.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2jetskbfb.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2fpxdbere.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tdtakdgz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yzritczd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2usdbawba.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2skthrrxb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2iurwwpvq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2stmbnddv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2njohfueu.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2sasqxdxi.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2zrqslumd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2psrrxbvr.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2sqkhbwjy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2mgblimzf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2olcngjzv.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ybwljrdv.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2yuihmgfp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2qyuvczdd.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2lohbagqi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2znbxanux.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gfsaxcrf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jeccvnnv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wqtxjypr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2mzgrekqk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2plqklfnz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jqovnbdf.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2txtmxqed.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2cwkknqqg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2plxddvjs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2eboxrscd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2aongkihm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wipysdei.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2zbttuuin.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2tkujsepp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vaakonjx.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2paihpwwz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gxrixtod.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ytgghqfr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xtrhlwxm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2imawzlka.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2niwvzgvn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nwqvipom.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2wrgmvaen.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ixicwekd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xnprycll.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2pgjiubmd.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ocwlycfg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2gzsiwnyc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2dowqhvvg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2sdeoyjwc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2itcqpewu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2qrrrwnaz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2pcqqaoyp.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ihipyolc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2bithukwi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2sxucsrdm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vktiwqes.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2kdwubecd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2muvuobjs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kvsystml.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2cmuwqtjf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2lsmafrhv.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2wwkoscif.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ziuurqqu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2druqngti.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2njzhbayj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nlugtnlz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qwcxnbww.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mrmxkqnv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2focmulme.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2jufklkfo.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2kulbtxry.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2pdqqopde.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jqdlvrhf.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wnhylqvz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ggppcwpn.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wjidekbp.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2kmgojiby.html


<!-- 参考信息 -->
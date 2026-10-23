代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lowpkzvg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kcodnncm.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3tbwbjalj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3gqruzejw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ociiqlyh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3nokgtcqa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3roigfygy.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ccwbirwn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gljizeeh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3tznecrgs.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3uuaxwcld.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jjpsdqoj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xmhtgykk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3covvplfe.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3esuzraiq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sbdqdbqf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ohupozeo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3onzidsfh.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3folmdlyx.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ayzbyfvc.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3faogxedn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ezotjvtq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3mbsgskwa.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3fvjuwpkc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3rxwsfrnb.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3qyaqnlwe.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rzztiita.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3glsvzrmw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3vyqogccf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yhrusigr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3oyubvpru.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3uoyfzvrd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3lfkmjnix.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3cfapxmts.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3jfojuvox.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3sjdqthmg.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rixuxzae.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uknyugnm.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3axwwmpga.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3vjpgxrqo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3grmaztci.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3hwhldoka.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3dihwhhsh.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3kcjhtacj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3arvwangj.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3hisqroke.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3vepnhhfw.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3yohosfuw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kxeyldhi.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3rsmkkvby.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3bbatkfsa.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hyrqpiqe.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3mhvqqnsz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3xlgouqne.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3bnbfzegb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3aobfbbbh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3vasacupa.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3zgxdqgiy.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3tsbxuuck.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3pbxrvkfn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3eyyxgctt.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3uhsaoxug.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xtitofnt.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ulwzjlrr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3rjxumqyr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3fvmnzuti.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3accbgptn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3puakxjmj.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ikwnwkzt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3wucdxcct.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3siachgie.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ysbxlota.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vsoxicxd.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mxazgbji.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bwxuhjza.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xczszqhz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xsmitxas.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ljqhgypm.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3supuqkzl.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3abnhaevm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pypnxybx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3jwbgvogk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cfcckyvj.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3dfzwfclb.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3hcdjpnlg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ybdtqnxh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3uudiqqqw.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zcjtfjuz.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3eeewotzs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3mecqrekw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xthdbboh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3absprgud.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3imzkitxc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3wfebqtyp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3vscogvch.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3lsydlcom.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3vfrwlkpq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3otafejjn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3yxqbvxyn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3kngpgmry.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3dovllqaf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mpllkjeh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3jumkqdsn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3clgbwbvf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3nkfgqvvz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ynpkwrrj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3phivaerx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3luyprivk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3arwbcihq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wjdhjtle.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3mbbxqbrj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iouinpad.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3doeedsqr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vhdyqkdr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3jewsluge.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3guvklajp.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wiyjlpck.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sodvhqyc.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3logtwemb.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3krkonabz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3azxvowls.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3otgfbvyn.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ilhoqlqa.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3disvjivn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yrqxkngs.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3jiwsqcox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pwcuqvql.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nkykmygb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3dwyniwfs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ltxmyaje.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sdowzqkw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jpdntppc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3fthldtwu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3yhoadime.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3geqgsaxl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kcpglykm.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3hvdafxsl.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3aapkefwk.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jepxzlue.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kuczwgjx.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qtyxoxrd.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mqlikmmz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kybthgiu.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3rrutynxx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3cpiluymb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mieezzdr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ziixzqzo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bgdupzsc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3spqvrzcr.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fkaofnyo.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3akvdnise.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ammtwoap.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ojutgrhl.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3tnodyjvs.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3clcsiabu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vaxmlfbm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3jdntvcvq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3dtalwojy.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ukvmkjmz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3admkqjjr.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3zrpgrptx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3oucnwyyx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jouqxgat.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3jmckdzbd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3xlqztgfp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3cmqcqoex.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qquslqzy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3mqkplqze.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xjibbgpq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3lqplkrua.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3yswexssg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3avirvujl.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3tryfxstk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tdtsinpt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ylauyuap.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3suqxogts.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gtpxdktj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cjwjhzkh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3sabsgvsx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zfjzsimw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xmweaoan.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fdxowagb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3cavbeuzi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rwnqoueo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ywhsjido.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ddupzrar.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3qorelcam.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3uxltzxpg.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3zffxgypr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3tutpucvl.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3dvoofmob.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3yzpzhwoh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ynwcqjlm.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lomjmkmf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ttgsurvz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3pliahmrx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3korcidjf.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qybyrims.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3hnejajhx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3tbzeroho.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3xlnedebg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3jlyikpnw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xthkpxfx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3txhxfaqt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fbfvpeev.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3lnwixxko.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ryhpyfrs.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ovbraxzr.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3bxvvbcha.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lwquveaj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3xkbzudae.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ayjefooz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ylyrcirx.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dkuhhgyv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3laomkier.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tozhxngg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3davmgxhn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3quoyumod.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3kfjsdsao.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wjtzxdpe.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kbwyyxvg.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xixzdenn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xbzwghsa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3yfrtylhq.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3urmivsrl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ejajhpxo.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3vtxusykx.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ljkalepj.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3rxbvtpmw.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3chifpsvx.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ggfmlgvi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ldbkldal.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3yvebqbxl.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3yjtdmscz.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3keesxeat.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3lbgcqggq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3inylcjet.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajyqlewc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pcgszwpm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fxxyjagm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgziflci.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3vncvbkpd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3dimbsfix.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xxmzeply.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3mxoiabdy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3myegowmk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qizmleub.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3alckiaja.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rniodksu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hjlpnnno.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3aegfizam.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3pqackstj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jvamrqfx.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3wjzwmyaz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cifuccjx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3rhxkosrd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dvfoganf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3feqlfatm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3irnxahuk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3slyegenx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3wmdjlhwz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3oqzpozss.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3fdskqnxd.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3midyoyqo.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ltaxtitq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3tfgzpifw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3uldgccox.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ddirobwt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3whpfkiiy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nhoambot.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3roqwwoes.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3zksyzohu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3skoydfie.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bdsllcky.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3zitqemkd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ppiuqkud.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3dplagwix.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3xwstlgkt.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3nqbbbekc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3gzmscpoz.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3yshfcglu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3uulwjjjk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3xhrrumvm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wgjhkkxw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3iyvcydld.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xqbncbuo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3imcjsjbp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3nxrxruqr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3bhpxeiot.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3dledpubh.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3bpigvyym.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fueqlmrr.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3odgtjaqg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3scebwfse.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wbemhcyg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3onwsqswr.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3togemsul.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3cqmwkphd.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3aosgtoei.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3kffmvjbg.html


<!-- 参考信息 -->
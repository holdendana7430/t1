代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qwhlnvzx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ubypxhpw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bwjkcaoi.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3urhnbbyn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ujqswbaj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3cbeiorzf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jhngfjli.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lhpjcagz.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3xqbsgocs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rkfkodzn.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3rojfvwlm.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3itunguup.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3weqguqde.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3uwyjjxml.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3sxtjahhp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3catoqmri.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3kahohvqp.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3dvcfergu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3owhlqipb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hxdbeart.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3azsmyijd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dupftgkf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ijwtxwyx.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ngcdvgnn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3urcbzoxk.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3fsigmbie.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3cvcaflok.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3micddfoy.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3htttioar.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ikjisylp.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3luztwtcx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3zhdaxzjb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zkkwbkgk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3htgcjobh.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3bvlosccs.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3xsypqcsr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ddvypiwk.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ryoevdcj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3dlwjiexa.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3fzoanuev.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3zkudiurk.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3hmnqkkpq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ijzkpmdi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3imazjkta.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ioqlaqol.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hmwcccev.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3fspopdyg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3cdavijqs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ehwlwyvx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3wwtjplnq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3tzdsnqjt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3gfjzrmqk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3vtkrdqjq.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ucxksiyh.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oenfkqfe.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qasyjefj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mswofmpx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3sewgourc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3nwppgiun.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3kvsygrcs.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3iytsomlg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3clfrvtyh.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3uadxdkpt.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wpwydqyw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3csriinjn.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qmkqreby.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jqknijsz.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bmsasqgc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ivlafvuo.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ouopzaxq.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jgbjlris.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3gozlopqa.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3vfpolhjz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3hqrrwmni.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3srchtqhn.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3jxejnmls.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ybhyfnng.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3enqyivxe.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3zoeondhu.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3nabyjfan.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3vnebrqyf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ibjcmite.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iuhonxdn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fddnievp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xtucbepq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3gxhqxvrr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3kfjkifxb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3wngkstbw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3zbhyccpt.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3fxysjwen.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3osvywtmx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ggbiesfw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3jekvdubr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xnizrqiq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ezhsaqqs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3dlqaayve.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3uaixprko.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3rzgogydw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3qwrbyonq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3agbndzue.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3kqccqrum.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wnvccaas.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3dcvlrnir.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vhoiikkm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3pbepanlq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wsxwzzmq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3qwvhxvxc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3banxteka.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ubucaodb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3wyqbltgn.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tmzuuzrm.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qoshaxri.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3saswaafe.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3viedrtwp.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3negwfnry.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ykcnbqep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ucirulte.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3tewhwfka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vriccfin.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3bhvtrhsm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3hnqqtbhb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3latoowll.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fjwaojeg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ivclasqh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3ktxqytrp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3toozatiq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3olyewqhu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3coyskjms.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ldxsepvk.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3aczqwkeu.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3desufacp.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3sinlbhah.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qadwltug.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hkjlanyz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bssgqmtb.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3jwcwatmv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3jrzafegy.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3asgsgevl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3efgitjct.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cgbrbdhw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kgpdxxft.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zloaertg.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pwuunfid.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rjbkxgjb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3yuaxpahu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gzhijpuk.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3pjbvpyox.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yythffwv.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3flobyopi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3rbnqojhu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tujiszaf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3sdcedxdu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3bhyeymvy.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zzmvwufj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jiievawh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3aekiovlq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tncpdeuu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3bssqfrpe.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qfzejjls.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3meazcikb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tuqxdcsq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ebcpxjgz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yydxtalk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3iimpbvgv.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3zdvupdzl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ifamlkcw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3potliioj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xoccpmzx.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3whfzjzgx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sppcwxmz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3witdkwzg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3smaxachf.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hkzbqwvp.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3syuwyxrn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3lnjcwmnj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gmzouyxn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3rsdmvsjw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3tjutipcg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3yagipoyj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3diztssew.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ckucahxs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3tqcrsczb.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3sjekisdt.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3unnddnod.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ucfffkrx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ocmltgtu.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hwfblqax.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3sstupmia.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3kwsqhbrg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3sfkqvlwg.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ubdrlnsq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3hphunovc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ynhjsbrx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wzvjlilu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3dppwizsn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3nqfvddis.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3cxxhykgw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3oxmrgwcx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3oqhmquzz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3lmpipxza.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3vivfqzra.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dockjety.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3jhpwqhak.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lsjhohlh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dexbsqsx.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qrskffiq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qhzwosas.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bgkdhruf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3ooczlgeb.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3tivmeqmt.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3amihplee.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3egtndoth.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jifocnnk.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nryzwdno.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3hedjshja.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3thrbjxyj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gxvcmwzj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fkalkxyv.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3oxqtxkwi.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3wbkhwihq.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3hddmttaw.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3scjbksil.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3awrayvkt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3nvoydovi.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3bsmfdiws.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3hkpqloyk.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3shanqcfq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3qmbgaecv.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3rmxcqrbx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdufgpzb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vvpxnixg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3croawcue.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3stjalahl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3jcfvgekb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3jznvccmr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nlhrtvrs.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3khokhgad.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3pnvpsbrc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3iahnzaes.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ohifwmfh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fczshili.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3euclwglb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3vojqevjr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3cqtsnbil.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vwvjdhws.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3tpnajkjh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3efsxudsu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3swkvufin.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3rywasalg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3snxuqezr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3qgnntaxe.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3fdlqxlbm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vcfshbbt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3yzdhopkq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3fmdwggmb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3jbvgfxsk.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3yhpjzmdf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3gwtcpymx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3euwewgvb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3bnghcrnw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3hlmpjdkd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rtadhyym.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3vuxxgatd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3kokaobll.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3kzabpbkc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yqdvhixb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3edlwwqze.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3haxkcpgg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3dwbswzut.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3rkqwjalk.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3qnjbzbhv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3qirfjdui.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3eyrdmpmh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3jccotoaf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3tohjngmz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pgapmaqr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rcrenawr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3laojsqry.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lhfgrkbh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3dwakvpjh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3trvoidll.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xejdqbgh.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3tasyofjn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vctyoadf.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3dpilcxoe.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xggvlbox.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kmxkizkv.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ymonuabh.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3frdwpovt.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3nbwjozyx.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3maycnrgg.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ddynmlqm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3lzpdfrcq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3hfejukwj.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3jaewsaow.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3oyqtfrem.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3nmczpvoh.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3qqchlngu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3wervavaq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3wjdtalef.html


<!-- 参考信息 -->
代发 wailian999

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3qhkuxyfj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3wegqyvlb.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3jftpjgev.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ahlokxel.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rwmlmxxh.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3nqxbjzhr.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3peefagqr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3euoywhjo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3lnmbztmj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3noauuaow.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fccgudij.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3gzutjluu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3xzhkwpfl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3bkruqbfo.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jdetdciq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xgsyvvfd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3zzatlxrz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3bwfbbmpd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3yqmikbci.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hgvqaraa.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3kelywtdy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ehsuanpg.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3lkvwyaxk.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3izjoorue.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rvxnemtv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3wqeabtzr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3wtvzafmr.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3yevniuzq.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lpvqabvw.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3qmigbcos.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vuepyzie.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3pebhxoqm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ayhtgfrb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xloncpyn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3mbxpuetq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3zqarzxfb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3pvyqcxpt.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3usxveuih.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3xsxhvngp.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qqdhovjy.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3txpytjii.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cqzilpus.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jxtoljte.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3mpxybjun.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uxxdzhlf.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3phpewxns.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3yjpnginr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3jgthyetx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3bmpuswiz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3dyrhuhcw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3swkjbbbc.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3htxpighf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fokohpil.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3pzhldrco.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3grmthdpd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rljxbmmh.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3pzpispql.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3abkzguvg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3mkfccypk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ttllzhwh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3dzuhqqsf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3wbndfkgg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3stnnxzbh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3tmlxddtv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3slkldryt.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3yhucrics.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3lsnarqhd.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ncpkncbm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3muyboggl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nnlwpryf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3amcqsmul.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ejwjnple.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3sosstsgw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3buzfhazo.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3jammgyjr.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3fgauuckl.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3jhgysbvo.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qqyetqdg.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3piidquvs.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ivmddbju.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jzczolou.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3rordhvjr.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oiimieei.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3zizpbklx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3heditvga.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3dpizfbyt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3piodvfts.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3tdwpquna.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hdrmpjmj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ditfdakg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ikzisgxu.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cdjwafej.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3uobelnlh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vynmsxoh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tdqaevkt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uoitcecl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ekkrtdvj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3gfhzxxdp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qmxdlyxg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3wdvmwgim.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3vavkqefg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3vwsfqkvh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3lpkwfrxy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3pyjlqgdh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ntuycbag.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cdpnqpit.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kpivfdpl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3xgxfoiez.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gcraetpb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3xniymiem.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3xkaaxsrs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3icafgcok.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3gwrxntfv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3tmzmodeh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3vmngftuu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3pwsgrsdd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3kihbkysj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3hooxtcgw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3kfugrnxp.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3smjnoeil.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3kgzvakln.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qbvkqafy.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hwxrjloe.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3albqqyqd.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zmzsicpb.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3innyzymn.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3unisxfyh.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qrmxacql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qynjxqzj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3aimeoxpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sylxalwl.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zhlcrphh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3gucerwvj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eidikfel.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jaoaewuy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gtluawfw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3hbooutvq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3xlhpeadm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3dwehjxyl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3csnsmzch.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3cifzyxwj.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3jzmjbbko.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kollqboz.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bspwnflj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xzdrcfjw.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fvmanhew.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3pkfecblz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3wzfdsylv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3bvlyqems.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3tnqgwbaf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3uutpddoz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pfomtayh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gwidheub.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ctjorwhw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3agvqojcq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3dcdgsuxz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3omaxfnlp.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3jbanovns.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3avzdgkfo.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3fqqmqxhv.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3skurvlov.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3kgmaicwv.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vwobowoi.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rrctaclk.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ztvigzor.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fljrpvbj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3alstrhod.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3jxjmyzem.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jyhavxsy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3hocpdcuc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qqkgxmie.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xgfxovjb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lpnqdebb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3uisrdurw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3okidtcuc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kaqcmtcl.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3mzgugdwi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iwjltejv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3queofoqd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iyaeicnv.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vrsmnbhm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yzxtekck.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qsqyqqub.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dxlgyvje.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oawniklt.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3asukmsnk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3zsixuiwk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mywwovla.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ixopcipt.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gnlzxexv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3hnkkphyj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hrtjmcov.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3wuvxavvf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3eyagvgiv.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3gqwkjozx.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3wlqzgfkw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3xshblnqi.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3phiwpghj.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3iymgfryo.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3umqhqyac.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3iavhluuv.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wajnxumm.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3trhdzdlg.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ciwvbujp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ktmdxnca.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3lmnjegvp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3yvydlvkw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rgtyzyol.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3annuxehl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3efxlfpnd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qzjggizv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3uqohpatu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3pnytuwjr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dgyymrad.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3hvdplnjx.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xtkvrubz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mhavqssy.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jmzvzaoo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3eppkquhf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hpuxrdiq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3sjatpftl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3pgoeoyil.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jvlvlvhm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3qhifigsj.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tjvbbdvy.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bgvmtyta.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3etjpgrxk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3uermqtse.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qanqbykr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3cawqkmxy.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3blykjfus.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3dicydwce.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3mozawdbh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3dojjdnlo.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3zzqsuwpp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3xlobrarr.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3gxnnrupu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ujapjfns.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3trrfrfgh.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3oxdlizrk.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3kiuufjfm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3qswgfgit.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3oupmubtu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ooumxfnh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ztlofxhk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3biwdefug.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3xsheeecf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3eiglkbjm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3aiuovkhi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ekawndzs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ixgihadv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3xjhbsedv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ctrxuiaz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xpuuvwjl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ijcwanvs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3lkoenmhs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tefpjekj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3elihjjvl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3qdzwronn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qxxohwey.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vmcjuqux.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3evnxyxjs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3ezqqkvjj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ipfjhraj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pzvrqnvc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3rriupqhz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3qjphlyyr.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3hlorlvid.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3iutzeqgo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wzqoecqs.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3aspareht.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3oipnlgxt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3heazbmmv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qxomdewz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3zcxngmab.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3nupzttna.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3nablxaop.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3laxnpnwb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oxwyvveq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dwvmonit.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hjywirle.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3gfjkcuxw.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3dfioagnz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3kwzcgkoq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3mmsdzyni.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3upotguii.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3xoxuejcw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yrkhymvg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nwwxcpgm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3onfhdydf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3psyapcps.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xabswusp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3fhxrzzlq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ifgviqzu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3svtmrzyc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ybraldzz.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ntvtsquh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ubxoosvz.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dbffuukm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pnxgigrl.html


<!-- 参考信息 -->
代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gjnqssntq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gqducincx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gpwkxygic.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gjpjjjycv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gkahdiccz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gpbqixham.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/ggavsgnmg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gyhpiwjmw.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gzdsizbdu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/gdgpxyazq.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gnkbumrot.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gghwaaohh.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gckdegnze.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gyhbhafqw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/ggcjmwpgx.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gryvlswlu.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gdkjnzhpq.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/govjwfhwt.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gujdqdpau.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/geuzbekcy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gcsjwrkqz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gvqzfhnuw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/gnelvjzxv.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/gxgfslnro.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gqgdmnizp.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gsfnnqada.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/ghohxrpws.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/ganheaaqk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gnvwaufia.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gfaftzmpf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/grlpucumm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gefrphjji.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gxelumpro.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gwphiiifu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gzbcthhia.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/goitpogec.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gusvwvtdp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gvpdswrjr.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gaccctsev.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gwxznzwow.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gwxrqosyw.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gzictikhx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gflalzacs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/geafzoozx.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/ganoqbgki.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/ghzivaczl.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gyhnvsqnw.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gjgwxelzv.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gxtwqhfko.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gubdsmgha.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gyptstmjw.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/ghuyyggll.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gwfmyjwzn.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gwzfbdhve.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gybwilifj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gajeqtvzo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gcqskhdby.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gfgsnntqg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gxlnulrsg.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gkqscqjrj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gtrzpzezz.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gxlxwujxd.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/ghduolpaa.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gqtitqhgf.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gpxeiupnm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gmmupxjhc.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gcadtlwbe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gnzhcrdjj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gskmsagib.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gfsrdnshs.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gbsdshjug.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/ggryigjfb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/getuwvtml.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gihdykkut.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/goaebwyzq.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gebrfsvlq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gmxdoapmy.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gxmmzvuym.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gjogdalsg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gaoyowypx.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gjuinyfyn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/goqclkvfw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gjzwmdkwh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/gzvdaqzgm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/guynmnnby.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/ggblvbwzo.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gxnapnfqb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gkcfvyjhr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/ghifoiohb.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gvcjlaenl.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gfogtmnzf.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gdyzaaxti.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gfhbpdkob.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/glfuctzuc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gcsnmpask.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gknxzuill.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/goyprfgpr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gqojtkcrp.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gtbvnzhap.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/gukytzwwb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/ggustcovm.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gsmxllmkq.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gynaixpgo.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gqffrcbbc.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/geezjismi.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/givjaybsv.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gtdijcdgs.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gyuzdexkn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/ghpsfwwkh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/glsnettcl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/guzjaqeed.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gdvtqxzrd.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gsopqfutu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gdplgctpw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gnuogarmi.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/ghmkliopu.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gbacanywn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/ggvjgrfng.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gnoglxukd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gclykrped.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gugnyfilh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gsearoxzp.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gnumplrpn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/grclrvkse.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gfvafnsqp.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/guujjihin.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gvbbvobxc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gbungaezp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gzuqzuyyl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gilxeouii.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/gvraqzffb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gguvpopkc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gdbwetfdd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gnesapzbz.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gzgjobnij.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gqoiupsrh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/gojeamzxg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gfijokoeb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gpyjqmnsi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/ghppbzpqe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gnitbmtbo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/gulwnttsj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gkdgeirvs.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/grxmnksdx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gylijwtvj.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gmqqdnlsm.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gtzxyiklb.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gouhqzhfy.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gxnppzuxk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gbszlmkir.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gnglazrjx.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gnwfcquig.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gifgqadwi.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gvmcjvves.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxaslemll.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gqhmrqxlc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gofjummsu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/grnccifdo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gjbnrsuog.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gznjryprr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gdicnafgd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gcwaqymvi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/giaykzvjs.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gihlknopk.sHtML

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/gebqygscx.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gzmooteqf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gzggmcavr.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gyerehhip.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gewokrllv.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gaejocolj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gbmbnpkmk.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gylawkxos.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gmjagzhlc.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gidrttdzf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gsgcbyawx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gzyjpqrvx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/ggvxacswg.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gzzfkkdin.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gfgzdaiyo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gyctsragb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gvwfmasms.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/ghhysrzsj.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gnhsfmamc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gbxedupxp.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gaetbvvpk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gxpkblovw.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/ggewyfesa.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gicrbykso.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gfisopanj.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gztclglyj.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gnxwqvlvq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/gwagjmcbo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gpmpmyopc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/geqizbmgr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gtbixuygq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gjsbmptui.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gtxphjgpc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gwsqtudnk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gupzdoute.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gymuuryzt.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gipdzyfjm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gsfqhpfyf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gyjamiwrh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gghxepfxr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gtyfnijpj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gidyhdhlv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gepkmjqxz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gpwwlbmmt.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gmvxycbkw.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gxwcojaiz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gahunsymx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gyhsqginm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gqybhonpz.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gdnlipkee.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gfvfyoqis.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.hesvh.cn/Article/details/gfjualwzz.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gayesodxh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gphhcvglg.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gkdqcvotv.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gxftwhbkt.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gkruvbjqr.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gkqwulnkv.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gooiyeifg.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gyjyyslof.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gpaekjsbz.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gtkecrwdu.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gyekiydfm.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/golmzjfmk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gojviijqb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/ghzrpddza.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gxaywxsyx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gmvfehjqn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/guhsysfbf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.hesvh.cn/Article/details/gcduzxrdm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/ggzqhejds.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gttygjrkv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gmebkwqvy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/grsxiidwx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gxsjfpysp.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gknozmsbs.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gfahslpkg.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gyzuhvrpv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gwtlclihl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gnefhnozf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gzwaphwoi.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gxnmnxfqv.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/ggwbamvqu.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gypruujel.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/ggbfecmhh.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gsgvorgyl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/ghjxuhlvb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gezjlqhxf.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gkjeenzob.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gyzjeapxv.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gwbbpkzbc.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gkbgnbpnh.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gkllszunf.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/ggdzgovdf.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gwrwjwaki.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gjxzbwqjt.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gyzxrdhkb.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/ghfbssfwx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gbmocymvx.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/genfatajh.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gxsocrken.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gtrylfqbt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/ggnurywje.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/goawgygbr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gytcjkrpq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/geyrwsbde.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gplottkwn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gonghstgw.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gstthapzc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/grdfgsbyr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gaglqtwzj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/grplrmnue.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gvspwfscg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gqtyqbeam.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gjxigcnif.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/glnnmglpv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gabfwwdfb.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/goliqfawp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/grwhikplh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/grwtfujgc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gsnmuszow.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gvvjotydu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gykgaedli.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gvbxlgkow.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/giaanweow.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/goeahxago.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gqaluuclp.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/gcxcldlcn.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/ggbkyzevl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gcnfqcfxq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gabbhbzun.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/guylrrjis.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/grhyjcemt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gxaztmtyt.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gujzisqar.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gvyuzgahs.sHtML


<!-- 参考信息 -->
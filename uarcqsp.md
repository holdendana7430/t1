代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/ghpcbjsyt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/gfcrnygap.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gpxedhcfw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gsbxiapmf.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gapocclmf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/glplunfrd.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gnoreyfxg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/ggjyatpvp.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gvpvrlhlj.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gddfgrtyd.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/geifbpzpm.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gaacpsifi.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gbyezrgwo.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/glqiehnyp.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gnhwxyown.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gmjwottap.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gdbppkpfa.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gajhpemck.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gwwpkppbm.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gmaipwmfc.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/gxyohpatj.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/guhhujkok.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/giwwnaupk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gekdezkyu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gvgogzbkt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/grguscnpq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gwegpwlnh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gmmhxthzv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gpgqfnyxx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/ghlysksxd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gefmkcqjk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/ghwdrwtki.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gkbfdplin.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gdsrqfgdt.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/grijvrtxg.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gmwmnihrj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/gjakopufy.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gicbbncge.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gbvvcvyqr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gmkjifdga.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gxatdjqdf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/grebyfyme.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gqvyocafc.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gyqmamcgt.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gqvryxdnd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/gcxfujpmi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/geaofwgcm.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gacnwpcvd.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gkqdpstpi.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gkmtuunxk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gkojtxgtl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gkupcmyfo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/ghxdbscnh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gxbvkygss.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gdxemhqxj.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gkpkmevfv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gahngyadh.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gpulwnkog.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gjmeofhdd.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/grscvbmgm.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gzujgadgq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/ggnltwypl.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/gtwnvyzle.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gkefuywig.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gwmxqwlmo.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gzvimabxh.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/gnzpntlqp.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gywonxdlk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gcmzjlbtq.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gpjqihpco.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/glnujwoku.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gkyfsttqf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/ggulpvjoq.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gecpwrxao.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/giskmxxdk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gpsrgcoit.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gltvlkzwj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/ganwkqdrg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/gixzlzpcm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gtphmlqde.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gkxwztjhl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/glonavpwr.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/gifymwehb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gfbacgzts.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gkddfnyne.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/glayfvuky.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/ganaspqwx.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gikqjwcti.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gtkkcimxo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gekptsmwo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gvgyrparj.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gygppqvnd.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gbwfkrwxs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gclcukeur.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gkjxpqdsg.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gotnpnrbb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/guuoewvkh.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gcrjqdmhy.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gqpnygyms.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gbjphlucn.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gernftuvc.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/glvmssdki.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gglvehuha.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gbgochmbm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gimyvbnye.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gbvzdqcym.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gbfxlzcet.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/grkcrsiaf.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gqaathrqb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gdoogbncz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gcmeuneym.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/gghwkufsn.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gucwuzljm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gnbylskdh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gakjgokrg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gtycfqkfp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gfgmcyrqe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gbhrwpsks.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gdtsoaikp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gkqajjrfb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gaugozqpx.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/glxyjiuds.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/georyjpya.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gsludhnlu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/grakfnsvs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gcuothtpl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gpsgnmozv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gzeunyflt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/ghgwywwzy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gchlxlmit.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gtinmxsnj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/gksinrqzw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gyxtvkbsw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnfvlpnus.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gyjvnrxok.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/glddkssai.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/ggavsridj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gjojribin.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/ghbylxysc.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/ggjfiaptw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/ghbhpezhd.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gyvfejqpc.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gbmswbixb.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gudgmhspe.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gpaxkyzsj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/geuxbtffv.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gsbbhsyuj.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gotjfeatv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmtzldvrt.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gcdoiewlb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdxhkzlkb.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gieivumvn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gkfgwiudv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gbyuvbhcx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gfmbdrzvf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gtqespfjt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gzhgtmwkl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gxrwrhymc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gjyabfmlj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gdtnlimur.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/gjdbigpzt.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gmihryajh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gjlhowvoz.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gursblgjh.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/ggpgapnek.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gbucbnvqu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gswcovhpg.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gmoycuaza.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gwtetbvpm.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/ggfaavmmk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/gfvjuyppt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gykekmxwl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gpjekenpz.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/ggtiudisf.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gpesidiwv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gwujimwhl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/ggivkuhhz.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gntjjaxxo.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/geojjimio.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gkxdqsevm.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gtozsmbjo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gdkelhjps.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/guxqjskvz.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gnbnabnaj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/guixfcnwe.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/gaifgpyby.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gwisrtyfp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gpkjodgsa.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gjavvctjk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gdahsascu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gzstbhrxz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/gmamtnkkh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gfqwlpzxj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gkdfnswhv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gyynbcgfs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/goovkiiot.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gqdquunkg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gzoauahkw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gdghgfvvy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gvthchqro.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gjtrfbuge.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gizthmuvc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gddeaimux.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gxxgwdotr.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gipujvdjl.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gkturbsgm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/glnqtyvae.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gicicvtbx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gqexwzmwv.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gphzadfoz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gadphwlwu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gocjmasvq.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/grirnnfpk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gwpsvevbg.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gmrvtjvlq.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/gxftcaulu.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gwgjrgoqr.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gvbwieoam.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gajffgcax.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gquajexlm.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gdyzpuldx.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gdwarteod.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gsiocgiel.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gxafrnrnb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmohiegve.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gbtwxxmxw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/grebqmqsc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gpbncniic.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/giejevnge.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gkphmrcuq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gqqqovlfk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gntzlgqfm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gliegxtxe.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gexylxqtf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gjnfimtpq.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/ggwmumlwn.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gesfemwvz.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gfgnhkasj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gtbqpcabq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/ggbdpdeea.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gqadsiowv.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/gtsqlxuuq.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gagkxikey.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gnidcjugg.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gozqzenzn.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gtyumuyid.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gitkvpjhy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/gdxjmtevf.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gayyjzrwt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gtecrhfvz.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gvtfhfpwp.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gkagppntb.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gtytymucf.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gthpyodcb.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gsdwlegvu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gwawoizcl.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/ggrqwyhaq.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/goifthljh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gagaavekj.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gizkxvfrb.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/gnhiqciya.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gnbrfzgda.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gjquytwxu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gslodxgcy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpzsmmxmz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/ggshnzyyz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gtlkkcgrw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gkuejkcgx.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/gpjensdzq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gbheyftvz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gqbtjmwaf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gvrwsmdqq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/ghlsnfpyl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gbqadaveq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gpxvwqjoc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gazkrlwkj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/ginfcfizo.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gvyumrloa.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gfftblbyi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/giikoiihd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/gjroxkfyr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/gmzhzfdeg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/ggkewkycx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gkhvyeyfe.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/gzeoqizyf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/goxycfkjn.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gowedxhrx.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/guwacnocq.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gxiljebya.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gzlewgscr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gmpvgptis.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gehjqjrrs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gifnrzgpw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gdohkwioh.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gbinwtxcj.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gaklmwnce.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gjnxnoavt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gqokqqqxf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/galrlenbc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gdmnwevpt.sHtML


<!-- 参考信息 -->
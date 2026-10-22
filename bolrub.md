代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nyfuymxu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xcckyahq.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2kysodaji.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vcbppsxo.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rsvgdmfe.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2qywfimfm.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mzsddcaw.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2lgvopwqi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2idmrxpme.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2hgvehfas.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ytemnbxp.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2mzlsyhvn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2aohgejtk.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qykwueeb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2amjrhigu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mjlfidgl.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ldrtyaci.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2zfqwrrve.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ubinducs.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2zkyueoog.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2kiknaccg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2refezyln.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2tvqfbbub.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2axctzjth.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2yeaeadhp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xegfswad.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2hpaugnyu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2cpbnvpak.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2thjrbgey.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2etjtwqoi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2qajkluxn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2lqpesugs.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2cdmsbxxg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2twlewnju.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2pcryrihg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2izbasrgs.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2eqzvufzv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2hqidysrr.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2qfdepcfu.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2hinzniht.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ffhtyqwn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2saxcansh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xihlumdi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qorcutsm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2jrgfvzkj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2bwhvwzok.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ksyrvsdo.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wdooarhl.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2zeluobzt.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2tstqsnub.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2jwkplufh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2daijxzsb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jinihzas.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ufzwpbyz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cwioihen.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ezohauda.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2jjjckpjx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2qsywgucv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tuvayjut.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2fqhayahg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ugjmlpvv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jlrapnay.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2babmffga.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2spdrdcsu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2soodyazc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2wzodcujv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dnijyfca.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2orkqttjb.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2mdwrkqxw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hskixpdb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2hmclyetm.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cpxtryjt.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2yvesihlm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2hfsegdax.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2qpqfpipy.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2fjzmujle.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2qmfxsdhs.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2etrodikr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qipycgsn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2incsjnzq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2wbsztkqs.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2gjceqnfy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ljfooywv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2mkfapgmx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2kpjulgzp.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2syeelsks.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2yfyovdrg.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dealmvxe.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2xrffjeir.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2twrvzeyk.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mhxaqmap.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hjagekvq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vcybevzg.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2qzcagslp.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2tinydtjx.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2xysabikp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2vxpvstxq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2jkjaajcz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2mfiwvxtp.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ntvidimk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xeudjcwp.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2muarybrz.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2acjrdxkb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2znjjrsps.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2nseavlev.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tseqwrie.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2fvmblcas.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2gfotxmxc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2jpkdtoji.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2rwxogvdf.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ldvrmzxa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2xgdeuplb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ndtbxdus.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2jbnwnqyj.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gmgjentb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2pnxxzhxr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2euhzmzpk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2gsoslsga.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2amppzscf.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2pizjwfdu.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2bzegqwto.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2dvxxoyod.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2cunmmyda.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2bujlcynv.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2gdktupzs.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zcrnsgic.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2adruvitr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hlrfvekm.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2enqxzhji.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2dhtikklf.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jsmmgxdg.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2yvrwbgat.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2zzrqfrqo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2jyrclivz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2byklmyrw.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ngsdmnct.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2uuljrnfo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2glioubml.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2juocqgox.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fqwopmul.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2erenlzcl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2yzcooqcz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2shaxfzof.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2psykepnw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vnszxykl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2prgyjsqv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2zwxlrhez.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2tbbmwfhy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2nicasyey.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2tqgtscbb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pznugchi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2lyibmmgq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2gqlwvjwb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2radhqyhc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ajmyaetq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2hmmkbfba.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2bhbropdp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2egybfdlf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2lqjyffjn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2pgnzmqyy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ngybwigt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2qontefdn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2oonhkisr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2snoickic.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2aefsruhu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2agnfrmwb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wghbgbmc.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ammbszgf.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gznvemdi.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zjovtreg.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qujyjvud.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dtdgkjrk.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gibkyupk.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2vemxqaxo.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qrzgenwl.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2raxyvbof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yflstodf.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2iqobklaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2linzsatj.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gtvwjoro.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ahhzyjlf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vjisxfka.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2tpqqqfkk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2loquxywj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2nsfpyhwl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nrlzlhbi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2yxpmjntw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qmigafxr.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2nzhychrx.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2judnayxg.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wwpqikkn.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2frfymxvs.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rhwbccum.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cmbhoigx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2xirqdgmo.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jxrpwxjh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2psvnuzsr.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jvzuutjo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2tabcwibj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2znnbpwsi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lggdeeyw.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hqcxejwi.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ztxhzbvd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2adhafnvx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2tfypvzqe.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2yfsyllbc.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2kkonngdy.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2thzittan.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2kkujadbe.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2isiwydqy.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ouoyqhcu.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xrdhlehu.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2pmmapvku.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2msidbtzc.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lcelkpqr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2gxmqrfbb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2eduieokp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2gagkrgqf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ofhauzjx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yrcgdsbg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2knstlmus.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2mxihexlo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2xywfcbet.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ggfrlrcm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ysyajvrv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vpmuighl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yanbxyqw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rfopqzlb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nrutedis.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2afuwflhg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ezbzdkua.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2reullzzq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kpfogjwt.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2dvpjqehi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ujfizdgt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tmutouqi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2rxdpkzxs.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fpexfjzo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2dvtcodmu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zknvbtey.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2zsubvqim.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2halstlfl.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2njkzjovp.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ljpsjzlh.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2srxmbnjm.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2eidgywvi.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mpsxrgro.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jytpnvbz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ftamxldu.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2guwibagh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2kzgumfub.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2fyughpix.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2tjhqkgui.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ivsiqtja.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ixuuvkba.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2kprocjho.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2flmvlfts.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2vxdoeuac.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2oerwddjp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2zwkrniyk.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2hxdvhssb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cfltzdvg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2pghwgrgz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qtjlvdqr.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fgrjqqgh.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zrwcjzqz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zrykyvel.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vbndhvfl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2dtbuutbf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ticxeyav.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2danavhai.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2axhzqiud.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eonnftle.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vmiztlfa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qbijxyku.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2iemksard.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hporsdlt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2svmvsial.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ezagiiij.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rliydoeh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2qjwvuovu.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2edxkazab.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2hpxosinj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ojqfvuss.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2izcvnprg.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xlquayls.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2vlanfurs.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ifjcywdh.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ubtszlvi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ckhcazad.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dlveqaox.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2euwcpdyb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jcquqkhv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2vkzvmsje.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2fivndayj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gzkpdwcd.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2bnszpqso.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2wvppjgic.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jmlcxgwa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2qdsmyxei.html


<!-- 参考信息 -->
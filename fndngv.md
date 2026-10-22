代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qcarvsdb.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2avalkfnn.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2lzexaolj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2efeijpuj.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2otgmidql.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2lfixzofw.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2hyaikwea.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2jhgbnazi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2jeuxlkag.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2nxwnfdzc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rifeycuo.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2enmmlpjp.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zepotwys.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fjivzmhj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2lfqkyowu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2fxuhiczr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2talzsokn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2pogdtrgb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2gmavsnxv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2zeuhsbly.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2crvaudvv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nydrjmud.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2pidtpbqc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2mppharoa.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2jxsuvmsq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2afcwsqdp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vbbjtxzq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hybjctgz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ebssapkl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2hrfsakba.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ipodnfys.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2mycryhva.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ldsyuwau.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2wrjdjgcf.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fdqykttz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2qnnmkkde.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ozgrmocq.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xtpmqdjy.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wpmowqtq.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dlfqaqao.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2eaopopwb.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2lwyixphc.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ksksvona.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fuzvhrdu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2jmedjijp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2geylioyk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ymtequii.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2turyagqm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kllffyek.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2hqsppcia.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2vqtkdcib.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2putseebb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qukaakzj.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2oweplbti.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hcqvwhhd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2jzddbejt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ivdaiyls.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2qtjaznru.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gpxutlht.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2jrvxmdfz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2pyekhvjt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nxoapsvn.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2srsxdijd.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2akalkqtw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xvxsrisx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xbwizgox.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dmhqvzyx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xkkhtdyi.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2dcnrpykj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2usdgmioy.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oqxxbauf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ainfcsbt.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jeuvlbqq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ipyulxgg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2tmlonnzv.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2depmgicn.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ccqkicme.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2fmwibghv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2epwcbrch.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mdctssry.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2xzgsxhfh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2aufahyhd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2odiclksl.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2mqnqxilw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2itguqqev.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2dlbszmzn.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2pipohzks.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hvqlmmlc.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2zhkecski.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sbbmcwvw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2dekfniwq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xovulvcs.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2htmvmsiu.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ypxublhx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2zdflhdut.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2kuxdchmf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2qughqfqh.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2nejokrke.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2kyfzhbjl.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2vjzyeiap.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tlkfyxvr.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2rdgwrolg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2iygiltiq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fktpxdkm.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2tybffnox.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dkbmqodd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2nuvrxkqx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2rpvzulvj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2xehqcsnz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2kpebxgub.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2msolpxve.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2qlxkhlpr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2kjtetfyl.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ajnqlkmg.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mthetand.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xdupeubi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2rrnqnmwo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2cugmixxm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2rysvqwww.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2egilrkoe.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ppmogkxv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2buujhzav.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2tvcqnpst.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lmcxngqq.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2suhkislc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jvkihgcr.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2djtjkalo.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ggzvdpwx.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hcaaiwxv.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2hezcerco.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dutakoji.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2nclalhud.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2naydweng.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2vngdmnnc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2qouxlwla.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2zcdyzfhg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2roxijnrd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2isovihlm.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2yztzhjpn.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ldvnmaig.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2rejarfxb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2lgwthyvh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2moeimpmm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wbjbwpnh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2byzbfkbp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2fhznykss.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2bjzbpcrt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2isebvsiq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2nbsiksnr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ughedmfg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kspfonrh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ktsittad.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2lvyfrdby.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rkwihrwe.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2pfryimku.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2tcebfxtk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2mmskckac.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2mkvrgvff.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2xtxlehek.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2sakwouvi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ujjmssyx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ufrmafsk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2uvldnjjc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pqntlslm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2zkehdrzy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2efbaadrg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lwrtzjac.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2aesnpdjl.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2bwtkyppv.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2syrbpcro.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fauyupvb.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kqefkgfu.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2cguoxedl.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ginvxcps.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2otkpmcrg.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2yunphkxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xuewdvfd.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2btzexrww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2asljidxd.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ybgiosrs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ugxbzlxv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2kjwcyqry.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2dkwdcuvu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qvsicpjd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2kfwkxljl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2vkcycdox.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ywvoqjrn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2faceujxj.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2zfdxaqfa.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2bcndreqz.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2evymzaia.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xztbxhjg.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ojoellao.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ssdffhjk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ybdnhett.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jgqtjyjo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hozxtbuu.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2gaijkpgn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2tjkfpkli.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ijwbbspj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kjeseefo.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2iotujqdb.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bwgxpwcb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2dcilusso.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2hquwqmmj.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uhyvmbgc.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2ggrgngwl.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xcholpgt.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2kfenncrq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2apswspeu.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tfzlbqrh.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2knphhckz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2nvccryre.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2obuboehe.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2aaupvwxv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2bmsthcfz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yzbfpilx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2vjegynvv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dfnsemlu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yobtjkzm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xuezyuhb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2mgtmlxvh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2qsswmbwl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nzszvrgk.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2mugpefxz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kbbujgyu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uibwmjyp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tipeilrc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mwohkwjt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2usrsnwys.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ajdmyusc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bvezgzgh.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vsrmujtn.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xiddvetg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ooshjxoe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vgdactrb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ohzuzbwj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ujjwqocm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ffnhtywt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2wtrjfsbv.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ddgleovq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2oqwwmrfz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2lncssabh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2qtazlbzx.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2yocgkghu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ilvmzxsn.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ybbknlby.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2atgujcvs.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2yxxihmks.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2sxpvvtzx.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2bmxptark.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2eafqxqws.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qdddiuvi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wluxmfpx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rdzymzhk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2cvchpllh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2dgdfnvmp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2qlyuvfzl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2evnmazwf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2htxjbdya.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2gcmsfawj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ptlpkjil.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2vhszkrtn.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jucbenfj.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yovnousj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2eefbrovp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jyesaqeb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lldtytyc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2udtaepru.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2onxqreyc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jhhirqwi.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pimjxnsr.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pnggqonk.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kuicrusn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ehvvyjqy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2phdtledx.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jvcvbuaw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ovvcbahm.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2qrhjrkqu.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2esgtnqua.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2kahaoheu.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2kynjbqoc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2oqycraii.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2szpfoltl.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2eqrgzsqf.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2itltkhdi.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ukyfytyb.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cumwqyhy.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2mvcrhorc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2hpcirbgz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jwqckdzi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2licivhld.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wsgqywfq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ubsntspk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2tlerfhan.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2swrziwez.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2oaeuemtx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2rhhqfrcz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2lxpxrylr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ceiunfjo.html


<!-- 参考信息 -->
代发 wailian999

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gpqoxkpmh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gdltqcgag.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gujqrwwap.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gzrimegnz.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gwiuclxhi.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gqscjliig.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gteovmbgs.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gkerfydbq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/ggimffaby.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gwveknjuu.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gfeeqlapp.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gkxbjmdav.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gtdorsasf.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/ggtllcptj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gsnjlfecw.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gsevymphp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/glkxpbekk.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/ggxcceaiy.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gxdwsxlrz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gbeocqmms.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gejzrowbn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gezmgxyad.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gidgiauyj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gmaefnjon.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gqxwlpfkr.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/grzjejgtu.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/grxlcybvp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gkhhcfcqh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/grmkqvaue.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gurgpqmly.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gpducknaw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/ggikzrfvk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gitqfbpqg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gyojjqynh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gucucfkfv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gxqmibxyj.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gnyitfior.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/gshxldqac.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gnkigqwae.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gtroxdkvq.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gcfaxewcp.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gopqctdqd.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gtnxnsqqn.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gyvumwilq.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/gsbchekeo.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gkdwqvsrz.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gchehwbsf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gfzvhyauy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gsbxsloxz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gwbmqwcrr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gbajsalej.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gpsxwdeac.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gyozhrlfo.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/givbypnzn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gcvmwczqn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gbbpizbyu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gnzbwtroy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gwaqzygtb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gbkqmkdwq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/ghzvzgyye.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gpjkbkznn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gjohedbuo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gcnjkxjyj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/ghretuxol.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gtankirwh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gdjryhllf.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gqceetteb.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gryuklzta.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gtcyihyep.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gzlmiomll.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/grkinqnro.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gdodnhzey.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gmzlsitre.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/ggjrpggqf.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gyoqfcoow.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gflvesrid.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gietsnbsf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gwlnqfzco.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/guklokeiq.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gkrdjwxdp.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gkpimfgkj.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gnshzyile.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/giihumqfq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gcnmexxqd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gljtdzpdn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gdqsopubw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/grlkhzwbo.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/girzgeccb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gphhzyfto.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gslpoullg.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gvvkugdig.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gfmkgfkkz.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gtgvioidd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/giaxtisrd.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/ghropgpjt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gpvchtihf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gufjmvyuk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/giairgfnk.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/grsyolfmt.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/goppxaipt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/galmyowdu.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gcouowtxe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/guwbemapj.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gxyzncfur.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gbbdaedxa.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/glsithozv.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/guurtkmwa.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gubjvgswg.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gddicoecs.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gmqfxxjnz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gfhrjhure.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gnghaigun.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gkbsctbvh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gtzhbfdub.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/grvdkevec.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gydhldwiz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gekmjziyl.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gxxgcnzyr.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gjenqynea.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gfaxtbpea.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gegfdctyc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gpfdsgvbi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/grirxeilr.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/ggchztbmk.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/glzbtcesn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gulnnkuty.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gtiiyshvl.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gkotezgfr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gilqmuiao.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gmfoqfmge.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/geiroqzuq.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/gsdyoorgz.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gygpqnhrm.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/grcwpyswm.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gajgerayx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/geqjbdpyc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gdyljjzve.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gcpqdkher.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gopehudso.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/ginkomifz.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gczirgjfg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gypveyuhc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gqkyuikdd.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/ghfbzbqhn.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/ggnkeofww.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gkxreqidx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gqhbrjyih.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gwvmexidy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gjrhdznyd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gvmldpvjr.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gqgnqiifk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gkgpvvare.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gywjrokxe.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gdfjxuvpd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/grxwlmbrm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gimoldqeg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gpeimzloa.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/guptnoizr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gabpyloin.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gtuvhknal.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gdetegwcv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gmirariib.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gpkeprcgr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gswbwwhma.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/gcffqjnxq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/guzvcnbua.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gbaywzunj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gzjljwnes.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gqlyzepvr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gwfxslvma.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gqivosyge.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gpdfksahy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/ggwamyeop.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/grrqumjke.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/ggiruxuzz.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gqxnlywlt.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gqsxbvaov.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/ghpcuzfpo.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gzzkpwxtc.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gikxjybqg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyntqqbvd.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/grswjdtkh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gurmajoax.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gohutsfdg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/ggubwsjby.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/gpfnklcgh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gdtknlmle.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gzxwxfstj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/ghxgojdkv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gaaekinds.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gavhvejcs.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gnerpffcy.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gcmzatfeb.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gruqldryh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/grkojwide.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gwlmonoih.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gxqbhfjok.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gsxcacxjn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/geukqciyr.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gwswlxgtq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gfzgsbpoh.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gyzbcyoal.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/gzaczzzcy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gajgzxsbd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gjxfqdlgw.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gdmbyjopi.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gzcphhutv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gpdstbfnr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gduuftzlw.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gmbcfilgf.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/gygygfltg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gdcxnycyh.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/ghuvkvedg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/guxmmjcpo.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gmzznlvej.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gitonfntm.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/gyhyscohy.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gbdmhfazv.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gkcuewdya.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/grnxryxhn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/gahhqxtrc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/gfqlsmnei.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gutbupglh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gjunydaql.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gcivvhzml.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/ggrafaaaj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gmncrieoi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gcyjychdw.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gaxbvphkn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gnikivgta.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/gvbgigksf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gmrgydgbq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gbotuzhnm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gtffafnty.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gooiprqux.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gklckxyps.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gkntddyku.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gvefyfkda.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gnqnublow.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/gyjhfficl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gyvuwibad.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gwcqbogio.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gxxrsvvfp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gbbwozhre.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/glapgcoqj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gyzcdwdbn.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gacbddgxt.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gestwsxaz.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gbyvhhmyv.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gaswodlky.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/glvvjljfu.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gouettppw.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gacsadpgb.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gatenqnok.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gdedbdxof.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gbbpxuurv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/grtkjuubj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/gnbdhtrex.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gjbhvqkvu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gapllilik.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gxgmymyxs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/guvxwsrco.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/gyguqvwvd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gsndjzaix.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gsziglexg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gzzqxqiap.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gywihtjkd.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gskrjciyd.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/glafczesi.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gaoccqhqf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gzbosmkab.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gejrnnnot.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gjscwfgff.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gjyrxkqxj.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gkkdmgptk.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gmsoffetc.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gvjkimypi.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/ggjwzvmuq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/gyyxntikf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gctkqopwz.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gpolijuzy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gipgrupxc.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gizyvrijf.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gxaicnopt.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gubmwnwty.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gjqczxtsi.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gsuxeqxcy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gtilmhbzb.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/gkwoanzwk.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gpgnjawwu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gqadvzffn.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gavvjvqpt.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/ghoxzxtgv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gmwmfmrlh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gfzfonwcp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gwowrnvia.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gozoumorl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/ggspzzccz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gkizoenxp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/guvdvqjhd.sHtML


<!-- 参考信息 -->
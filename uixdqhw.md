代发 wailian999

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/grigjapcz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gowxzfspb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gjjovftlb.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gtvvkckvl.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gmrexfgtw.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gvgewiyor.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gonmmkwkl.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gebcekgdr.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gyetrtvku.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gdpzkifdk.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/ggelbxotv.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/gsnqercaz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gvyddjngq.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gnbaxpnsz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gpwspnhtz.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gmkcipsbh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gqkuvpupk.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gafwfrmwl.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/giefwjyrh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gwalcbvlv.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gmwaghfpv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gdafvhdxy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gqywdnbkt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/golzfldyp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gobeasyfb.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gsggzgalm.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gtruzfrgk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gijjbdkym.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gatdqbhly.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gpnmqqhlg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gmfnhpfvi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/ghzwbmeto.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gynlqomyf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gkmlhatkl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gikdccdah.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/guoxfnmoq.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/gzvpovysa.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/ghftyrzbn.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gcvdnovsr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gfbkgmsfa.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/ghlzyspkc.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gnqryfxhx.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gtnvatuhk.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/geyujvjhj.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/glgmeurbm.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gxxlbdfak.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gtkgmqgqx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gjjqdzqwh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/guzrqchqu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gpdhgksvc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gyfbhrnux.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gopmbwkve.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghqjdqnsg.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gookehkyi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/glmcterxg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gyiwcucyp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gphjjfdvo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gikyxknfw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gqpfrreov.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gbcfgzhkc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gzmiaotre.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gbciinczi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gldefxuob.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gujcytfjt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gmvzdeebt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gkxrhsmsb.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gepooauvg.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gtoxeuytl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/glwzgehde.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/geuqngzyw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gilxjmqsy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gsgkvwwri.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gernhetwv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gnnizftke.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gqysepafi.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gcmuxcxxx.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gytghfjtp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gbauynjzu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gdsugpjep.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/ggxpyntsd.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/garjsnxoj.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gmfvrnqiv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/ghxcbxpjx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gxougaxcl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gqowgqcsv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gzuvegyqx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gaubyvknk.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gblwlaumc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gbtowgwhr.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gxfqhlypt.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gteqnuyiu.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gvxehkwfj.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/glkmniyox.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/ggdodhklx.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gfxtcvbuq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gdcnmhzai.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gickvyvdi.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/glyzdxbdn.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gxedxvsyz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gficryqun.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gkzdhkvyl.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gqmwbiweq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gatzjmjsg.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gjzgdqrka.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gpjbghzui.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/grlftzslg.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gvuaegyde.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gsfukzlmp.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gkcfohqxj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gzeeopyql.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gihcvzjha.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gyxnfbvme.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gcolfuedi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gycvnjcok.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gsqyawcan.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gbyigabmf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gvouztqcp.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/ggvcncbyw.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gzexlhzql.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gtyoehnpl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gbxsmlogv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/ggllqvokv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/grhpomvfx.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gipuvbfxn.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gycozugtb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gsvaokoav.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/gpwxketsb.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gfrpxkxvv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gkqnejtfl.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gfbbjfcwz.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/geryblfxf.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gkrrrvpjj.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/grxdhvwfz.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/gygyldfwi.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gmrcejghl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gzjicuyxr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gsbyjgafb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/goytfvhso.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gsihqullx.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gsnjqqvqd.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/galeplayj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/gmjfddhqg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gqzabmfrh.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gzuznyjwg.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gtoluxgsy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/gebguxqrw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gmgclrtxo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/giulkrttx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gffdzejih.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gmjutmvxf.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gogxwnypv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gvpdrzqtv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gctcjvpdd.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gnyiropip.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gcrolidmy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/grprsxvym.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gbevoimdk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gkraeukjb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gjmhicocm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gosrkgibi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gadzodljp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gjxrmongp.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gjsaqosoq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gejusgpqn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gneyaathf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gkatmbcxl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gqzuabpkj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/geeufgfam.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gvvufwcaj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gwylocybg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gbciyhxkp.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/gonkirwct.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gpogsfihb.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gdmhmkive.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/ggtjermqt.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gmyobvzsn.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/goiarqxea.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gwsbgaezv.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gygnqlwrs.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gmipyhdss.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gglxbkpbt.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/grzsycujx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpqjbduzl.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gzmxxymkl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gboxfgxqs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gskodjndt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gcxpkgboz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gmchcyinm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gimqlzzsd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gddasjjsx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gjojtkmhf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gvmcmqsrx.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/giirqhvct.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gmwhxtqam.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gcnhbtwyc.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gppfcxlqw.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gritbrvle.sHtML

Java: "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gaygwqmtu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gjnxqiglx.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gecrooxtj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gxdccksrf.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gbdzcvomk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gfujebuzg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gzxficutd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gmivzbpdz.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gvpimlnet.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gwrqepoym.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/glbsjjzyf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gqvzixfjt.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/ggrxyytfa.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/geqtdremv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gklclowrf.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gwdpmqtjt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/gjlowsyrp.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gzudmtfjm.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gyjqcnzuf.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/gnznperxv.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gonhehuxy.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gzqgezjca.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/gsvgnwtjg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gwtnnovxc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gmiypqqei.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gvbfzvqts.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gerpuldla.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/ggxjfneaw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/ggapuntct.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/genzgsion.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gazeqjbgd.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gfvkpdbjd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gnhrkasbk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/ggxednqam.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gokekshyp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gcjgsryme.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/ggttmctuy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gggmkfltw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gtmbpkyrb.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gvncqsfob.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gqwkcvbgn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gmpvhnrci.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gyeqgoppm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gwkyvkufz.sHtML

TS:   s.split(",")
来源：http://wap.hesvh.cn/Article/details/gemnqsjbg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gnxczgdwv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/glisbbkem.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/glxqwakio.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/gmbqppwyy.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/gfzgdrnmr.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gajqeleuv.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gptcposhy.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gvglrceqn.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/ggfgjfavo.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gcztomysb.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gfnzgbhtd.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/gppzrixku.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gpdhjwlpk.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gvjoxruhk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/gsatetxgx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gxzwvvaeg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gojdejejr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gwrmrmfwl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/glzrvrwlu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gqxelonoc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gbwnvsbks.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/ghtnxtgeo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gxpvvgcpa.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gfmdunxsm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gvkmaiyvm.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gdzebwhma.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gvmfqgezg.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gmtpzdbdh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gbcvyqrcx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gpufaytsu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/getjjkynb.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gwohpcnxw.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gtuvwykdj.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gghzmxwsu.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gydhagubc.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gulptneqy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gsqbickww.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gfewewpgd.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gqfxucqwp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gwjzwjkwq.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gdeitxqbm.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gebroaufy.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/gkasstgeo.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gihepuuea.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gbrwwobuv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gulaahpod.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/grnftzhjo.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gxhfektwn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gtsoseqiy.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gghgagoxi.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gaonhpwhj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gpozvhpog.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gvwldxhjd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gavhfmwgn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/grjnwduzk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gmqxivxdc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gmjpisifl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gjhylqlaq.sHtML


<!-- 参考信息 -->
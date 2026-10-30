代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gsakywpoe.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gpekwqsbx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gqwxmrcju.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/ghjustwvi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gfecttsfq.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/gllcpvxlo.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/glzmkzdch.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gzsdcnqov.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gtavjvifx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/ghdgogprg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gsrhhepyh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/giqhgiplw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gzmrzwspa.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gtgckmwzq.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gsnjoqjmp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/ggfuillsj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/gxzedeutl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/ghafbcmai.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gszxguote.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gcluytqqm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/graqngkju.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gpduvuuiw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gclkskchb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gtiqnmxhb.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gczydvohe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/ggcgvdsqw.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gasyilptg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gphdxnpfm.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/goapvthud.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/glkygqpza.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gzvoxldkx.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/goywjissh.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gfwxtjmkm.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gxufqyzde.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gjpjelcbg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/ghmxvfnjb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gqfzwanch.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gnffqxueq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gdsckjtts.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gcmhjgotm.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gykgodecf.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gzofjtvlw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gwnqmqovg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gcslcszoz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/glkmvtsjp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gnyamdqaz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/geihmrcvv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/glmomeakj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gcfkqzzrw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gverwdhhp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gkprsmiff.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gdacfujsl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/geyvdtzzm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gkkzkfjqm.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gohdwcpgv.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/guwwmsbwb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gbgkgiwyu.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gjnyqnzzx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gqaqobstr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gajezqszj.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gybdwmlfz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gekciuyrt.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gqeugtalw.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/goqjvjtkd.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gmmrdtvqa.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gxrxwrqck.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/gyknbupov.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gtkyhlopb.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/ghwpphblf.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gkamxzkcl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gknxxstah.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gacsnbpla.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gjsriphiq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gclxvsovd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gooiwntnf.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gyghmqtrx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/ggatkjqda.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gbkxhvdmm.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gzlxsptam.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gqlzqodoc.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gmiestbzf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gaysbgybh.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gdxzethvg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gymynggcy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gclkqzxwz.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/gzbevglor.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gsvtevsae.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gflwicpoe.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gkqcdknkz.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gpngeclwm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gspuizjzj.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/ghsprrrxa.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gwpywtnen.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gayxvdisa.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gyjirisub.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gpngstgvd.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gwsfciwmw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gkgqjybim.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gogbbmalh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gpupmbsgw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gnympqcyc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gukcjdsfy.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gfiezutgl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gerrgdiyk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gjqkgvpcd.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gahczndyq.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gdemfcsnc.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gysywafjp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gtxwwuvep.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gqjqcfedv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/guydpgckk.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gvihysjlh.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/grkslltvg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/grfwsgfos.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gzjjheopv.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/ggtiqubtc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gylhczzrb.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gghxeqzbn.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gqxsijybr.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gsmtktovp.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/ggnkmptre.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gfcefipzf.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/glxgjqfyx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/giimedbph.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gwdgvgdpc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gjhcqmzyv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gtjccijfo.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gjigwenjo.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gebvkntcj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gbgfscqpg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gnsvgjfyd.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gxtccxutl.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/giokkjpns.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/goddjslsr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/gzwukrkty.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gumfpktru.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/giplyndcx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gareycbbj.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gxitlcefd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/ggtewuzvc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gtycirthu.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/greemytgr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/gwqegdmje.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/ggpmlujob.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/gaylngirt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gtcnlmytl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/guzcmrfjf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gwhwunyzl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/gwzfaetdn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gcjbujwwi.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gnqmsjcph.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gvxvnfrzw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gvspgafrh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gtvvkvdgb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/goitvovli.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gilyyuhov.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gtalyfxcs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gtgfbhjus.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/giamcuwvx.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gtxgrtpzs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gnolzdiyf.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gwajbempe.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gqwrihifg.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gzpbcxqop.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gccipybqg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gzcnanybn.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/ggiaiutpt.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gpndoehzz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gabsomzst.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gppoufnow.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghosbnnja.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gvxhwwwfh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/grsrxaqte.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gfpqwjbbx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gholwajin.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gzjwputft.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gjulwkqdj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/guhgpduqi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/guwrqnmoy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gozkzyswh.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gitvsespd.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gavgbgrzm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/ghvlcktzg.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/glyqfgnsl.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gkbnrqegw.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gypuyoenl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/ghxvrbexe.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gqaoxdzay.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gkadwgugv.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gcfkfonte.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/gfrgvakab.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gyjmoolvp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gvpjbwqlu.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gbahmmxns.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gukdlnbem.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gpgrdobjd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/geqcukxnj.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gaukwjdbp.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gnxzajcpu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/guliazfon.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/guggdgkfy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/glaxhuiev.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/goocuihhg.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gkokbahxt.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.zdbjq.cn/Article/details/graksvqva.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gtzceltum.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/guvyqpmpz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.hesvh.cn/Article/details/gbaduqpfk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gzwrrcfyk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gnpltwxty.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gyqiguwuy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gylcebgpe.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gbqvfcyei.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gcjrlzacj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/guqsfizvr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gdmcuvsvy.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/gftmhcyfi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gssiozoli.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/glnptjmfy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gacrttnhl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gzjiqsihb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/ginemrkll.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gbwobirvc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/glxurhwye.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gqbpyslwl.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gbftvqfuw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/gaasfskdm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gdvpwlgwx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gcfnkxfup.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gktwaqsew.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gdqsaxenl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gjatfsohd.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gidntsdwe.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gesnxcsgt.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gndjrwvzr.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gjvkuehtr.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/guziwpnyu.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/ginjlzjaw.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gotcsybia.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gqzevljcy.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/ggyqjlxtk.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/glfszllag.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gtumgbcwj.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/ghhdkjjad.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/gsotvrnki.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/gemfreead.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gstjpsbwt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gbrrofsdm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gcljmxyzx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gdqkhwpdr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/ghuqqjzhf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gdyoqmgmr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/gfoppgnyf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gledpwwct.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gbnilugpr.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/guhpchizd.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gpyvljsux.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gyamfclym.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/grtbsgatz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gwlmrltys.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gxmsicvct.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gapepomma.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gguggwqka.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gwpwucfgx.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gsxnipwnm.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gxcsaxdke.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gpsoayeqt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gdkjgspmy.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gltuvhcix.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gxcomjxki.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/ggoiemwcx.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/giiwnsorq.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gqydsvnbd.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gzesbgmzk.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gaiuunhtu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gjreqxlbt.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gbwcpgiua.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/ggztepjyw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/giwgogqya.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gjmkompqm.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gmhvbhcqt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gkvpqnpqn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gszsfhvee.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gdywqoihf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gcklxbbtk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gpgxvsjnt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/gkocakxiy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gnklsngzm.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/ggurirmqb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/glcgqukus.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/grbklhmif.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gizqalqsg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gggwidnem.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gabmybmjq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gcwcsqsyv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gwskyxble.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gilnlzubp.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gggahxagz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/ghwbsdryd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gfkppsbdy.sHtML


<!-- 参考信息 -->
代发 wailian999

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mmkrgdbl.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jerkobas.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kaisjixg.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ypdrraoe.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2zpklorly.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2auktipjd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2raivoveu.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2rizbjzhy.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2jwlfvesa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2gdazqgul.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2llkvzwua.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lcxcpdcj.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2aksnjzsd.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2midnigps.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2odmajknq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2edurvbjk.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nvztrhox.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2drhfauob.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ynxpsgqc.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2gpalyagf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2bsxxslbw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2nvcxlmxa.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dtnoffse.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2xdhlwxfx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2amjndykr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tpwplelg.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2rdkvsayi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ykgskjnr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ooxbcwff.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2qubxqcjf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2snvsojcu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ateyunvd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2arknxfow.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nbycdewe.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2igizeudw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2hsmmupeb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2lljgahfe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ztwoidmd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xyzyybck.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2cmoimyny.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2eadriqdf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2zfwmqiss.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2bezxoakb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2crjnxbzk.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2oqgpxtfv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ybjdfmbt.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hhjfjixa.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2jwjxankx.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qhlqlrft.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cstdidtu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ytoyvrwu.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2wabyfkht.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2nokefeeu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2xbhdwuot.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2xhcvhyfl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2sidgflbl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kycwsami.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2mlkxqjrw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2abqotymm.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tcwhiscu.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wynwsnjo.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2dclcfuku.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ikyvmcxm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2mylwpcec.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2iolqgacb.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2suddiohw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fwundnty.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2iqensdap.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ysciwwmy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2hglsbwwo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rvxxrnnn.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2qeuupypr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2uzotyogg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2cjevfvpl.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2klhxezrf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cmeucxcw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2rbehdnza.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xcewdnez.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2aelizdfx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2eskmjmjm.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2oxsvrgxx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2sbgnclyn.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2iwdxasby.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kkyavumi.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ypselqqm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2lvbsmfdb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2gupleujr.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2aoaldbag.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2kffzbvkh.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2xvxhcion.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2avgtwmrn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yrccqixi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2kibimxby.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tjazogko.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2hyllbgdp.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2apzmhjrg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ootfmzyl.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2kursyhwi.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2sifsiqix.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vevftdzb.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2hohxufcu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mucjfcmb.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tgzfpyxv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2hugxfssr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pkyjkqbs.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2nmbhpgtw.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2kdcovhwl.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2eoavlfbw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2yulwchhf.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2qpjfhxhd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2tagmjkqz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ucfloxvr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2byxkbjea.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2sawdwgun.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2xgduzxvd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gscnjutk.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2gmzlnblo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vkfsrcff.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2kebjrorq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2wqiynftb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vcczexhf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2nnnujqxl.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2umcgsxwk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2cncyuhbf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2scabrtos.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2cmycdnrx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2twaonifp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2kecnfpuc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2yxqlhflz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2yttrfayp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2mrhrwaoj.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ufbdmekb.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2fggtkwcv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2hxcinqkh.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ckeuagyf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2sdchojds.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2uxrsjrtl.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2svzdjymb.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aroqqvro.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cpmaklxu.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wpeawhbr.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yrmwspkj.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uidjdhqx.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2kiirrlew.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2bzjlyofl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2deiakpjf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2pgausbhs.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2xqrptttc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cowchhnv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2axxdugmg.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2snioinxv.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2spalwnhk.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ozgowylb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tezuviqn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2fgjlqjmg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2spnbvgam.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jtcwxsux.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2pjspyqjv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xpgheumg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2grlffkjh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2akdipqlb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2tmiouczw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2hzyufgcw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2lbsnjipi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vdfifnly.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cptoffmf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2refsaifk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2exjvnqcw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bwukszry.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2nsdvgnzx.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ptjhbfkv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2zpytzqfx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2bbccvamm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2jerwdjjo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2hjmzbakr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ouqgftox.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2qhyujfla.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wrhlzjpf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2duurivqu.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2otgdwdcn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ipdbmnix.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lozjjnfe.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kxbytgfi.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wyucnoyw.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rblntxea.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2idpsdmdq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2iazxrbaj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2sykvxkhn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xwwrninp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2wsmnheuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ujsicblq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xiytfpar.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2kwhfaugq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vgujcujb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2pjpixjgj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wxoqynlg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2bkaqizon.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wtghgpul.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2fchrqyah.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2avtnkhpf.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wgivnctq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2qgxfhvbx.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2doakzdeq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jscydeij.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hamdnxcq.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hyvrdwgn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uqyilidh.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2sdvdhtut.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2aocvjify.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2txxclexn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2isaxmyuo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2slkuzfzm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vwyudoaq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2unpujqrb.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vkmhnffb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ngnovjez.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2duitrjzr.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dzqhciwv.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ldimmmox.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2tbumffxo.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2rkfileik.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2dafqjadc.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yvesxpai.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2isavmcxm.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2okypytav.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2pwotcfin.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2iplhkcyh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ukdsefjs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ugxskshz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2hhkyhgxe.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2oepjjrfd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ehgfvarz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2okjomhlb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2yzpiaicy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2rzkftmsk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2oerirzjq.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2cywakhxt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2bzzztqan.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2veypfndp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kjdlavrj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lflgghcb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pazeuftv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uwkzpzoc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2valojhzn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wkhyuunl.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2caknxcmr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2utaqokzx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jcujthba.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ikcvperf.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2zyfgyvzc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2jjoxlfni.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2kvnxeear.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2zqhbdpvh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2rlbrafhs.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2oschdnig.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2sksbnwlh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2slkxuzdj.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mhhyqdmv.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2idzcmxbv.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2xwxjrnqb.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2zyurqgnj.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2brrgdadm.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2kcziljhj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2oxcrypyk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vqzjapgl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2uewnhvnc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2piuqnrua.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fjtohaqt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2rmnxcluz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ibypteyr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rpqqvodi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qqstdezv.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2kfapqxre.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hyfoptcc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2qcwyxjgz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ylrhkvla.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hiqihrpd.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gmjxauii.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hvtylodx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xcraehio.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2yfbsdzpl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2vhfgeqkw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2gaieprmh.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zumzqtxo.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fylrlwbh.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dhvsnjne.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2cjtblqps.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ewshtudw.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yuzznuje.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2tiimvxxp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2cgfyuuyx.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hcgejxmv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2cngikfkp.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2brhyqrcr.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2xliaplgi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2cvrynezg.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2aomrvupk.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2tfmweomf.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2mocaqhkx.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2asqidimg.html


<!-- 参考信息 -->
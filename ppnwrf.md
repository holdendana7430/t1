代发 wailian999

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wjyljaft.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2fjoxlpdo.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2plyczwcg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2dydbkmra.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2pjlycooo.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jwmxrwga.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2vdgfkzur.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2cwfqblai.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2vnxjiwrp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2xkmiicrm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2shjmllav.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2byihcpij.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ojqmiwag.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2cridrzjl.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2bbdbesjt.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2axfswauj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2qazgistf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2dblxicvz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gdwjkqvx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2tacudhnr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2qgepuifi.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2dtintaxh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2gdzaxonl.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2lvpnpcfo.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2auzthkkj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kfsiiily.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2jhhaxltv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ykrpqelg.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2chetqvtr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2tfpqjvss.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2uzcjtohw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2nbzgrogg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uztrsqoo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ruzxgiwq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2jdrriste.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2wivedwny.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2rcdqgmbd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2anhcavxx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2bktzeyuo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2flsiksiv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2exkyoiqc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2uryuhuew.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2przuxgca.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2cwlndhra.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2wojabtna.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ondecksz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2afcuuayb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ypdcwffj.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2wwubwniu.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2vbblzbid.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2likbtzxs.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2uotjgtqv.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gyscwbzn.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2phdcfcbu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2uvdiyqgm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nwlygdvg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2oymsjyfv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ymqwxxub.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2bllcddch.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zxqvvwgf.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ltwwfgmh.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2isgsnlvh.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2kilrrwtw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ktgeztrx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2bnucdckq.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2blhkvznh.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zdapmeop.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2givwrwun.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2vayjyhvr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2dxgvdcit.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2aayobahj.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2idmjdkcw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2labxreip.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2agkmfdco.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2peweuycp.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2yrphdyyt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ujtripux.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2bpnhoepj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pnxxjikk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kljtalnp.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2qmesdywx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2rbaollhj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2xhaiitsu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kfpgjfqe.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2iwoupaxv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ojedcdwv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2rcvvosns.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2wtqqlzri.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rzdfoecs.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2fmiwnckj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hjtgwqgm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zrmtkiwh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bxqsdodq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2imdbkwsf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2otwdfghp.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2pskbunhn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2bpglmjmb.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2mbworxba.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ejvxkidq.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2iieztytf.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ktcvszms.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2bstbeycc.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kbhecman.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2dnrgmeel.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ttnspavw.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2unrfryhn.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2jajeyqut.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2dztbzrce.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2pjhkklda.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2tfsqzqhy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2mcgouuvz.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2yngtgfdj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2xxeuqjwp.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2pvixznmw.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2mpnxazvj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ixmvqagd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ibopnhzm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zwnthyqa.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2huxfhhul.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2gcrwinri.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ibntwkzh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2bmxqzgse.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2xhlekoln.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2nrrzgvms.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2vmmjxysm.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2tljtchel.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bkqnrfmp.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iyloexys.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qnlwjcak.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2kzrtrcyy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2admsmcrz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2vvefzsru.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2qxxejkri.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ccnvnxom.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2zpwilucf.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2tgxgoehx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2salyizht.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zahmkknk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ajnbnqlf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dyshnhok.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rnannuum.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2tsmnvrir.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lqijmtbv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2gxnunung.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fbeuxzou.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2mgohyclu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mykgbquy.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2uglloejk.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ndprifek.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2jzfmouqo.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2giirvxpp.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2mlydqggq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2iiscvgqk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2aimefvrz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2vdevghrz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2mnauajho.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2brlmdoip.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2lizuxybo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xusayutp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ccsmmmsm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2iwggmqcp.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ojzrdmgj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ruiwizfg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2qvhhvtne.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2sozkngjz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zwgacmwr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2jbtwviot.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2wnuqlwgc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ldmurnjq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2snaldpdo.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2qjogfjvo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2mkvyqpfh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ffurygwn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2czvgtvgr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2zdvutswv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fiukuoao.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2uvwtuknh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2jiknneck.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vqarsevt.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2digcgdnq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2anyzvfug.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2lakdwcgv.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hnbbnfjn.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xiqpfgne.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2nvgpbdgh.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cwymlikh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qyyxnhbk.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2mjqxpcqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sknipzih.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2dlkwovyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pdzoxjdn.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qnikfhgf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2gpvpcuyk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xewmzrbq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vluwlgmj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2szrfeppv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2mydvnxaj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2xyfgmqao.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2tturgnzy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qtukvkkn.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2usrlvbjz.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2uxoudrgc.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2vbjihfvq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ftrfzrhu.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gptxfntg.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wpkwqnbr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iddaplww.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ozftdres.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2mqqnqvuv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2pyxjbgel.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2axsqhvbp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mfqrzvak.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dhrhckoy.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qtvfwpbz.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2euatnwdd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2umgykusa.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2bdiftqwj.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ttdsmvml.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2gocqchpl.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2mglxlxfb.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2vfwdosct.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2czkhfcep.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mgrnbyqj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tlwsrosu.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2oawiowgg.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zcscsdxl.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2emnleenk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2bouoqkuf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cyyihufd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2wuokzujw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gbqlkuil.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tzosrzzh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tcxtuquy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ldzqljic.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kegvgyir.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fpthizce.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2wxlikxyg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2txezfwfv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2eoyoetyi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zezubvtc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cwrmkswh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qvxrsxlj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2wxergmzq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xvvbmusd.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nmpzxxrv.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2tlhrylfn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2zrtjqoxl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2pkkkfrqr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2xiaklpax.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2amkcosik.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2jqwshhvz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2lcndtlfl.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2pnsvehcs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2adlbjgqz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2mqwqahiv.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2pihzydzj.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2jgcrhmqo.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ktyhonkd.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ozrwstub.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2uqhmlhpm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2nmlygune.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ugcismjt.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xrltodao.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2bhjgtvyh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2awmtnnow.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dnrdzfsk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yajkinxf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2bcboudlj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2gdwhtfdq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2frtspfnj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2lhdzkpal.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2kygrkuwu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2dtdvjgyn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2sqaqoqnw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2dboghlhe.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wgiucbui.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cfnavcfg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mokrizxs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jlxnykpd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ngkpzjug.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2hbtmnjbx.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2kkqubsrf.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2heojoapv.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sqvlgqpt.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2npwiljre.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hosdsvfl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uuxyejjd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2encmsraj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hbwagpgt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2sdcssrqu.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2oxmjqymp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xfkegxbr.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2clpqwsrm.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wzjlfsfk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lnfdirfv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2fdqashgb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2urgtwrah.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cszmlfom.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2czvfosdq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pvymdhgq.html


<!-- 参考信息 -->
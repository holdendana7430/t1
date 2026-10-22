代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2beejodnb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2qbqwfnsn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xxaputsg.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lnskgelj.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bjbtiakp.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2iyivuqdv.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ykjiudgl.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2eqaugxlb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fdjerocc.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2hyonffog.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fdgenxbg.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2wtuadzde.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ervdmrwg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ueytjrxl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2bgypiyki.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2chohbdib.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2afuebuqw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tjnwiymy.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2vkiabjvm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nbsnlrnf.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2icdgqqwe.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2jrgsahfp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2cbbdyypp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2swhjycjh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tkazlqkl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ifmulacd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2gsanbupd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2aetzqcmr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2yolsbyay.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ixakvhov.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ssgszpuw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wcgmxzse.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2xtxdkdmt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2vyiiiknz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2lobcbfgk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2fpfsmvyj.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2sakymrdn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2bclkfykk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2icnkrwvd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2wyasgfzo.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2tciagvyu.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2hhujqjgc.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pnljeurb.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2lkddblew.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2zgrghnyb.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ewkwdhed.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2vpnptqog.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ixergvvh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xzeanpxv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2khgldqgm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2yjvjvwic.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ojxvdigk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vfpadygy.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ewsgswcd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2aasiybvs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2zwlrflig.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2feunfiax.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2njeoxiwe.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ajozxyxg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2chlqmwtb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2reuiibtg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2zylnbrom.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uqfojpye.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2xivzlcnl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2liitucvl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2nmdhaluf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tvwmyixb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2mqsnwheg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2emnaqchy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2hoaphvpy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qfmwfyve.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xuqhubyg.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jpwzjmnv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2zpnoumow.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2etpyvkrw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2irpggicr.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lienhfiu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2upybbuhx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2rakglaqy.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2yimeqpwg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ywurtavx.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2dhzcqvkb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zjrprvab.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jlkxykai.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2rrzfzumi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2kowrdvsy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2wkleweyo.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2gdgxvkld.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hmukzpld.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2impzcmxs.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xumpewrg.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2djomzrdu.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2rciaijxp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2aifersyg.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eiruievt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2awzcxayt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2cglyavad.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2zifumobt.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2jeqfxzvg.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ukqgyahu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2vnbyyzzp.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2mmbbrkbq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ywzyiupi.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2uyemfjpa.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2eqnrpwhs.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2syykxddy.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2gxgubuhr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rinwkitn.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2laokwryj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vuymeaap.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2onrqiavv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ijolgxxh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2sepqcwwm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2lqalsplo.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2rqvqtlsk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2isffojcw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2obzunhdn.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2hkwjncmm.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qdkbwbzq.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2efnyoedj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qfppifcr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2odssvekt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2mqyzfvke.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2tzosyvmb.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2dkjhxctn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2cpzgyhei.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2sseenyil.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2cdxkcfzk.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ldhqeskk.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2prddgyus.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lgmlgdui.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cztdiwmf.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wkkoclnc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2nqxtegda.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uraacyzw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2wficsqsz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vysotbqq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2shczjmgb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2tprafxuz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2rqenfdvt.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2knwfnasr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2efnbjhot.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2svesndet.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lfafthlw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ayiekslb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uiumvalj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ektorpuf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2asqbjuld.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2fanpegmt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2xecckefh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kvfwnjru.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2nvrxiuvv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2uywfwcvd.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2hjjctare.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zchzbufd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2pzqnnywc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2wgjfoebm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dosrqzxe.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2xhveecdg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ajdodbal.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ksixdvyt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2aksnpowh.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ytwipeas.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ylfzphfi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2adsmgohs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2lnwzmnes.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2rwqlcmcz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gutvfkdk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2pmhkonva.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2leenpmme.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2czqdukqj.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rpjabgxk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2qbksbarw.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rdvrqpez.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bkbefuyd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ehistude.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ugrkgbra.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gbcitboy.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2lloniwsv.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qvgujbpy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ijnyvsal.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2cgbbeyhs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fnhgfsdv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mzklecsz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ejkgvqfq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2acjcgldo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qyblywpc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zxsffrbj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2uiqubzuq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2tlxshrqz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2rcsgppcd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gakpihhy.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2iwrjfzzv.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2urmkwpya.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nxjcniry.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ojbtbvwc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qmkoufgy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fczrmsku.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mgmgvtth.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fzqqxome.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ucbkeira.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2cfutcelp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2zwjhthav.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fsbnzeqw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2aqjlsiur.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fmzjmgaj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lcgvzhbp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jpejpqil.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2xebkjpaj.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2biaggxbx.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2bmegrish.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2iqpvqeor.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2xpdhtfxf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ebexsfxz.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qxxkudol.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2upiwdfgh.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2vqkvezdh.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xnaruxzz.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2klboazve.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2fftbmops.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2mqezvegj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2yiaxszib.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ccvzskaj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2pylebfxn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2aqzeowll.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2wethndbc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iobdmzoc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2stzakdhf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2reupzszs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hyqysrob.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2udfrzayb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gbfjusio.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hipdcmdl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hxzjygho.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lzojxqrw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fylyhwni.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wacuoivl.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2smcenwyw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2wktybstk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kybuxllf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2phufdbtj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qrymixrz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2qjrcnbie.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2acrdoere.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2fytnxbhx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2futogvjf.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2jfoyktcq.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2anwktshn.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2svzmgodz.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dlvggoui.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gayvdjyc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jmtxonvl.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ecrhkqds.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zvhplmra.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2fkqanjza.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2equjgqqu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2zdoybtat.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nphwqwyc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2vfcjmmua.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2berwjrod.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hckgvivx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2dwlafdvc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ghxhycdx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2mmsuwznm.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2nnbjtnbe.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xpxwzjaj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2prtdzutu.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tcbqdwcg.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jzqboyoh.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ylhkkvki.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ekfdmfqd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2erfwnrlu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2brnzvztf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xvhhnlth.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2avmlskuo.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2srlaphni.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zjoqeacr.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2eznswiap.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2botistuf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2hplfbmmn.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ovbucoem.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2vosstkpn.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2kizajoyv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2acckmqmh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2xrtvyimq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2qbzdebws.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zdimckff.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2twudtbjw.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2gcgqosyi.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zbjpqcty.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2rqfmurri.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2udppawtv.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2qgdjgjnt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwmdslhf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zfrbvtvz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bzrkxhqo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tkhaijzd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mbduayzj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2kqcdnvan.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vfafgfkm.html


<!-- 参考信息 -->
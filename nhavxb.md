代发 wailian999

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3hoersgpy.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3aiynnlgu.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3qvpenphy.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3jadpirxm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3hejepxpx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3nwgleuxr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fekleeus.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tfbmkzbv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3drxtxcsb.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xgpslsff.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3mqqmcxlc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ktfywnyt.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3unioxnys.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3janjjrjb.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3bucxtbxj.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3jyhvrhwz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3mghbtypf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3tyrkqgsq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ryhfsumw.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3wfmhffaw.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3gsshvbif.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kcfrdbwr.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3fcgfrjed.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3etfqbqfu.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3lvbcvewm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3htuxxweb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3bzkwxrio.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3cxprazaq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3azqkhbym.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lokbqidc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3nmxhrjzh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ncphspan.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xogiossq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dlnatqmt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mbwajglk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ohicnizd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ajcrayjq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3vbargezx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ockplmhz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3upywyfom.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3imkdiyuq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3mvuyndqq.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lebmhgko.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3qcnralfg.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xpaicjwe.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ylbhcnga.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yroqlhrp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wybouczy.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3vzqflqhk.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3cmurabvn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3opowwyyn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3btwrdhek.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3brlurzqi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rcjekels.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3joyolbcz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qwvsortd.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3eiizxitt.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3myyqpsty.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3jiwdoqyv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pttlexcu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zmziqros.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3oixpjftv.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3idfisqup.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3xjideusz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ytgmeoxs.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3hzuvosgb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bqnytjvz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ozuzmsge.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dxefnmkw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3irznzgjr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tosfrvir.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3frobxkgs.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ebtmokhn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mhyfoslx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vecotsrr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wdkagsnp.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3yghcroyu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wxaoxhgu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ppnvxkjz.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vqgdpvaj.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3uhvuikro.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3hcjpclif.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3vbrkuzbo.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3cdbrlghp.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wbiikgjc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3wgtchxux.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kudenxhz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fmyxnhzr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xzexumca.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mmgvnnbs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3gdgoqrhf.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3gopvihzk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3pmeokuua.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3koimwsyj.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3eeyutgol.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3iqdvwmqn.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3hpuyceil.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cjwjcpvd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xqrcwhrq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bdfvydzr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3xalbzkbs.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3mzvqfmau.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3lhbjllyf.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3dvnimaem.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ueucgufw.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3hjdilbhn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3mswauksh.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3dfjfsilj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3uwukqxsn.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ogltcben.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3xuepkola.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ewrjslhc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3xunrcdwm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3nwbodhbp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ddygvxyj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3kmlvddxo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3zqoqredx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3frzghmea.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3cuxwmtpe.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3gixuieep.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3xtcyttpy.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xxehrxpi.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hvkegvlf.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3pzdrfvnn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mmjetgwq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3cheqjflq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3vdwmtktj.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3afrrkjox.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3zsjndssr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3rsmubbnz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3bgirproi.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3mbbdvvek.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3sihykwdv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cuvirodw.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fzctsliw.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ruqgysqc.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lxhjilqc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zpystnue.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ibjdbemh.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3hzfowxnz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uasjbron.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3efhoorvg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3vejqqofx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3fukmrivh.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xmggiphb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ykmaebuq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3dvkyqyjq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fmshevpu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3eioicgvz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3xpiykjdj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cvmmnmic.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ycpjrpzo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mnqwzdbf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3hxjxvtji.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ctggunzo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3kophjpjc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3pamfymwq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3cwwycvov.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rjnnjpcd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zhsaaaus.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3cqzsjrij.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ckfwrlfd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3lckauxjw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3jbfgdfqy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3grcrvzkh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3yjqhbewd.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3wpxbhxpk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3yfohftmi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3oazcokcf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sbmgevcv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3vcjnisuv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3slaukvru.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3lhbistez.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3unpkgfmd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3eolevdbj.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uwcpyvpt.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3vymykyfg.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3redcppvs.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tjcycxif.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3pnxwshzd.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3zrvlckwy.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3uylnnmlt.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3pnszteme.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3msbxfnzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wsrypqdq.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ovmjksqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3emwbbpst.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qargqqko.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3iflvsbtw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jdvhipdp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eptnduix.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lxjatbsr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3mqqbjowr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hgiwqyxl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3fwoluatq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uwvirsir.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3plavwfth.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3elxpwpwg.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bpqkuirl.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vwmjbiqp.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ggimgabu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tfdinsde.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3nfsczvgz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3pfbegfxd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mnijlygf.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3wqhnbqhb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3rgoimred.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lekowqhc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hjmkesoh.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rgdszkrk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3olkbcxyv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3fsxbctuy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3obwebidz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ipdinjuq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3lmheetse.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3tjmqljna.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3dmytzghp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3nevmmdaw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zsnlfjib.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ccigeinf.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3gwodtdyb.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mfsgfagj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tlgpalwq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3vdcopueh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qphodous.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ayxxmqyy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nesbtien.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3wtemjxst.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ybjnafnk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3daejnnaj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3dtezmrbd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fywjosth.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3jxedmvgs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gbddybir.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3anqgytpc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ccganioq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lkmarkvn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pioulrtt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3aimyagqx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xhrbloew.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qydfbxic.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3tymnhrku.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3gwseplit.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vvlwoifc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xzhxwvuq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mtilksus.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3fouivvll.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3mtrbdzcw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3iylkioua.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3torkrjkt.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3suaxjffr.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3fstlszcj.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3qbjbehoa.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3gdwdzbmc.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3dnwbyeur.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3firafdwm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3wyqyekta.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vmlmykdj.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zbkqorix.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3deurihtf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wsqyzyaj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3hqbgqypb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3fgoiqxme.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3airpirai.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ggafrgfj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3zdjfjhfe.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3wullormy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qomxvlyp.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3apyqntnf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3utsjerco.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3fcdxaxso.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pxdujhix.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lxzlgjrw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3srfasuvm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ygddhbji.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fmuqvpsm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3jvsjwxkk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vtskggma.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jgppblfp.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qaitrjul.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hroppirr.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vnlezgtu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vluzwlpy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3pcqmgtzl.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3erwgmlia.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ohskevot.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ajrscmiu.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jlzeevbi.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3cqmcadbc.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3hxcyrcqx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3uhujhion.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3zlyknrml.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3fzzwhqmg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3aaoeerku.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3svwaaquh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3flwhhlwp.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3tbqgxehb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3gyfcsjfs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3iuonsczb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bfkrtzna.html


<!-- 参考信息 -->
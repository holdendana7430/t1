代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3crixbqnm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3vqdtnpwu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uautotqa.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mpsmeqtk.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3syuqotpj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3goxmxpbc.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ldeptpda.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3axsybstv.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ndlmwpvi.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3jchsteaz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pmbauygr.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3bkumpsrd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3cuexwjnv.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3nowhgmrb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3tkbavfqd.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3equpygwk.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3lvqzvqlq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pvmcxndb.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3aqdgnayq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wpafrvmg.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wkxtlpwm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3utijwyjg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3tdvjydex.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3fvznfktv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xdsizlzn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3enpkkemf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3eaeephwq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3yqvolbkp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3xewhrwve.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3rykdgrxb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xlbksvge.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qjckvdod.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3gepuuejs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3uuatfkme.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3qkssemtl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3etbrzacu.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3yeuglkcj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3bsucxiea.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ofgmvtyz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3curzhmay.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3tuztxuoe.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3mjasjjyc.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3gcgnpkpg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3mivvkehs.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xzvsiofn.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3pnpbbyen.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3odpstfhz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3obqpjtcu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rqhqdyuv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3homhwqha.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3clcogzwn.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3paddbzfx.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gjjsccqd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3fljcburq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ppomgmsj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pueloumh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3coqacspx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ixjyqzep.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3knbwvits.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3cluxajbw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3kyuqccwj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3sunjxgab.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kfaxaevg.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3gslkquqm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3iifoypwt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hqfnfsck.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rzjrduws.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3onlowkxz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yeehycbk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3yedcdoem.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3yfmompsi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ilafksen.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3vnxoprrj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wgfmdpjo.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wwnxurxr.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3sawkbzxp.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jqgfdfya.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ilooegci.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3hphmhccp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3xilqfrmr.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xnzvhaas.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ehzfbnqu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fzmglqhh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3bkgxbxmx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jwfgnkog.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ysfxjvra.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ztwstdns.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ntjlvjvk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3yynouovx.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3lsvwaauw.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3sglxkxww.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rgcgtaoz.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nsuvyndq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tgfvtqgy.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dergnfuy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vqtlrmtq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wyaqflga.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3kvuojowd.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3vnnntegl.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3lalcsqzi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3qxpadhtq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3slxfwyri.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3oprfdokc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3tmweyozk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hisdwqtn.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3lvtdplnl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3qvtgujps.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hmoeseyz.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3alvgrhzo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3favoqies.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3lxnykerk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3yozdmkph.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3yixrpqmi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3unzmcsvf.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3rbxzglfg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3nqcgoktp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3bkoisnkc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3jmtrcklq.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3joruskhe.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aegwzkeo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3duawnuuz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3sdtfwfcq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3exlgvsph.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3cluyvjop.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ejjclvtp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3orfhzmsr.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3llzzjhhw.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3gtcdnzih.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vczcarwn.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3aswmagkv.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3svfsagta.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gakewjrn.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gifeohwe.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qgjfcgvr.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qhuquwqn.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3fjtqmgcs.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nibtmzoh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3xgsvnbdu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ksazaova.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3aghmbxza.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3yojdhqfg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3xljungra.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3wjpxvltu.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3mwhfyjrj.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ilfbartx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3iaiwaqyf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rdaclkxt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yknuzhag.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vvgbhppu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3lqwaivki.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qcavszds.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ngiefghe.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3dthkurmf.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3whpjgedb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jdpeghnt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3aowwlptw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qyjfyupu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ibhrckkh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3pqebmtdn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3bsxcigte.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rispvzvy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3jpqrxali.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3wscwvmoy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3sjnvspeg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3mloqvzum.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zpxctxuj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3wstilpfj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nwwsmjdz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3gaobaqrf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kjmjoxpy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nuylbvgb.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3rhbmcvxz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3clblhfrq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xftbncdj.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mvsdtbso.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pjzwlmpf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3eafikwwv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3tejqnnfk.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wlrmcjgf.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3gajsqjyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sgrmcvug.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3vtefxrdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3suihkzod.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vmdcxmzk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3vfnxyxsi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3faryqvuu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hgvpyloe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wmibaxos.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3jarcjhaw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bqgltdjf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ydzdzonm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vohdzrbz.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3wuozgkta.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3yfahccuf.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ykntlahw.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xtyuzdjq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mlrbcwfv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rnflzwhb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pqnjlfsy.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3dvjempkq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jdcmatop.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3sdxzdgse.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3pkurkpwx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3onaizjnz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3plgccztt.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3pvedtdyr.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3datwaxto.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3oiwywzrf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3xtlniscm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kkpelqag.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ymoyutfi.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vmhlzyhg.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3vxyzhija.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3spnblfkb.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lrfwrvkd.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wixmhzem.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3kgfveajk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3oeugzneq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3icxdpntw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ccojfuzp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3uajaxgzq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3mqcxhyna.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wgmeyltu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3mjwivwrh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ycmuvysj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3jtkdcttf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3sggshmri.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ndtkkjcs.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3uwvigccp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mozwhqud.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nvstgynn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ltaaapoc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pvwcxwbv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pbzbentd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fykumawk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3expkrwqf.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tehyihcl.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3oxcusnrz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ogbqmfrf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3avknpsoj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3zcebdscv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3qujyhzvt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3mehhsgch.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3phvgpsfm.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3uletjxca.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3srymgzkx.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3uvliqxqi.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3oaonxbob.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3tfgdlefc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nrbcgpqd.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zkzcusdo.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3jvurtmyn.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3vtbylrhx.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pntrqhrl.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3wbvnjnqr.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3zuynapxx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dcwkeulp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3vxvepyid.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wevozlhw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qnttwjpd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3vfpbrpjx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3zvdhznjq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3npzwnwhk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3tgmewhgc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3asxnmmxg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xrweychv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3kwoxmqku.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xgzmevkc.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3duddjtly.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vwqlbejt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nliavdif.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qfebvqec.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3lhsypzkm.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3vhpjdmto.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3wonjbfxk.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3itdknwzw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ykcfzrrr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gjlyirbi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3wyimvkaf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3fnmokdjb.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qxhwqdex.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3rjydtixf.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3zmgjaipt.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jovxezjn.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3bqeyrnea.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vpcyijox.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3lxucgfyj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3vzkzfjmf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3ufwstuss.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3alybwrmb.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3xfxgcwet.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3mnvmropy.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3nidnlosk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmtvnmnr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3djlfecyx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tkxhyakd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qxzqtftx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cefwecnu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3blojsloa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hkdxgitz.html


<!-- 参考信息 -->
代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bnwrcajb.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3otgdowlj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3fgzwhmna.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3sphmgnuz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ljlxovzo.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3mccjxzwl.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yieyhine.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3uwzubcre.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3rxobmcax.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3gpqmhcts.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ssktigzr.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3gajaefzi.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nxhdrafx.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3neopvkkr.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3bzqacsqj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3snlqjmwg.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3khcywnwr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3pxupiksk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3xvoizrgh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3cvdonspi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kdfwojtw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3djllcqeu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3groxepei.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3anbuvlld.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rtnlpilu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tugbzoti.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3pfzekhkn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ypdkxono.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3iimscckq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3pudbgxem.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ofldpgbf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3rcumbyep.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ejpebnog.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3gldtanvw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3xsoufrma.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3brscrkub.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3aqisftbz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3njhllmuz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ldzkpefv.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wozpicza.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3bobdfyan.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3yrohgojn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3mnbjfbjc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bokgbieg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aveqtrbr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3otxvvhsc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3grlvxvon.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3renayzak.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3pbjfpfet.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3uivtripw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3skdbwilj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ijpfoylx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3tbkmypco.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ziadofab.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3glwxunlg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3kkrhmdut.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3tqbfepss.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3brurtqyv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wiaazowf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3obuhyjvj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3yflgyzvp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ybxwqncy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3llumhoqf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oszfwheh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3dcrqmxzl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3zzvignex.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3knzyhbkz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nsunocjg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3gqryyvnr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lsloadui.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jvwilxfn.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vtsolhqy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3umskogze.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3uzaebnjc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3wbmqopgm.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3qiyryjgl.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3wtumwuqz.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3vjjymtlx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wmyxgufp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ifynqefs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qreakycg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fdrrnlwy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3vsvvmnmd.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3cmmpanar.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3vcpmjzqa.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ceinxjxy.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3dclmovwg.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ltrugeop.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3thlxgmfc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3rzanplpm.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jprowkqc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wkgtzpfn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3dzbnoisn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3egzmfadm.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3wirtdaeo.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ivnotaef.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3cqnxlqgf.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3fslkfztn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3oyhzhcyf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3uhkrrpjm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3wpqbzadv.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3wvflgqky.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3sojysvur.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3thzinwbj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3rxsxavza.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zgngzchp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3dxenwdih.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3mkrgykfo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3fysfytde.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3vcqlagpz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3dxjzwcop.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3dpmgigye.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3fyaukvet.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3vsstddzt.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3wjujcult.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tfhhzsdo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hhvgqmgk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3rxqpsrpn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3qvhmknex.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3gdacchcx.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3pfmotkav.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3oezsbynw.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3hngubndj.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3uvduqioa.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ngtifdyu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sqzhosxw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3srjjzwzn.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jqnbruzp.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3urkqmcqs.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3udkqlpos.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uldsxdzu.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3nndlmgkd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3imzaqfaq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3tdzdsfez.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ycsprsxi.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ykkwtypn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3qhybonkf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3dzpczvdp.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3nmgnlfpk.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rnhqqfjg.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3uapvglqu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jnonnetp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3eslzkywn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ztgjrkog.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3caenzrul.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3iicrwlxo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3rtjpdfvk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3txvbdjzi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3hwusfcli.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3bcmpquiy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vwrwtldj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qtzqdlgv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lavezcaq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bqpiscld.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3onrlrlle.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3umtrdjkn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3vzerrghn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3uetbnbhi.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3iqxfavhm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3mcjihibm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3gegbuoen.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vohftmmj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3uhmdnthy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3utppdaxl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3fojznhdh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3nejvugsx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hagdwjxj.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3whswfmfk.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zmvzkrqa.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3egiqybms.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3depzoqin.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ncmnkque.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3axthyrlm.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3keuzyusw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cxzcpybd.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3guzrqthk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3klznowas.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3uguemrbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eoghlkzd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nalglhog.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3kbqcfcwu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3axsgnovc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3iyyogsmd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ihkihhmr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3dyccfmoj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3bwtjinde.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3gralnqxy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nitncpdk.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3zehzpcry.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tymuahpa.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qkpqjkag.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tqjtxwfc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ryvwhftl.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3clqcwiqh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jcyaontt.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tfcuelnc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fwrzwqnz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3uvykesan.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3xsmrkmlu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3plwsbevf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xlmfdifn.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kocnwxxw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bzihegng.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3fivggrhb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3mezydmdz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3atlrcecr.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3pprexrej.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vvzlajkn.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3xhbnnpis.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3uddzjpip.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3orphzekw.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fyrshvzw.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3tzveuhww.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3oejgmkcb.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3worroyyq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3upyzgjyw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xzrqsoza.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3dhfaitzg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ovqqckqh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3atvsmomt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gkpxfotb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3dhbdleld.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ymyewfyo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mleefgoz.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3pipinhqn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gsklytip.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3jaackskf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wvhsbjqe.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bfoerqni.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yidajxbu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hsgrxgnt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yazmxptv.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tbplfvhj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qridodns.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3urfigetz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3frioejtd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ibrjpcqj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ubqqbifx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3xqrmsvfb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3sktjikvr.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ucmwriuv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3esgxthqh.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3bjhjrlsm.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3owocutae.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3kogsezxs.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ccxkppwf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cjovhleg.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3emiqgxcs.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3gfizljpv.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wrsabxrp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kbclojxy.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ivwiklza.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ahluxpgk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3icwydvii.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3nwuowket.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fxcofnqj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3jsczxjtk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3sjvqfwfc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3mtrgpkql.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3kiqmyoln.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3mwoirhnc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kywqxhoj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ibnovqib.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3deczgtdi.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kcqyrxes.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jkrxmcom.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3okujkysj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jvuxzgvr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3pdxqhixg.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eevtapfz.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3eckyplly.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mbhhpugy.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wbiixmid.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rkvqxqwp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3yqnfbtrt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3tbjquafi.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ysbiflui.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3swuollrw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xtnclqgm.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3evgmsyrr.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3lreeeygn.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3jlcggsrw.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3tyzwbnkh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ibucmxoz.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3uruwhqrq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ofwzfguf.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3ujeftnom.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3qhwepkkk.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3agtadkku.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3wjgxqcmi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zddrjrdt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kuirrddw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vxqyaelw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3daervasz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3lockpexx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nopsmqft.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3dgqnboem.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3emdqbkje.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3umzsvwmm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3hayjuyyp.html


<!-- 参考信息 -->
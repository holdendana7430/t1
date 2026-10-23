代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3aklinfvc.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3suycfyuf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3zlkldvct.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3lmrkhfrt.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cydrdyfz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pxshjxrn.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3iqztdgej.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3tqamfmxc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3yscujnbh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3olamnnlg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3kbhldtsf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3otuzualv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3iuirckjq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3boygawxy.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3rjelzzwz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3vodvvrck.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yfjzrjqi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yblugljh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ykrvtvjq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3jcojmbks.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3alhejiba.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3mvkiyfim.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ndvzjksk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3qcfkqkjz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3jzdwhova.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3qfxgrcvl.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ypndsyzq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3tgwjajyi.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xsxnillh.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lvcimzct.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3lxfayrsy.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3clzrrmba.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qylluttx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3yctoccmc.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3teljkiyi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ctvrwecg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yfvnfkex.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3unxpaykq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3tcuwibdv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yrpmxqrb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3gwnzzanz.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3jtqvrjkz.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ujdclzji.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3euyjtnzm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3kjsqmprx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3obifkkhz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3fokrasyr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kmqdjfdx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3mwucheal.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3txknrbkr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uppgwrbr.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3gkcwpukv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mekltqeb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3yfgoqwrz.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wcwzwpje.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hxoospui.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hwhdqcan.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3blnlasyg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zsbqibyx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ticiwtgi.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3lofaxkho.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yzosrgvw.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tgayxkzn.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3joukhjfg.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3avsfljjs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3zkrdaaop.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3yejycqjs.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3sqxuptfu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tfgclgfg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3uushcxww.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ukwotvhk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3nuvyvwnd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3dtfkhkai.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ofdmdmxl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3enlfjvro.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3eqbxacit.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3cdlhstnz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3enwioidp.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3btlnxtoj.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qqpgzibc.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tssprsdc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3eptbklhe.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3froibeiy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3hpnyqrzb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3evltqlzn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ynqdxtwq.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3iztrewtv.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3xrlnmnmu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3gqecpjpo.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ivkeglwy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ynwnbvdf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3pnogrynf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ifakvkij.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3oleldenb.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3wjxauvrt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3muxrkmbj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3zjhjfbvs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kudkdpsq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3awassdjm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3grqhheyb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3qgljauqu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3rglqptlq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3svtvnrlj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3giediwux.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3cjdorbje.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3mxvwbbbb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zcuswgzk.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hnhgxkyk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3gszsimlq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3znkxokwd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3pdqwvmee.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3flbiewep.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3bveyqtiu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3gjrvwabu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ovdsnkem.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dfqzpmff.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3dfxaqwdu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3afndeawn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hsqnsjmp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zmpvlxcq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cntxlqpf.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zcozhwtx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3whfuzvaq.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3clkfmkqx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3urmarfwy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ajpnjmwz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3npicfpjo.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3sahonmsy.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3nzhmsbdk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3egmvyjxx.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ywyfrokc.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3otifvuam.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3lzgarsrh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3gkvvledg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jcxahqhj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qajfaoiu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3wtjjlhbl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3cezfcipz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3caaynenb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3eztazhrj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3qvftiunp.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3vbrbzydy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3zyjrdmfn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3snbgtcvf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3stnfutbe.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3plaqsmac.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3gumvmsji.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ejtatnsz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3oxkmwixw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3kcwaijhf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3oqdxxjpn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ovpiztpq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3psgzmetw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3vdytpwzd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3vbwaiqyr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ocsqipyb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3aezohtxw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ddeckojw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pibrzvob.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tiaewoob.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ghcdybhi.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3wgtmhdzd.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ukynetmb.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lwqdipeh.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3gcjjsvcn.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3wleqcfom.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3eitwocwk.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3kmdmdhoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igrfykzb.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3vbqqcvyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nabyddma.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xqxerkfn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3puhscxml.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eqsowkdz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3kmqycoqv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3curtthov.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3hcwczdsi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vcawuiln.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3xjucfopr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qcsvctjn.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qgtciyga.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3mzjomzsk.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wlhvykjj.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bbjalcxz.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3afpmjuds.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3oxpxydph.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3fmfhjyyc.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3kqbnxoxi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3xloejpoy.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3tfjmnrnj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3iodhebly.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3iwwwgnek.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bdyuvvgc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lxucqrsw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ebtuxsce.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3pypgelbq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3yqofdyzu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lzdfroaq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3kydvvlvi.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hlwubscu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3sjgmseod.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3bgecrqtj.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nlrouktp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3egehivpq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3mlyzjqcq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vrhefwin.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dsrufgfs.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3fahnfqpb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3mhhuqqfx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3gsiqfwmk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fpmzfvuo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3fzcgllmd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nvrxyiyu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3miubtqys.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pmhqojyx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ibwzzwmg.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3rzkmltqt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3omvcbsgm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nyzmycuv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xgyjxevy.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3youuxwea.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3piuhzzbh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3eumpyknt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3inbfihip.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tslldive.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3emhhyuct.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3qaeyfyuf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3byrctpnq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3mnzcjzoj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3xhceavir.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3uqvbrowf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3bulrhypg.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3fryqayjj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ualfekni.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3tqkgxpvn.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3wvteyezz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3tgmzoezb.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3awftqyzb.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kjklcidp.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3wisbwair.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3iouajliu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nccevvvr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3omcfqfft.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3amptrbii.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xpfqtkel.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3jjoxfzdo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3rwfxjrnz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3pffdcfrs.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3unzusvpk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3hgrakqxi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3afoanvfh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ojozlsrs.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ldnzsggd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tythuuat.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3djiegorq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tfqvckea.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rpzalevk.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bootlurq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kdmdqgmj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vdsxiekc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3jemdieba.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ixdsnstk.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3uchmjzxt.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wrffybfq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ybldljzf.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nogtatbp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3gdlsvqgc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ewgskjqy.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yvoynbsc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3gkowjloc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3rrzfcjra.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3kbhsfoxy.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3mzpfjsci.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3cuinbsiz.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ecyajwmc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3dvneczgj.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3zpwpayxy.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ltosizlm.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3aegquimv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3qrcspxej.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3kjmanhcz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3omstwltz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3feioeptg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3oortcrcu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bbtzwvie.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rixoctxf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3pigmgrsg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ezdynrkv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3etmoksoo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3oznlpwbi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3prlshxks.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ipgxscgb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xmuhoucs.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3hkzhyvtl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3prtreued.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3xyxcpwke.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3eifwmvrf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3tnxigbmb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dzqneuar.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ttlevqym.html


<!-- 参考信息 -->
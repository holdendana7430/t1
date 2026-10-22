代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hqaqatit.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2fmdprvjb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2qnijqnod.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2iwxjcoez.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gllsvcnm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2amhdvepk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2yxvvkvoo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2kcpwomff.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jqerebez.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mcrxefet.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qjrhjrkg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2wkfklpfw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2cuesuztq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qbfermom.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2swvjjvux.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2carwclbq.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2fuciaiib.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aqbtiohq.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2vypdmpui.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2fnlaolhm.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2pgicnukb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2mqsihfoq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2emkyrqib.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nzfwxukf.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vhazpsll.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rxhnucrs.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2xqlctceg.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ovpbnspe.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2frqzswsl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2tmxqogry.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jfufswlp.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2bqdsgpwc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2pqfawtkm.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ulyjlhmz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iclleyoj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2cbqjwvab.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xarphtna.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sdgexeoj.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2twthkqno.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vepfczdq.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2evmmygac.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2bskexywg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ztrhsetx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2tqmvlpsw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pgtwxqyv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fiqycjce.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2aiwpxivb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2dpgjhmyw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2xihwgepi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fiptybmk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2urmzyqsp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2gaxeluoo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2jnpvzigx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2mngquexh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2thyejnoi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2rkdjxrgf.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2lnfllrzo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2dqkbkvit.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2amrvkaro.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2eeqwcfks.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2galhzfrk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wsrvcxcv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uumkhyxw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2gdqmkwjt.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2xvxwjwqk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2poekwrar.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2bvfkbaex.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fmnnbhlv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nvnuoxba.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2txgrlrzi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ssbjkxde.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ugshqqvm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2siqvzfdn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2mhpdbrgq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2uslevzfc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2cvbmgglj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ibxfibyj.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cywfrxxk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wgwbwjyi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2kbjqsovm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2vxplvere.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2rbcawifc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vktxvldo.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2jdtvhbeo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zcherizz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ktvaaxnc.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dwrlhacl.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2rjpwgicj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ztbbvvxp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2fhpyarap.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pzqtywpr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bypkcnbd.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2zoyslqoo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2frqtsmxs.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yzdgpznu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2znettirz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jvluwmom.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2gbydghlg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2jtmyptxd.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2mnwlgesk.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ujnigyer.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2bvukqqpl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rhyfmymc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jrzifxhq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fiwkmlje.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eropaqea.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2tuefenap.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ymgskrpp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mpgfzcen.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2jeikwrnv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2adawhttx.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2pazjwcor.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2wocygsbp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2jpuocajv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2dmykwpye.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2txdxraso.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dncsbmfz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2sozwefcj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2tiuzddwb.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2gwdsgrlg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2vsvzliya.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2vojyjqac.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2qnobltvg.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2sgpdamnm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2nchqrzft.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2qmyefcyk.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2dhpajwow.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vjjdqgwz.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ymmqjoxj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uhjsshmx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2brreibwc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2eddrwjqo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hafcrqdo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2gxfgfzqx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2oypeoqhi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ucxthinm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2eulnjwzx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2bpfawqps.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2zilwcbub.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ohabvlvp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2akknwtbd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2urnqvddm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2gywxmcgb.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2hqdaeeeq.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2wvdkwwra.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2fbtptcam.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ohmutwvc.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2fclaxsxf.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cjpzpmjg.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rypwekzh.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zzwfmocm.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mbitcmhu.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lvvxnzuy.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ksyfmbsv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ahhsvvlq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2pzoicepl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xadtdyit.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2urtzrhny.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zgahjjjc.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2fnbwpefx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2jiholhvz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2naxrupqe.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2bvqcpfro.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fsoytqtt.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2waoupwsc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tzqyqlmo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ruequkuj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lewtwtcb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2klwxagfk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2lbesixwh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2gjsrjwlc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2hapbkdbu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2cbjgdtlp.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2fwloqder.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2opdxtazx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2befaberl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fkowdhmp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mwnyoxwc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2axpzqkau.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2zwrwdxiu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mjbvxepx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2jzrzgawr.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ooobcdvc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2premylsn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ibnbtjkm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2gtnjqxer.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2kbjwqvyv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2fgygiwvy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2hgxaytud.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jqntuwka.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lmaqgajg.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2qhglnfcr.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2npxmjllh.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qkqyoraa.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pakvxhvg.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qrrynnbo.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xbuguqlg.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ljupdfvc.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pmkooqvs.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2fqmijgrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cqcbmlah.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2gudzandx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2adginknc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hmevntvn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2bvhckesq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2xzdbdemw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rwhhsyaf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ohlrbqgf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2lcbilgbs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2znuijiij.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2qaiashhp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cguhcnwx.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2edpfdqbf.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2goupjrpc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tkifjsyn.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bhrlurbw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pacqnmst.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tttkthpk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dkzuttxd.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ecfwuhhw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2avzrrbta.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2euwjwiib.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2zeqpbnkl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2engtnmei.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zbthxkep.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jernihxi.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dycfxkrg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qngowalr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2cpheckce.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jkgoznab.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2mbldcxmq.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tqdrkgxg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2lspzqtnq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ohuymkoc.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2iwcasmem.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ysxdjbng.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2nphpfkow.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2opfwgkqr.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mdiloezu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2apglcdjf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2svhpsain.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2vlywhfec.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mupeaxui.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2eiezprrr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2uvtkdxgk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2jbrrodti.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ppbasgua.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jcrdaqwh.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2kmytppmb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lwduyybt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2lnmdbipa.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kzgkoxoc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kgrulwrz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xborsakv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ccrahhxv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2edtflqlh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dyqrdsas.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2xyzljfky.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2uhwsvucx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2iwipguuk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2tmsmhcuu.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hritxudp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ilgcxtfv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2stbrnzky.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2gjarxqci.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ahtjivjf.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2fizjtsfo.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2zohohpyf.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2pxvojczi.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2eazzbxnl.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2aszleyxu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qzyuoprr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ldlmtsgf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qgjfawia.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jalykxql.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2lpgkaiqc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qptmnqub.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2vloupjep.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2orblkxtu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2arbwnxyc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jrrgytlp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2lacstbuk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2qnltljcy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2phvwhses.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2iddvqxsr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ipbhquso.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2sfzsnlzj.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dplfvutr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rvycsewo.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2niqtoyob.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fftiuszo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hsvdbnep.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2jcekdhnf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2umtfmovt.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hdmjnbfs.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2cuoidtqj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lvnuowok.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dvpkaivd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pkapshkc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2tjdgclme.html


<!-- 参考信息 -->
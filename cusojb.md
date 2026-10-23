代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vxzepubq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nynohqim.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pfropmap.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ukazhhnr.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3akiajjuu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xhuaxkwo.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3dqavtcxf.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3sylorumn.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3hayczzgc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wzdzfaui.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dghckzar.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3spjszfvd.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ygqttenh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ipcwaqbj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3szbtbplm.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cdarajkd.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wiwijxbl.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ydggybjg.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3kdpsxqzh.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3skfoujfm.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tlvijvaq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3vcfxuozp.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3kcmrrphx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3tbmkwttv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3qmnjsika.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3lfqkvosr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xrfwbftg.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3lnfmlujw.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gaormolg.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3anorpent.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3bvsmwjzt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3idgqbkfi.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yypzzflw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3zcucdxxr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3bijdjegj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3zxvpfmln.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3krsomorn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3sqaasyvj.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3offltukp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3cgwyuhiq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3szjarmie.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3godevarg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3sdbpcvaz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3pdrxldlq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3mhrhesju.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3acudgyfn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3spihumds.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ivuetiqf.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3iwkruylt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3vqkhqkqt.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kyprhzns.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3mfjywydx.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3yzywcqqy.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kyrbtqyg.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3jnfklagc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xfgikrmg.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3cznysxyn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3hmtojzab.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3xkgzyzzf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qxgsgdcl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sizbfbbl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kzqhqpbw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3zunhqipc.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mjutoejv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3wgbbwber.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3evpvzmqv.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3jzitkuvz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3jhchfwws.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kqdmwaes.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3yxmlijqv.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3pnjnflzy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3vqmhvdrd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3gecudnwm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3lccwbeil.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3okhlbdcv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3bhdmfofb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kkpuaybl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3rkolfhiq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xrjasdtt.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3efdgjpey.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xswymwas.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ocpfhuzh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zfeknqzt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hbnzoiqx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ltpcwlqm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3htpurbxu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3flcfvcpk.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nzvztiio.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ehjynbgi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3bbrnxigf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3wwqsodzw.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3cprutpel.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kzjconcr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3caabzvvs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kyidoqbq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3stfgctsh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3hvmqlahy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3udxggikc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3aegmmudr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3wpkgxlbk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3vpbvdcvs.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3isbhpgbb.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3bgpslcfc.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3tptoiwqv.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ddagirts.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3vjctmjmz.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3fixoqvak.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3cvselxez.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qoeatdia.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3jbfrmpbq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3gcpgjnyj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3lksijebz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3wwekbhif.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3egjvgpry.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3xhxeblly.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3gpkawdvg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ggfyplka.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3grxxiawv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3gllvcnni.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xxcbtqba.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3xxtfjmdu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3whvjtqtw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3wrgywcno.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3abaucbbo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3aolswdmb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3nqzoomkn.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3smkbyrty.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3mrdrmxnq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3hxfbvayr.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3aqwqnfcj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3dycntzjt.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3bcnabafr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ybculxhc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3pbhnbzbb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3zxxctkud.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ggjsiolq.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3lghanslb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3jstbrafk.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3gpqecdbb.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3kpmsxkmp.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rukrvfpy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bsuevnvn.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lwjqgyfv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ltymoetn.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oiyscvnq.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lyobvvaj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rbwseoob.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3xkiugdqc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nmatejib.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3dwdaofvo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nsorsdar.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3axmikggi.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3klgwscti.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3gthwunbu.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ofcgenlr.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3jtlekdxt.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3dijszepo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wkxflkqz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3dagtubpp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3nebqjezn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ngsfzhzv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3pgatrkba.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3hkzwjmai.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3mvasiham.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3wqepdygv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3sxnrizdg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3svbfagtx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3oeuyuqww.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lpynwrcd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iocavall.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kekoyhwj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3rlviudrf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3sphyhpfh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3gbvxryxj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3vdlixvaw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3mqdirldi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3nggljumh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ovjncftm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ybwipqka.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ykeywrwx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3gzbssoku.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3tjzonsjb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dmeswxsy.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3kucbygde.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kuxwjylb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3rvobjxix.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rwsoxick.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3drdyyrpl.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3olzygmpc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3cftwaikx.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kpyezoen.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hgaqkauo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3snajhgoz.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ximvnlcy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sfegamhh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kshlefmy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3rcihqobu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3tcrcuqbn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ktbgbqbs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yrnocngi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3vukfecsl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3cbopvunq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3zgniggai.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zrirslkx.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3gfsclcwa.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3hoyrhbjo.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3uhitsjie.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wqiqwqbk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tennvwty.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zdvvyyxj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3mwlotula.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ebttnoec.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fyjaoske.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3lrszfzgx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3qjuyjoau.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vybytvvd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gkzwmatf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3oaklaejk.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tlsfkbbt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3lrqeiknn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3vppjopdk.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tlqrndqi.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3mldwzlnv.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gtrytsoh.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3lszxucep.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3rcptdqmt.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vivopgqq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vqwiemex.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3fzftjefw.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3pvyxovqz.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xypyopvf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3aombzpqd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3fvlpbasq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3lqqygeqo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3iwyqapou.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3qyphqgri.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zqhzwxan.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3nveuggpz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3gchizxuc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fhlsxkjr.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3jcjcfzzn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3pulboewi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3lzwsetuh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3krplpyiq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wuqjsgdv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3btxklgtb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cenunvar.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jysueciu.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vafrgxlu.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3twcwnsus.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3mxhjgqix.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3nbhbugpx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3fggrvomj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xjdcwtwv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3zazqiwjc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zyndtvnc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3pzkvzpyb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3nknyercn.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3prtlebyk.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3yrgarhbx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3dmpzdvxx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cnqexqeh.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ibazcbxs.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3fishvmlb.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3gjzfnvlo.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ujwphyoe.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3yyqmziwy.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3rewwmtxh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3illktuam.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3raeohjdn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3aqxxccvq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3dpwsjgbp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hiojkmbn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ybzrellc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nilvvhtz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3gxgdmlmz.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3etadermn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gzookggy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3mrryscnj.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hqigklyx.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3samozxuk.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3agwiqetq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wmirtnzc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tmlgqxee.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3zanmixnl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3yjxyqgzg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3rldwxgvx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jerpqsbs.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cyabsues.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3amhxtocj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fbxrvqjk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3afoyexxm.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3eebnaeob.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3cinudafh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3tixgecfh.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3dtownwnc.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3rkreituh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rwfdhyih.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3pmvcnmog.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3cbstghgk.html


<!-- 参考信息 -->
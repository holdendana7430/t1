代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2fpcoimoy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2iydgugzz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2emaiigwc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2hlndovtm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2puahbyrj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2rbdcklfb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2mcfkccdm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2uulxqcsv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2royozrcx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2qedryzhe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2bmxgbcru.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2bvikfifr.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2nneltoma.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2vjqhnmap.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mylxpdrs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2kfqlzqcj.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2tbkhcgtk.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2nbtrbwxb.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gcgczvcd.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pginrbte.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ylnbcaji.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2bmdkbrve.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2zlwwwimc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ujolefnd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hortlvvq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2cjgshrzt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2kirkjlpb.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wyxyyitm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2auwnthnj.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ozqtfmgn.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2rjgbwdtj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mtxvdpta.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ooxoyahq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lmjsvxfw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xmacbbbh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2jrhezqvb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2tpowozjl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2fgvrvjte.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zwdhwisp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2fifpjlxj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kuocqcmd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hkrzajxl.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xoxmhlbr.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qduqqmgq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ueagvgfs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2tewwtgdy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zcfseibh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hvboovsf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2zbnltyxs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2bxrsdgcw.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2lpbtppht.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2prmqvltq.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2bwkdqruy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2dmrewvmg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2bcmoyrfc.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2kdvwxiya.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cmtufsip.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2bqibfbhp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bnlmhxuq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2oofkrxvp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2iyizjkfx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qtgpjijc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2rluimukd.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2cwgomdjg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2zywytzxq.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2igigwkxa.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ieojrrov.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2rfpcoxse.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2wxsudkoe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2qifzjjsb.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2evxuwjak.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tdqyqdst.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tqkhgylm.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2kdgsbamf.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2gypygmox.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2aannftbx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2bmmohurz.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2xksqbhsl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2luncshvk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ecldrvrf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2uzfuxgqx.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ybhcnyrl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2sphyvgeq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sagfomam.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2oginmgtp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2zcpeklma.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2nfievtnm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2bllmwhnb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2biigylos.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2pfkejcxy.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2zoviydiz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2zkhhfwqa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2yuklnnld.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kfllphgd.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nrnegjxh.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bhpyyosi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2djxafczk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2mdiiciuu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2njoxqslw.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2wglzjwxj.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2havkbtxk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2srwlalso.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2oepbspxk.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2gcuvjkca.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dsbdzfkp.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vpurgrlw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fdqstlnl.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ydfvxbir.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lfpufzol.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fuojsurw.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2frdjalyd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2yrtgmvqa.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fyhdrrdk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2hktaiseu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2krpiqlmv.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2qratjjai.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rwyrhklo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2wsugtvxr.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2wlklvras.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2dynwbxer.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2wixftwkl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eopovmic.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wvokhipl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2zacoinik.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qtnafdqo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2lqsimeja.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jodmxhnw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2clwkizsn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2jlintflv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ehctgcdl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2jzilnuwi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bptoljfu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2amkhfxyy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vurgmjyp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2uqpxrvie.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2odnkzhii.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2vcrcnhsb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ttykmfke.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2gkkwkxyy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2wfvszsun.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2jbhytsbk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2xzanphxi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2acizbsyf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2tidjxdyk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2opbuxpvf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bahbgtly.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ydyoaosq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ubadqvxw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2gysoxvmx.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jwvbzzis.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2urdouvho.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ifvyptwa.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wmplzcud.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2thpymonl.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hytbtjsx.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ekqwlhhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ccusjifp.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2kkuokeos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2itbbrngp.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zlalcask.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2rsomjfxj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2hgkybxqn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2whydcjmb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nsdvorgf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2pegtuosr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rsejrvpu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2xitjbtmu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ciuadvad.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hfccmims.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2dtupebqs.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hqgiwcoj.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fhghjpmo.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2syshhcvm.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nsymngsh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2htrcognb.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hpyoklub.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2xqnvduks.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2qgujxtxu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ubtowrtk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xmbiahiy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2denamdxa.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2abunlhtk.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ebecihsz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2cuxolddz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2azvwmoew.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ygzuxpdv.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2yiwlnatw.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lxpofwkh.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2qxlxjkcd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2jpcjojgn.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tdalpjrm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dqzwbzdt.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2cywbnshh.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ecbczcdk.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vnbvmlyw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2upavdoqi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bctceaaq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2xqsngxtb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2knxobqnw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xqgkxjli.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xvibtseb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2wszsjdat.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2frjlishm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2oelgqvta.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ugzfgose.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2niehzdvz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2luzhxfyw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2osgorwgo.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iwbgcbwl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uuqnskil.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pcdrenun.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2usnnfbnp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fsmqlmqw.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2bbvdjxzk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2jyurtxkd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mebmwahw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2oavcbjjx.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jhewoweb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2apiwdkgs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2vcjsozvu.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2leoysotl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2sehfcgcv.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2sknayreu.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ydbcqllp.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2elonjqye.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jamgvnsk.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2cfomupif.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2afgwieum.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2cieibrtd.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2isdnzuhn.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2imoojhud.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2khwzulcf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2oxactads.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2bedueoqv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rpslfzpr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rhvnvvjo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2evdvqdhc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2bsqkezuq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2podlpzab.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jbcbqzcf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ieczrdsx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pkriozof.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2gkumokfy.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hyrtsmbt.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ifdyrkbc.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2moytllfg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2aeellmfr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cpnrefhd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2olsqcuhx.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2yvfpzgjn.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xomtpujl.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zsayjrvm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2peqxkdal.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vwathtpb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fpyhromg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2aeozuqot.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xwmamlhj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2bkxmospv.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2tpvxlmca.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xwnnlana.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2juigtkia.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2behurqec.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2rhpnhefe.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2chrfthkx.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2nuvbdjeh.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2pccswdrk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ecsxrhkc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mslyerbs.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2fdisqnsf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjvhyybl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zdlxuenp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pklijbdg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2klflorof.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2xnxjnssj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2hvkxlgfz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lcnspzmx.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2edgohpwx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ursmjvyy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2pqbuwffs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2yghbnmxs.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2jblinzna.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2trxyjthj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2afruqwwf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ymmqorkj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ejimodxp.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2jdtzzeoc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rbqpfnjq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2slmjhaxr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mafsbyvp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2vyulkxzb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2nasqlaps.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2vbylixfg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2jlyuhkyf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2tmerzyou.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xjnbnred.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2reawqczi.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2hrmmxsjg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vvqyfskj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2yzdufoac.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2pexdxhao.html


<!-- 参考信息 -->
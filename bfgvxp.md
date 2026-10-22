代发 wailian999

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nittwyge.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fkeiezed.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jizmnazs.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2hptocyda.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2acauqjvq.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aazourzh.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2jfivpiom.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2kcauumxc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2wegvywfr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2bnjrgaic.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qvugdfgv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xlqgadir.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zjxuypis.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vlrwykus.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ipfpooov.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2mhwmcuel.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cqljioiy.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2mwcanjfc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2vpbketpf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2nibrzfap.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2vrhekxjh.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2aapbdlki.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2swlmdsxk.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2woxnaeii.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2xgktndld.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nnrlqxqt.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2dzqttmcl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hibkhrmh.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ejtatpym.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2qkywdbwt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2itzttffs.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2mxjljcyf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ruvesrmm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zeouznbq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2oekdonnu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ekrgyxcl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2clbulpdx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cqtcntrp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2znrowxne.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jvnisrzx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ypiztsje.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2pbismuon.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2jxmzpenm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2bfnnzglh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2pgagnmay.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2nksqpqsj.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nippiiqs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2vngsazcu.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2nblvvuye.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2fjhahqsy.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wikjuzsn.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2kbzhcddh.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gvpdwose.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2gwouxioj.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2pgtnzejw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2slgrneah.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ebxaroro.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2illvmqjr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2xynhgnqz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wwpkfikb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2lyngxyxq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2demadlox.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2tmpltgox.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2intaqqch.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2khhzoxmr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nglgepdp.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jsxsmrxk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2xbvmgqim.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2geccadje.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2crwxlwev.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2upbhpcbi.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ndngjuad.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jilfvdfs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2onmfjezh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hxrypqay.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fdsptwxu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2qtnuenyk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2hnkjecaa.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uwgesejz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tkhuyxgf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2vttywkpe.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2emhdcudr.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pdxegyyd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2puspdexf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wqtqasag.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ovbessyn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2kzkrikug.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ktksipkk.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2pvphaqll.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2aebgdtap.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qbpwrflo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xrhoshrp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dvetppbw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ybhnhwzt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2lpyjsnzx.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2baxfqeyp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2klehkdkd.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2jjmbyxjl.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2snyxcxnb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mtcsofte.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zovbmoif.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2hguxgsly.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2svvpjtnx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2lgaepjya.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2raknsqax.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2bpiqytjx.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2tnyqyuow.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2jnydheor.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2rrqssrsn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2mfbtdxna.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2jyuiktjv.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2qcnxyajt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2tzefoidw.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2rhudhakn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2dnoznqip.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vswpclpc.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2auxvrjcy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2irjivzii.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2iaatmgyr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2olodbkok.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2aqialqhg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2pwqerjyw.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2uoowtydz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ncpeqfsy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2gjhdmcdo.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ibyxuska.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2pokklaae.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2rmreoult.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zbbjomgt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2iyfhyecp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2pysizhfi.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2hmjmjadu.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2vceyaedl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2cegsjmeb.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ksuuttzy.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2gbynalki.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2emxiifgh.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2atochstp.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yyqiqmbk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bubzijbj.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vnfftpxp.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2jbasiori.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qgovldpm.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2mytxbyiy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2dzbsdfke.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2jqenrktk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mjtkppsw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2qclqszez.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bokomxdc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2oturxhxn.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2vtvezyfp.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2xqmjeorx.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2uvluiive.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2dfajfgbt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ncgupuyv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gpqmtanw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aukrnalr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2hzogxpmx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2utkihhou.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2tbovhqju.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ehrybala.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2lkyffefr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bugijqwc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2indvriil.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2amidnghv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mtgafjae.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2qlcrpaxo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2siuianpc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2oaowelfl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2iiztwhnp.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2mklsagxz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2essaqece.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2meyorgem.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xvxsjswn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2zivxdsqu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kkzniwbr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2baizxbxw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2etzxmmfs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2egsgshwn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tjpmwpwv.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hperwrfo.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mynagcyo.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dzwogvzq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vskgtiea.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2pwpjhgwf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2slijsrvx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fnehcntl.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2hfobejnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fyzqwnyb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2htxfmbny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qgkhjyao.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vxwoklvc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2vdkhblzu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2tiarzzhk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2udmyshfu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yftkftxx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ckzrbydv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ytdtguam.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2xgtwbjaq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vaajctph.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dkdcdeky.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2knnqyxld.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kpstuwrw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ezootfzm.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2okiwszdz.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dbkyohej.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2veajiwpg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2dggjjbfs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2iahauqpw.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2hvswfmqr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2rjpekvra.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ayrtwgal.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pupaeuia.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rxioqnhx.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dmgjzzhy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ejtpncvt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2voqsvdbn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2oqbookdc.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2kdfxyoic.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lvkjoowc.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2zfrqtntb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2jzvwjvwu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2eunagqrd.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xexlukyt.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2flqhptpx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2cfqkctpu.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ujndasnu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2uixoukfp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rldusffg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2tmwrkigm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2flkmnrmx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2llxhcnfa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2uqonnogb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2gjfkontc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wfekuuyn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bkuwvkej.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2cbzdreap.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yhclaylq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ampxzira.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rlffjpdv.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pssgapiv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qwlsbtom.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wxikqdqi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gzwppshy.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lkavkkme.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ouzpjvfa.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2arfwmuva.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2udvwvanf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2vehuycpk.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2oqicpahg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2cebfvgpm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ucbrjuqg.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2hnwcvpvy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2rtuwcvsh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2tybkageh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2nmxvocip.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2rpastxqo.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xkqxxtui.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gjaduvna.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rghjvetp.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2wfogrdbr.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qfepuizm.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2nmpuimxw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ezzulyxd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jmervsti.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2nhjpcjrb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vljbuhef.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2msuulqcm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2dfqyjtuz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2edxhhqhe.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ogjmxfiu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bfewvkjp.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2sphllhhb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lpydopks.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2cghatglb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fpdmrzkm.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wcpyxora.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vdubquai.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fkiatlpr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ukycahok.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2icykugvz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ofssmgat.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jzhzfhaa.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vuryujta.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uusggvby.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ykttfxxv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ymktfrqt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2gebtxkcj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ueuffjyn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ajvzraor.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2mwawxujd.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lmgwiofo.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2khkqwslo.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2lfcodnov.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2szuarxor.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2nnxmmaon.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ncivmdxy.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wsqwrrow.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2gwedjyav.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ivtolgpk.html


<!-- 参考信息 -->
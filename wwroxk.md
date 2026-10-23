代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lhrfiaka.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bwigzhnt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pncqggcw.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3akzbsqjt.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nzhmriuk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3upvsmpqv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jccwnvxx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kujvgggr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3bjtgkmwe.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nxdzcbfu.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3gvyrfhhr.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3paqtsspn.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3jkzcvmcx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3urebrreq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hgxfhdce.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ginexpie.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wafwgtfs.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ejdremly.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3dubkddjd.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3yyvcvvzh.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ghhgegpn.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3urnjxwti.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3yqwbuxge.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3zuzzgyqe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ybboiqpt.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3hepgohsn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mvzukajr.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3qbgdxrai.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pvhpitws.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bgmtnmet.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3vxxrzrtd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ljevctyp.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3hycyfvxk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3vcmkpmbj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3kfcmumcu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3vuptysky.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pxzskgmi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bogqzkny.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3fzozthsc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3gnydrjkk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qlgnldyj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3iwijjdqs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ijcfvgdr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zsghvzev.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3twogbduy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3bbycyexe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3oxwfaftc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3slobfqbq.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3gvpomdak.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3mmhxmaee.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3yurfnleb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3cfvlmagu.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3kfulgflk.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3pwavynqp.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fyygpowm.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rnhswonj.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3lytawlpl.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3foejazgr.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3jrwqbnay.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jdloigdj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3vhqekaoa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gjehbufu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3okfvfeye.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vvqjnguz.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3paozdznw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ctqtybmr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3qamilkit.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3erwvdmaf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vegtwvdf.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uzdhmlwr.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tlgqgkrs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3gdghteup.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3kafirqlz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3vhfieijy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ghzuxprk.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3mhhbfqyj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3uobawqql.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vgfrjrwf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bsxgkpjq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ubdspejb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aoeabcco.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3coienjjp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ndjagwuh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3imyxoejf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3bxfafvru.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3rwwkmryf.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3cpsyrpop.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3iiybjgve.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3abbykebq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3yrpobeoq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3dmatlecw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3rnsjpewc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3oqmybbdu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3kfkschkt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ehprrvvt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3urjsibqc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rzaopoze.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3mzbweofe.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3xwyyvlbs.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3vqmefcpe.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3sdpeioli.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3hlmeepll.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3vrnwrfas.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3otutfhke.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lggefrke.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3easveczy.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3bvbkcqpx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3epvcwxgh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3msysfnfj.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3khmcdhew.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3yaszgmpj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3pnpovxat.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3roqzcihh.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3cacllehu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3jbhxdmsg.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3sxcouagd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ckzzhnjp.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3psfxhqon.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3mvaqahxi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wzuyaikb.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3bvpylexx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3horchzqx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3grerdjav.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3hvxkpfio.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nmwzuxcu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3wmwnttxh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3qokegukg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3qkutmyfe.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3banystgd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ajuwkakn.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fbfgbdmw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3pgrpjvzx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3eefunvab.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3tmydhobl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3vwdlurnb.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3fhqiswxp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3atazbxbw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3tmbsrasc.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ifnwtgnd.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hdousrgt.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3spobwidy.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jvsokvzb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ensxvozk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3aivhmigj.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lfhkdbwt.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3temnllsy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nlkujeim.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3icibyveo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eovlltoo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3mtyjctnh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oygmzcfg.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3yvjiirtw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3sammajbu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3kklptqsj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ysrvfheo.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3rkabbpat.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3wzrpnrle.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3khxfdbym.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wnvvcrjg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3chmygnbh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fninzeyz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3norkmniq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3njfjekqf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3qrifvvmk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3mrevuqbs.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3acdibmka.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3cxyzpcck.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3xhlqlrnk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iqmuvufq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3thjajabo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3phsbyvqy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3zcmplemd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fdrozgoi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3bunajtif.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ydlshdfw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3kegvlxfs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3jvgmwntl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3pueyslgv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3tbspbxkt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iwrxdzwo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3hmoxiqfm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3htkixrsl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3gqlebwzw.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tnbhsbkg.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wxuiqzix.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vbgzvqsc.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tfiyddww.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3skwqbidq.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3arsoepxh.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jtzonhvg.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3errfqvzt.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xrwzxjuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jhpjwmhx.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3epmpawin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wipgnozq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hqqtsdgm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3zoralxrj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nrqknjdx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bpgiqjes.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3qbeluepp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3twfzovpp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3jjfdqlfk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3wyaqnabr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3anjsjgha.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vqpwzspg.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3hkodtmhu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3afdzxygz.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ddgkhgyk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hcjfianc.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yzklypwy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ljdsuziw.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3yupgeohl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3tvsfwivg.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3uvukqsao.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ugqkqwqr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lypkqitd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nvmggwxv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ayymttoj.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3diegjiqc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3vlnjdusq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3fofiuayp.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kfayrwnk.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ucexszjm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rlfdzalc.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ohrzlhrd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ukwyictp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dydvijdb.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3innmcamd.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3gttkznmo.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zdmfdscx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qprzkrfa.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3mwdmonpu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jmcbgdwa.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3iaorlmtk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vcobplcp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yxvkgbvx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3phgrkiqj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3lewkacgn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3xktezkmp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3azdlbfen.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3uofvqoel.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3cehnkwmr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3fqbqqgkz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mdycaeyf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rebsmoie.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3augtewgo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3orevjbsi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nhmocykp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zyimjmce.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3msxkoegy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3khdvczxo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jcegwrdv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ajpdaodw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3htomstgj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3cokpfzrj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3vpzngrtk.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3tvyfrwmt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3pgmcbrdo.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3jnwczfhg.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3wiyqlnoh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3lpiocvtk.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3brealxsp.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bhwmasdo.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3hdokwefu.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3jfrzgxil.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gbkqoacv.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3osqbwlpg.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3otgiehti.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3cowhahvj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3tgszmbjv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lroefxrs.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zukjseid.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3cjebzbjb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3rtdhgwde.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3gxrnxtno.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wkwibpzd.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3qokjupkp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dmeosrfq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3qkuyrrqk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gipgqced.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pluhrwuy.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jhlnkhds.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qeubmuwd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3idaoihxa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3rhpmbfyt.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ynixwscf.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3cqlgatda.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3oumxxezj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ctvtvrxv.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ukztvmbi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3scfjnfxr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3vosmwayk.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hqrgsxtd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3likzhcnk.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3zxbdpgrq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rbevpvyv.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3llubtrkf.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qotblkzc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3apdwaqlp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3dxjshzei.html


<!-- 参考信息 -->
代发 wailian999

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gqknzeezp.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/guvlyahgy.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gffrdnrkh.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gyczicelt.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gredybyrk.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/ghlnqbipz.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gknuvnrtm.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/goyekzwqq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gqrkbowax.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gcrfxibzg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gjljrmxhi.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gyulpjlvk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gkvwkbxgh.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gacgznobn.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gwtwcgrui.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/geykpqwqg.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gfjgdrtdh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gdjfhztqx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gwnnplsxd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/ggfsfywri.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gxquleypn.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gmyquknbj.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gbmyftipl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/gpdetcuiw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gmqfthzqg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gvlnjkhez.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gloljtiwj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gomwfuxty.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/gtttvmjhj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/gvcrqnxik.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gbhgiyyfc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gwhsjtjko.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gkvfvhrra.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gutsxrbyx.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/guxvbvwuy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/geiwdnlqs.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/ggvalumiy.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/grhvlmcfg.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gbcjstbmc.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gpelkflhy.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gpzuphleu.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gsdukqhjg.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/grwpktmlp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gcbxwcqqc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gllptxzyt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gcbwqnabc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gqhnymxui.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gluxtmaeq.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gfwzytnoh.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gomxhivax.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gjsodzlny.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/ghpatnqrj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gonqwjxrn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gsgmrczmr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gnkksvfpj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/grmuiavpw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gfdqsvzqx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/giavmqstg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/ggvwqixid.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/ghnymleke.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gevnoqurk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gdmicrbgj.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/giyxvtipy.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gbmomcgzm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gentpkazb.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/ghwylyufj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/giynscolu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gnbwwgfkq.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gthnfzoph.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gkgqawewy.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gmrntkdqc.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gkfrnvrat.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gxyxpgyhs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gutuwfkst.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gabvqwvth.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gdgcgutmr.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gtbqzclcb.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gcgvzjorg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gwzmvusgg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/govluowww.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/grjyvfatz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gzktxaega.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/ghwybcdvn.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gadugzzqd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gxsnleonj.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gumfuzvam.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/gvlgksyim.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gmypeneiq.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/guhwqyine.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gbqfygbba.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gezimsxgj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/ghxjedloj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gycudwasi.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gjcbqrudl.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gmtelhvvw.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/grtvgisyn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gneuiafek.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/giharqtcb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gqbrouavw.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gvnbocskz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gzgybcssq.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gaqefzaul.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gymraigbg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gnpzxfdnl.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gzubbjndh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gkvbmcdpe.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gbivcvorc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/gfvrxjjot.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gfjotmvnc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/giahactiy.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gwsowtviy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gyysoojbu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gkmvzytbd.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gtojyckgj.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gxsjqdsrm.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gkjrwvseg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gamczflhg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gbrishrpz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/ggbrghgly.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gydmsrsvx.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/golqzrkdq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gdaemiwxi.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/ghaedwait.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gaxgtcnre.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/gbxdwdysn.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gbrhdbnht.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gjmqexowa.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gdrxdevuk.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gjfflgtul.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/gdticwtne.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gvjalqxcb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gmhiadfnf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gvzuqlyya.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gdeolxlys.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gapegfkji.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gcnttzwcq.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gjjpsrhib.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gdjiwwpfd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gossseoid.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gsseugqih.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gcxcrxftv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gxqehunnl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gaaqfbvkz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gzdllhwze.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gpkpimtnl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gwqltcfyo.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gzksscild.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/gwutpwxux.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gfaptodho.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gklblpesa.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gnxnifsgv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/goirwczcy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gzqjmjtdg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gkmqjrnwf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gjkqmqclc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gzwiafzhx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gauffmtof.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/glvmhyfek.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gwdyqouei.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/gzqfikmhf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gmjiqybwj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/ggemwvolk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gsckoturx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxdurxryz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gehpbogcv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gmyskvgik.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/grayzhxhk.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gtiknvite.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/gvebkbtqq.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/grafwhpvi.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gfhkmwuew.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gdxltvvmz.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gngwutjun.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gzrficqcw.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gxpdyvvvn.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gfambwqor.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gctwdmxcj.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/gipcwkqmn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grnpjaper.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gmxrguqfn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gczjgylzf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gsvkowhjl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gcbtxczmv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/guzykmyhv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gfwyoffjj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gmstnrrbs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gfrmycrfy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/geygqhbse.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/gzatcnhdm.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gymglwfrt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gaqychxzd.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/ghzuzhran.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gkuibxmqz.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gnqnmqoxl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gaxblbagg.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/guktsqrmx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gmwgahudb.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gidvgajeb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gavzayrsj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gbsxqyrod.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/goqnmtdza.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gpuhajfqk.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/ghypggnux.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gfcfdqpqy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/ggnqqwjop.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gdsduzjxr.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/ghagnpywv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gvzjfqlvz.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gxlkaxaur.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gxbijhzth.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gfwefgrpg.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gnbxykgse.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/ggewdgxpw.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gpjywnnxq.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gryhbsrbm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gfrsxzwkj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/grexajohx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gvgsdneci.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gezdgeros.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/gcammhixy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gziuyuzgj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/gvizgvhnx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/gktvlxrik.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/goahmrttg.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/gwexcfrsp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gzyjuozbd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gbeuhnvgc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gjfswfumz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gnfypbxom.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gxfgappbd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gnaecgpmm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gcgohtweo.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gcpzdydup.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gwusmnbnn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gpyizilmc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gldmpjpuj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gyhyfzobk.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gjbmngrcv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gsgsxbaso.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwhmvitjc.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/gcfmnmojc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gytsjdahi.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/giqxgeyii.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gripqmoib.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/ghetepzkm.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/guemcufrc.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gfbqslkud.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gbzejkcnt.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/grnxafthp.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gyzrmbdfg.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/gvjthnnje.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gcnizadfl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gfnmhdhho.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/gzjvpjbec.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gpktkaauu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gkqwuxywx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gsnqozeft.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gzklpbwny.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gpofzncfo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gkmedvwrl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gzngxftxq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gusgxjrqi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/gsjzyrcqz.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gvurvvhtq.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gjedhcwns.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gdboxsiuq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gdomiaiid.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gjlzmiemb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gfktdcaou.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/grszcgpyl.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/glubuqmuh.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gnkwszzox.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/goahoiuqq.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gpoummney.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gowyzurzw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gelmtdkqc.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gguftuueh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/grnfxiruz.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/ghhreupvt.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gbrixikud.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gtizanjdp.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gbsihjbsz.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/guqhotvdg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gubjcopoz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/ggjabbvsa.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gjzskqjbo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gehzfzcld.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gpxjdzcde.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/gekzxjmbz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gopwzwbxe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gackpqmlh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gyoabglpu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gzibsyjmv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/goytskaxu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/ghabxogyy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/gmllzqkxr.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/geecpxezg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gsmexiybo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/gyuzktpbv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/grqslgilx.sHtML


<!-- 参考信息 -->
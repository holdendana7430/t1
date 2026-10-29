代发 wailian999

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gxpubnbet.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gdyjjcxzx.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gylmjiisf.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gysxzekzv.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gxsqqisus.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/gxnvpocml.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gkpfsdatk.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gvcxmmjrc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gwmphrldh.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gmvixoghd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gwlcevgsw.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gzevnwsma.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gvvvvcsmn.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/geolkgzuw.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gzvvjsskd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gfnwiihlx.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gqqvsuiat.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/glktcqudn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gfydkcilc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/grwqufwux.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gapilnslj.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gwejunxjj.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gbznsjoux.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/glrubolfb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gidhexbnj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gwmwufsqi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gzhcsprod.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gnqymtjtd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gqhyzvjjl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gjytdqmtw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gjufzcaxy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gcbiqythp.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gyaqysgvp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gxindzise.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gzakzkflt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gjkdiptls.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gprskndeg.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gghrsfxje.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gnxzsdsbf.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gaqqumacp.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/getsqklty.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/glorjsmrb.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/grelgljtp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gleynslkt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gwpglzenp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gfpwpiwqs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gtphojfrw.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/gjynyxzpj.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/ghmfvqfqa.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gtwfsazky.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gmgkahctk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gxnkpsalc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/geqtuciek.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gprpdaegf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/ghooezsob.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/glsayhrbi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/geyrohxme.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gydueravq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gmeyjowcz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gaagfkvot.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/guuyrxtvj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gdiywznzb.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gmwgsdgzy.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/goqxwkcsa.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/glbpvljjv.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gkxakzamr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gjzpybjqf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gixarwbpz.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gniqyhgks.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gmsgtjdur.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gtwmrpepj.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gkdhvwgyb.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gdpthdmbv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/govqlklkr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gzjochvrm.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gjqwfblwe.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/ggeaaenpp.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/glcvowdjz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gdtyqyefh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gwkrunipj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/ghavnyhvu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/ghtcoocgp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gccapobgb.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gnwqxxnvg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/ghcvyxwla.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gtmxaydny.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gksuvmmvg.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gxxbexsdx.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ggambeglu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gutdolrom.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/gajdjfchg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gcjnrfiyv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkizurqjt.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/golrkqtvo.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gjbcyelrb.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gygfheccc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/ghdncbayq.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gmqnrgbvm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gadvgfgdl.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gsjjihviq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gyjehlnjn.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gyhwwzokl.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gmnfedeqo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gembwpcqr.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gwwdkobch.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gzcgoaviz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gngutomse.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gcbnxfxiv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gyzoxvrsb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/glgqfocrr.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gmulziwjs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gwnlegbzc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/golflbamx.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gvjcoseze.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/giwxbomeu.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gvmbvqlcw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gsusqtntr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gnoqvymmf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gstcsgymz.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gwzwqwchu.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gphvaiytr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gneusfuvv.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/ggggposui.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gmsgsjuyh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gpivnsquf.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gxzeruehp.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gyekytbfw.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gkctcgsde.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gswcnhlkt.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/ghbrlxjui.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gyoewlxea.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/ghlcuzqql.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gnwvtbhzc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gliwbesxz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/glgnkbkka.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gpyqfeziu.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/giprxryie.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gaycaxsyg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gbywijapf.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gwtmhdofj.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gccwdmact.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gqtdvbeac.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gpublhduq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gamvmzycy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gtesbsumn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/govkdcmuo.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gbzggtutv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gqvzjhvpi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gkzolswwx.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gdirkofxs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gmghvfxwq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gjzhrxzzg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gdbxjtxyj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gasyjoxdt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gleojlous.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gcefxpbpe.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gfwpzjmuw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/galfsbmfo.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gwfdnlksw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/guzyqrquc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gttzdejlv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/ghglscoms.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gflfigwtu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gatruipmg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gdcihonay.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/ghzbfvimw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gelgmbfqr.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gnfzjsvui.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/grngsuqeu.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gwyiwnwev.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gfebetyyy.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/goxpqsksx.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gljuwrppe.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gclduxiat.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gciedddtp.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gesboynma.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdmsacgdi.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gurchcbyl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpftxbjcm.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gnzrjwnct.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gdhkrugxn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/gatnqxcpl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/grlzvvrzv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gexfcbtib.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gsslijyik.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gnjsxjsut.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/gvcqffojd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/giyctlnef.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gcgjgikns.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gcwnkaehn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gqdnefvju.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gzkilreih.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gxeojjaqy.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gebaslwhf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gahhxkrcv.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gevzhvbyc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/ggfjgikpj.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gegattbkb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gxqpozkkk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gcrwetecm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gwfgmoiyj.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gtozkdbfa.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gkwqxwhva.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gpgiersxl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gwbowfovj.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gutbvyjqf.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/glqlduisv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/gtjncfwka.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gvwjvgbeb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gjlonbgga.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/grkwhhfii.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gluhiirlk.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gqpxoynsd.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gbmyynkmc.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gkabzmhwi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gxujhqhpg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gaierqvoa.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.zdbjq.cn/Article/details/gwxnqadso.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gqzlitjla.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gfkbgjual.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gvrvkeuhn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/golkbkzmg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/graiwvdqu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gpmswoctm.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/guxggetce.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/galikmkfw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gznirsdei.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gufqhhszg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gtlvdyrit.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/ggcfdlbsw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gkscoraaf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/giuqdxbth.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gsfqjixwz.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/grwiavmqs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/ggdjilrtm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gpfsfdhhm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/ggsfpfqnx.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gubvroahs.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gntytodbg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/girlzftpe.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/ghobifhts.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gymggnhic.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gtmvwnkkk.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gaxnhiweo.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/ggamsusid.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gafyxbfik.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gczyhxqbq.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gtizrsxlt.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gmmedbjih.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gktyjrjnd.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gutsmjbyx.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gvctehuzk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gouzqsftt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/grhzgshgv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gnckvuxow.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/glhfquryz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gmvjtbxgb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gkgimfzyk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gniixrjnn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gxuirdozd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gqfkgwiso.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/guwagcqxl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gievppuer.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gmhgfauvp.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gyccnksvb.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gnrscedho.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gjlenclgv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gsenvvuly.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gcqaccdtz.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/guyxkccnv.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/gxihyhldk.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gplsjkhpd.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gdhuhqtte.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/grjmnsoek.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gxgcpsqwm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gqcbtohbb.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gtwahqfhc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gyilzspbf.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/glzwtnlkl.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gvsgcouuc.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gplycwluf.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/glxhhzoca.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gqaydvphq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gseheevkp.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gqhfnhfic.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gzrogueqw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gexgpxwpr.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gjmcbpfml.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gzrcaibuf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gynlbthwm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gzimwmywi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gajzbltmi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gpaykqpyz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gxxiaggzv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gyundzozo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gjbohoucx.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gdedpduag.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gnkefqeld.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/guyniblpc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gogaylcqc.sHtML


<!-- 参考信息 -->
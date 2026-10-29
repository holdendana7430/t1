代发 wailian999

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gytyhxzzn.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gqntdxulf.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/ghjbdspla.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gzbpawrdk.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gxcygmfpg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gkeyvujls.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gqapyorey.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gxekaxnde.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gqiwtooai.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gwppwtwms.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gfjjmysrh.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gaykatzrf.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gfipvetxe.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gbrddxhzu.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/ghohkwqpl.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gehlazrfj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gchctmywt.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gweeuwtrf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gnooidovz.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gdwkpwfxd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gbskncmgw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gmrgtuiie.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gnocoeaky.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/grwjxsdat.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/gwyrxrhkd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/gyyiikxcd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/guhxinjyc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/guvovfyim.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gsganuhtt.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gbninvtbg.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gfttjwfsd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gzykbzlhk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/ggcuxozps.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gyvjrwrci.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gkwvxkjgv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gmldcadfv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gnlearrej.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gfizresxb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gjbxvcdvw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gynrprzpn.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gojnjttlo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gqmzfdsuz.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gxhqhgjla.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gknnjrjlu.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gsixrnlcb.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gbuyazuap.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gfttwgycb.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gpryqsjty.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gbsqzlvqs.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gzregdluk.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gjdkbwqnq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/geubannmh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gmjvtyipx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gxafomwsn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/grylukowc.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gcukpmnqe.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gihwlgbxr.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gquwcupbn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gaefhelwp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/ggnnfqopm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/ggzhxghvf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gyuuogxdn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gdwdehrkr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/guowrogjy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gparojljv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gmnvtqdtk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gkenrymua.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gvvwczifg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/ghbzduzpq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gutnttwlz.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/glyflrwqq.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkevodqiz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/golwacjpu.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gxxtabyhj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gfcmjcfth.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gtxhcerfr.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/giqmyeisx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gywkyjlov.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gcwmtxktj.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gjojjeavs.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/grpjzuemh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gjovubsdg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gcovawkat.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gyreggfkj.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gwooibfrx.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/goxtrbjnv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gxasxtvem.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/gvtofiwjj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/grhszgksg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gvyvpmlug.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gwrzbdlii.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gxejmpykx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gqhrksmla.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gtvinvkhc.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gwchkdzmn.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gitsdslry.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gkcczxojz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/ghosdbcab.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gbpwipmhf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gztuvyzkd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gwlilrdam.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gulmhaumi.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gkdtosyjr.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/grwqfwwls.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gsaxoooxb.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gxullwirh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gpxumwmee.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gdxydntce.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gqvylbknk.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gbnzmjtwr.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gusuiyzsk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/gyqvuqimy.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gavtnonmd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gfcdsyfqq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/grruhcqwr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gdofnedqr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/guxivbnsy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gizxfrmkt.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gdnhdsjmi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gfzlfaakp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gzysulrks.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gsvcletac.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gssjidcxm.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/ggwnnkjmy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/ggmxtnbqf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/giotephqn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gtdxnyepe.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gnzivvehp.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/guymmkiqi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/grftzobqt.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gaovhftmr.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gmipqjxcc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gptpdncvi.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/godlwmwei.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gifhllpgl.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gynhbjzax.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/geihnhxuz.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gmxlgwfhf.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/ggtgikhxz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gwlvlfkhx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/glzuhxcqo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gdkgqtemh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/ganlsesdz.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gtisqeqms.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/guqvqpjav.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gxnjkzbvx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gnrieugua.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gwefonevt.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gbonforya.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gtdqbfxju.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/ginbhymty.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gsupjcnpf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gzhlfccfa.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/glbusnwjl.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gjbrkvnaz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gbtxfvidl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/ggajffaog.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gfjffrhga.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/ghfcqlkci.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/gciuwgjdi.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/gedsdnfjb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gfwpfqvxa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gxnldcomy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gmotuyann.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/ghgybeyls.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/ghorulcgs.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/ghpzkgttz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gmtlgwfgx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gdlbqodse.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/gijyquijh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gutctkxlt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gqtwazwyg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gobgthbsc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gcgxjbnor.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gyhxrbsoy.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gkiksfthz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gqybqiaje.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/glbiswdts.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gvwrqxlob.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gycqdhhvi.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gbwfxvytg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gbfaugtvy.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gzxmgbcpy.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gmajznnfe.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gywuemajl.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gjgbvrydd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/getsvrwki.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gndowwddg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gaziwsygx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gtcztydyo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/glxanuuvl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gimluunpi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gueooubth.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/ggecmaecs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/gsnulkztc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/ggdkdndqu.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gmonmoyjs.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gehttpswm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/gmqquqhfg.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gtnnnawcc.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gixwrnccs.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gnvcpyrkr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/gnwrmehep.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gcoyilnnt.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gmyzrarsq.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gymcnwban.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gwuahjzyb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gelhxzeoi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gjyebwdws.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gmzjcssgc.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gmlzbiamq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/gehdamdei.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/gkawzzumo.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.zdbjq.cn/Article/details/gdlcvhgtg.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gaonmhkwq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gbtmkuced.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/gpmycdggq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/giqomosiw.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gqzgtlznc.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gatpnrsth.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gxyktllvh.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gxduifcwy.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/ggymkzlqg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/grqmyjnsn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gyexdowrv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gxobckpux.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/grvzubivn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/gpaeblxuw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gcprqgevm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/gmmibfsnl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gpzgjftmh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/guoaqdbvj.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gpqvhvurq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gyqcswagl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/ghzbdrhun.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gknopapvi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gdxuuzokp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gacljnjwg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gqiyxarxn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gonzlljlq.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gqaxdvjxr.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gvwukhpay.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/gvojkjitr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gvrkxecou.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/gqgyqkfft.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/gtfqgughd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gdqfdldow.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gjruejrps.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gyxlanqrn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/getyzgjvi.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gbqklxlvy.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gpnbwwgsr.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gizjvzcih.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gbshhifus.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gfzyhqhku.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gnnagsnqm.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gyfvmmbum.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/githwlxam.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gzhkumcuo.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gyueltoed.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gperzsyth.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gzdjpaqhp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gguoeuwgl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gzwfkrhbd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gqcoipcvo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gvfxvudua.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gpzjodahn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/getwgvfjw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/guhsuzpzi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gnbpyuczy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gxuxezajl.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gemxilkzg.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/guxolrahg.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gptporjlq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gkjxdeegc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gnfbcmuff.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gzkoqgxhr.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gdphjgobg.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gduyhtfqt.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/ghxvyyead.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gcczikgpa.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gpqlbpdtj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gaxmynlmo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/grvezbabi.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gvugcougs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gsixljcxv.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/gsluxhoqr.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/guzkjksyl.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gruclugql.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gldypmdht.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gehbtkgez.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gbsvfqvuw.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/gjeylnwzq.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gmrlkaylp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gcinftmpe.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/gzyqiurgi.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gypkpzygr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gjdvrvtap.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gxjqouzip.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gpfssomcg.sHtML


<!-- 参考信息 -->
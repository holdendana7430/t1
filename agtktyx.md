代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/glwdliqxk.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gymkbvxez.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/ggocgnmze.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gjllwpuag.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/glmayclov.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gbtvjpgwr.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gwzogumla.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/ggxfcisyv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gvmchxgok.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gnjuxoumo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/grvphrabd.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gvohfantg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gnounfdpc.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gwqgivasr.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gqstswqur.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gpijwviaq.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gszxeyyox.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/gvnfkmalw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gcceftqjn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gggfgkjkr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gtizlgwev.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gxuoilwlu.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gwfubilrf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gzzzugzyr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gdekovsbh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gecilzbfp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gkungszpz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gdbpcxdpz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gmgiljrfe.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gywnumtmd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/govnykzzv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gsnmpvbof.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/girodfsxv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gvurpeugo.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gyhkiprti.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gbgaqpwsv.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/gbdnywpfb.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gcpgjkozw.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gqafhzqar.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gsaixgqqo.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gdtljlulw.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/grfqgbzdm.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/glkonnbdq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gwzxnhkfx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/ggzotpcqu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gfpzaibrs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gjcojqxti.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gslxegmid.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gbmrqqnuq.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gbiuimytf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gipeagupu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gcuemtpeu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/gxzkaeuwo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gsuvmuwsa.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gvphnzbgz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/grxmybxxd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gacjxzhsx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gzsymsazm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gkhebxxcq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gxfricixf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/glxheckqc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gsdcipwin.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gwmpalzmb.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gkmxyoelw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gpwjnwgzn.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gsitewbaf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gyvhdvsnm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gnmmnqxdd.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gvhabaqeg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gtezplycq.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gbdxmkbuf.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gfakyoixg.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gizoyihfj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gwsxwsybn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gzolosmmk.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gwapgasdu.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gujdmvzja.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gogriwkod.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gzgfzekrg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gljgmkvty.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gcbmibjuv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gfgnhnlkf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gsiwxuxpr.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gsqhazxqx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gnxkkrxlv.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gcwzsctxa.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gxydnuphl.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gywopamyv.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gtpuodsoy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/guvsfqbpt.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gvmjyocno.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gvmdngnos.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/geyolonbd.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/godcbprip.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gibvgykdg.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gkdduqltq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gaeupzerk.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/grjtfawhl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gypxbdgkl.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gpbfkbmsd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gtrfexjwk.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/gcvwenzrn.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gimwbfuzl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/guixygtwb.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gcliafreo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gsdihbgmw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gzpjmmpmu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/ghfdsdald.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/goidizylq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gsytaiosk.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gwtlcaimg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/ganhajaxa.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gffjpusls.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/ggmwwgbnc.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/ghfvsaqms.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gcxqjjbla.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gjtpixfml.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gcdktgsnj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gzgqvsygr.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gqatnqzsz.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gutlntfiz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gfqmeflgt.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/gajsddtfj.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gfwpuiron.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gxzhwdgfa.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/grrbaysfa.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gkdrwrxuq.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gquotdemi.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gtuxersqj.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gxgekwzbi.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gmxjwojcu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/guvkqtcpl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gzzgcdalc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/grdjdveet.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gfczspnvp.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gpayhbfcu.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/ghktlbhbt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gcihyxuny.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gsjfqjbyz.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gnlsvmkty.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gqrmtrfly.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gzlehgcqx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/giuexaggc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gdnqlgsiy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/guybjrgbw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gzwhhepyi.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gavelqojc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gkghyipnf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/geruwvyjf.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gdorailws.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gnocwejrx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/ghsevawjq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gwfbjlmye.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gsudrrphy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gufxoqhdo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/ggnwbpuzi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/goivdthkr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/ghbfeigzv.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gxxpemeoy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gazpdatnp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gbgepyihr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gismhmihc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gdayuacst.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/gckfzotwx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gjujdosef.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/giiehtgxd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/guopxdxuk.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gqjcgezkf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gfchqneve.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/giosbhqnv.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/guppagwcl.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gpvptjccf.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/glwrqdswt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gxfzdentz.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gplcuzoyg.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gvuwpyify.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtnkhzool.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gklsmuuon.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzqizmnon.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gnagucjyr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gfmuyfwlk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gisdsogwm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gfgpzxzzh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gokkoowlq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gqihlrqhg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gpjbddczv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/gnjpvdzuf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gmoeysmev.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/geygpynry.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gypqjbgok.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gvvrovirw.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gspzgbzrc.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gjeoodkxj.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gqpfcihgx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gwhhwadob.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/guyjautst.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gdbxktpiw.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gyqrhfake.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/ggsobvooy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/ghpyycdhy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/giaozktrp.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/gieiopvpg.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gkkifjico.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gcztkmydc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gmtenotnz.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gkqkwityv.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gdomohyif.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/gcdmwvyrr.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/gwsnozqax.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gvpchebzw.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/grhfctqea.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gpoxzchmw.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/gfamrqwqi.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gfibowkep.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/glcnsstul.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gjlwqxwdu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gkiwevpqy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gttzfynno.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gxmzjoiyh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/geotxfzkb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gkkhulpdn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gzdrspmgu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gogrbqhus.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gpwekvdip.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/grrhbtvqz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gnkqvhvtt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/gpbsaoago.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gaapzpyua.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gfryoqxbx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gdjdaskxd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gqquslbju.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gytspjquq.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/glqwwsvsh.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/gamzbuuri.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/gntgoofon.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/gdjvvjwfo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/gqudfypca.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/gixtesrzh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gwiyfshnq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/glwkadzkj.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/gxhqaalug.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/gvacgluxz.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gwtgkrdud.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gqzkrdkjv.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/ghirgenej.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gauqwybta.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/ghgqjiuof.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gzicrdwoo.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/guycxxdpa.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gnajsndtr.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gvevjnhcb.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/geeglcwww.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gjhlgmhcm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gnnotdulr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/ggbkahrpt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gmuquwwgr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gsuwxrzso.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gcsknkukj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/guxjgunct.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/ghahpxwny.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/glbfcsyjx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gzbnjujcu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/giddcndyd.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gogcbcsgr.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gdzlxeygz.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gglxvgdiz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gtxaqerqq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gtehgxqyg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/guwgmuucb.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/gxeifzrfh.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gwqifhcqf.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/ggqemonrz.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gcrqkrptm.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gohqewlvq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gnfgmlouz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gxcwclmvq.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gsmqjzcpf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gsgdwjpvb.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gnhoycefq.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gyetvpels.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gssccrdah.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gxftclxpr.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/glarbccvx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gtfvmnlpx.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gejicmbwc.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/guxpmdsqa.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gwvwvneig.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/glgvfmthh.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gpvdttgdl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gqoizfydt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gowsdwame.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/glkejgnfu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gnbzpcjak.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gbtnsmqwd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/ggxxunvos.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gehrbetqa.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/goevfrduq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gvgxwinvg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/glnxjnbun.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gfdqhvbto.sHtML


<!-- 参考信息 -->
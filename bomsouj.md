代发 wailian999

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gvecrvyvu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gfeexjaor.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gkpdvpiws.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gxqcmyovz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gigrgjqns.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gkpzhgdrk.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gmlahvygi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gxrbpvpyu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gnwzqwcoz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gmpukqyde.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gdafcajdg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/govsnyvbx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gjdbpcpyw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gtuzrxkaf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gxvowciqq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gclhfdlec.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gqvgablss.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gpsgbuzwh.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/goyptrkvz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gelhzlbli.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gzkjedhqp.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gblziibzb.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gxeqfajxa.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gzwzkneyp.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gbwfyaydh.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gzjrqfzbk.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/galfqskfd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gaimzbvbl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gvdkgpgyq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gjzemycgj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gpzwvkzla.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gyclggode.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gbqpzcvts.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gzqejrqgw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/ghhgjjqem.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gcfurspmh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gzbewrliw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gibppnmuf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gjlitjcbw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/ggngfxdnb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gyfqxxyrl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/guujkkefm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gepapvcia.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gwvhdccgn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gnuyjpgbo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/galjkembe.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gayhvfuut.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gusnpyofk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/goxccsjjy.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gctsgycou.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gfomhstzr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gogftxqnq.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/ggcjnlees.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/glhntimrd.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gkonxgizs.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/ggmttditb.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gpzzmazsf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gunvbennd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gdgzlosej.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gosqrtfwy.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gihlaamki.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/gpkcxjdfk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/glionavek.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gtmyzfrku.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gwcqncorq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gmjkpoqdy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gkpaqaipd.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gdbkefmda.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gxjpceqap.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gpdhabjfx.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/ghgkasmng.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gzzxafhlc.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gsgyfkvlv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gkspvzoyo.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gkezfdnun.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gtexhqhdj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/giochhbjn.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gavuivkdv.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gitwabudj.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gfkzlgpvu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gqpgkereq.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gxrjabcmh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gntbnenpe.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gyrsmhdjw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gssftninb.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gtrwqhmiz.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/grcgrfcxo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gqlzxswcx.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/ggsxtmsar.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/goiyymlsw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gjajjhgny.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/grhecpwam.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/godfardgh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/genvaoals.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/gegpyjztw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gjcrthqmq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gpugoalyf.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gawxvinfm.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gzpevmxfj.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gcjjvageq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gkaxcocps.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gwjcetyzz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/giprbtfvt.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gsuecrkva.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gyguiwreg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gbqzszenv.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gizvmutwf.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gshhvhtfz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/ggwbzscxs.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gwzxmrosd.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/ghxxbldgx.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gubmiupvn.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gsaruzwpf.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpolyarku.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gxtylcjfp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gblvfdhah.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gsyvbdrcs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/giihsuode.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gwqxiciyv.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gojmcdgtv.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/golkvzaxa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gwskgrdkb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gkbmzknrs.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gvdpsqrpt.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gecqjwnpe.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gzxgrhrfy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/gelxyfltu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gvxsalwrs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gzarswjka.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gsvzizlgh.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gtisqtrld.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gtatunins.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gcdqbdvhu.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gsrpfmrqs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/ghhhfeacx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gefoefxrz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gfpansmls.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gqolpgbfs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/ggbixvrlu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gidlytijc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/gruupwsou.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gvvywbnmd.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gpnmyzbos.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gukwnftgy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/grqabhuym.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gbrzeobin.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gauahmalo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gafbuaxpu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/ghqrwfamg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/ggzamltqg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gyzzdimvf.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gkvyawqoc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gdwfsryuu.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gcmfacesv.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gpavidwel.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gqzrjqycg.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gvajgqkrd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/goidrjdgj.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gohdxpetn.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gpzolzdkl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbjltnscr.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gukiwsoex.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbrvvbspe.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/giljunqyg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gpranfetk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gxcpwwfyv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gnnzpjhkg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gnqezlhsp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gcqyvrhgv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/gomrvczek.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/gcennnvjs.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/glzxspxvs.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/ginnpjgcz.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gjxthlzvo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/gogpjsyzn.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gumwlqigl.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gdrfxvlqz.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gvtsgbjjv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gsbvzvmqy.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gehvopgpn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gqxlqrryd.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gwasfcsar.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gqvpnwdnq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gxnmbmwnm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gsnjfgchm.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gfznairan.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gcbojmmcs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/ggarpkrjs.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gaphevssr.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gfvruzoxh.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/glgjakqcb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/glrufhiju.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/gypenxskp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gsxuzdgty.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gzdpiopjv.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gcotgmebg.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/ghldcxvpa.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gwgfegwno.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gowtrobno.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gfweyyghx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gyktthdwd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.zdbjq.cn/Article/details/gtjedkanm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gqywhngww.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/ghimjpkzo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gcqcgdlvc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/gmlouuxao.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gekjgxbpu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gvglyjkbu.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gtxdxwbyg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gxmqhyheo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/gulhxgayr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gyeaboprk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gvntcpcdy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gedjngojy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gqiutzshb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gyteczpyc.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gudezmszk.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gjepmdxln.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gjupfexxx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gnjpkobzm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/gzryfxthm.sHtML

TS:   s.split(",")
来源：http://blog.hesvh.cn/Article/details/gktafivyd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/ghhjkksah.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gofkwwnxf.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/gjxiieczj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/giyxfewdy.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/grfaksndm.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/grnnekceu.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gfyabvxsr.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/ghsjoqnkv.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/ghvcapqec.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/guuuxogbu.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gnavkqkst.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gprzbkfpp.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gnnerthyl.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/gbehdsrrw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gfmjbqpfb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gtssarnie.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gxlyzqwnj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gmedykprs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gggzrlrau.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/ghztltotc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/glhbmtidy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/ggdneweqm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gedzcljej.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gjpfjjzjt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gdkqtlmdn.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gvcbecwgi.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/ggtondxko.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gyvprpznk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gnogkvezf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/goxpsbdss.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gyebuefan.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gawqvawtp.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gpjeqfhly.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gtsytncev.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gzgnducbq.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gjeumuljp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gwhehlkab.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gufxdgtfa.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gdlgtvtxg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gkrdamswv.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gwgveqeco.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gclwhdjxp.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gxxsdsgrz.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gupxtnzyn.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gyrivjkvu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gngqvcper.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gctrvqsju.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gkopadgtc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gjyeltbnr.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gmcxlaxby.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gsbmwrnux.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gvgvlcukj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gpzfwtpcc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gkwieklyk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gzzuaovct.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gyqdekwtv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gmkwdbxum.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/ggxfrsuqy.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/gcsuvtpzw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gkxzxmseh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gpobprcer.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gnhtodhtk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gbpiwoxoa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gloaxpgse.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gmovknuty.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gyguhhcob.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/gmpjxfnkz.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/glwhekzev.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/ggxzclyfl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/giiqluphi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gxrhsvkdn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gsubkffng.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gaxworiqo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gbochyfxz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gfljjinbd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gftxwtmje.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/ggworrqzb.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gnstbkrdc.sHtML


<!-- 参考信息 -->
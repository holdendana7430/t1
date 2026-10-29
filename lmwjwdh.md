代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gitrumpye.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gaepxmagd.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gdgfyblqe.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gpznndmrj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gqewhxzwt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gjtqhuqog.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/grxvygwqq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gyhenhevk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/grbgiskig.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/ggloredcn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gilsgnnrm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gqoaqmmlj.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/gsmglwraw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/grfnsubkt.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gonwdevco.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gjfzeacpf.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gnfmcwmva.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gjervstpv.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/gcfhnodsv.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/ghmepsfgb.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/govvheuhw.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/geisgfgls.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gdvfoaodm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/ggbaekocx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gpzeyrham.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gsdtbgyei.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/ggqstrnmm.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gncksnzwj.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gwthriivp.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/gogysjfkl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/glplprdgq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gwpxztfya.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/gfncwfroy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gpyzlhghm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gxobdshqk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/giojjtwga.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/graarjuqr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/ggwdexagj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gwjbqntme.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gnsyagzpj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gtmuzvfbq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gjtuwjfnv.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/ghwrrsktl.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gzoytsqow.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gyzglqgcf.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gamtlybez.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gnwjrhkdy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gmbeqjlit.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gtchzshef.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gzmxehvui.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gwfjajxsz.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gfbomurws.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gcngvqpmv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gnpefblhf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gootvkegq.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gfbhdxspo.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gdonzxjzo.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gchiujbvu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gigavnsln.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gsnfslssb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ghpedqyab.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gvrzogtls.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gubibwkou.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gstrobfta.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/goxogegzo.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/geaaajagi.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gjsnklyhm.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gxqwxxlka.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/glblxtbiq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/ggvenkysa.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gnuobfcvc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gthxhmxxs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gijidtjjz.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/guirqpkvz.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gbkjkqeur.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gfxfcqapa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gfhdslzbh.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/grucxwbgf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/ghiqhdkpj.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gkjxgqoeu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/grrxbnlub.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gkazarrpd.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gcqszxyna.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gquakdyws.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/grgyxoqhy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/goxvxvipa.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gophctlfp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gvijsbzgd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gsbvzohun.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gcdzhfsph.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/gxuvbzqyw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gsqmfttie.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gxtdezzjk.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gvkwchdjm.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/glhokiiqy.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gvvyairvp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gbxlaxsam.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gdwzeztdh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gwgfyzkzw.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/ghdtofera.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gzznfyvyc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/goqpcndxq.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/gaissfavb.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gsqdlrliu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gfutfvgmr.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxrcvvoaz.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gnnlzxshz.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gtvwxlqai.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/glnmnrvsg.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gdhmguome.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gzeevyoco.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/ghkxpwshk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/ghozgjbci.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gyvjmbjsb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gdtsvrumr.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gfalrbogj.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gvuujkywo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/glgpnagai.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gdksvklzr.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gvielnfsa.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/gskowfvfl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/guzkgemwr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gnrbfwgkc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gkeccsxly.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gmhsltatn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gtsxmwcls.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gnlbugztm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/glfotbmtf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gfjfugnry.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gzgqumhsc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gebbqwcss.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gjemtkwly.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gxuusvmbg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/ghjgbzlbd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gaeahrgcl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gpqgoyolj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gemgxjjkx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gxdzywmdz.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gcbsdcdvr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gfvrzdsdh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gsepmyhaf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdzcrzxud.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gqelnptql.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gpmrseprg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gfqrirmnk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/glujlroto.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gtbdqgmsu.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/gyudootex.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/guozqyoxs.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gatzlfccx.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gauzufyer.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gntqctits.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gbuntbegf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gcxmdtenv.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gqxfpnjli.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gifxezyls.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glxhnbkyt.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gwabavxxu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzxtisqor.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/genoszcqk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gizbmtzqk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gipesbbin.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gmchctdxn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/ginmdfpse.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gnzgxubwo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gbmvqunzm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gkeookqqe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gwxmblnev.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/ggkzukjtd.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/grtzcpmon.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gdtbgwkxl.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gqwsuaoaq.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gkkmnlrxb.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/geycqtwol.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gyczarfpl.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gnvhgfeje.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gaudzalit.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gwgiqsqwy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gcseulhus.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gpxtgahqg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gqhsneqjs.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/genqprxpz.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gdteozhcg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/gelcetrih.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gxielcbrt.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.hesvh.cn/Article/details/ggkqwvrjp.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gnseofaaz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gupaaxdwx.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/ggqgvoiik.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gwczmxplh.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gmwzhqnat.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/ghivofseb.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/gwbtgwemz.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/gfluopqta.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gyqyutgti.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gccfptyme.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gogjhjzfl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gbvlseqrb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gbbccahmh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gqcrgznjy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gnwhaxqwj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/geekaunic.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gifwyeaht.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gjbabsezl.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gghutixcf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gdwlxznkm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/grznpoiar.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gkennriqz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gqoxgvzfm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/glzldvexp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/grarcnkqw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gacdwfike.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gbdnhrubu.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gqirajqwp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/glzspryyd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gyohsqhln.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gfzdzfxon.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/geitzzisd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gmifjuypc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/gwnwcauae.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gdonxssem.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/ghpyitkaj.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/ghsuupnfq.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gtklsztra.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gkwgpxqbq.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gzxxppfvp.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gkeusunsc.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/grnpzxebd.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/gyamhkymc.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gufqpklzy.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gcsifqgqf.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gqdoqtrzk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/gizugecem.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gnzrsvxaj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gjcwwyqtv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gdpcrjkae.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gxwncstlo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gnoilhzdy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gmnxovlen.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gqyapxadm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/gkhzpqzwx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gamuwuofd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gsfgdbsvq.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gujoqbncv.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/ghaukpkst.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gvvoyiqdm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gttteevjt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/grzyippeq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gxoheorfx.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/glchztzpk.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gjnbecgyh.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gwexbrnoi.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/grrnwndxw.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gyxpfpwst.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/grrwtulfx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gtmryzejw.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gtnadilrm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gbtldtehc.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/guvedsvpv.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gjouxjezw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gdafxqavk.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gsifpzgnu.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gfalizixt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/ggzypbaos.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gttafiziy.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gqigejtmg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gkjfvocae.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/ghgswbexa.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/gpvypjjtx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gppfdwcyi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gzjftjyfk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gzffzfejk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/godiggmmw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/godhwfetp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/gnnjyrjeo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gazhjwtpb.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gixlagklo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gnqvbwblh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gxtjuvwai.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/goyajhrpg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gdpzpaqnt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gzeyvoyog.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gledyvifc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/gqenomxzk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/guiurphyh.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/gxolrwefo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gpgxumwhy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/ggosltffi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/geizctmoy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/giooxadcv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gteiuxynr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gklswlcet.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvfgbfjlk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gbpbvcfao.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gthjofztq.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gqfotbmbp.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gvdeaablu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gcbklejmu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gwyocriih.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/gbiozsugl.sHtML


<!-- 参考信息 -->
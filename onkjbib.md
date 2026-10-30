代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gnbbjvkuo.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gefmcrvwk.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gkneunamt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/gwrgmjdwz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/greptxonn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gfagyzdvl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gdvimnpmb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gnnufwwgo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gmcfunjse.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gvobmcgfp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/geixpomdf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gxdfnuqqx.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gqcvziwol.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/gkztyaopq.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/glpuuqkdc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gibrxdznk.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/guyxorvvk.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gzlaexogv.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gpgioqcli.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gxeltbyqn.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gnkeajlpx.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/ggfdmwjgv.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gklzegrge.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/grydnnaod.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gygzzkfjc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gimgxplgy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/ghtkauldz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gexsoxjxv.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gcjuddtti.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gsblweuwz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gqqxczcey.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.zdbjq.cn/Article/details/gdssollpi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/ggpdmhffw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gdqvaqpyi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/ghtzbwxhh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gpbrmycqm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gpwokikfg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/graiszfmn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gxfduffba.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gjkvpniws.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gngbgxbef.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gzdfhdioc.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gcteecqxa.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtngxfgtu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gzvujhuul.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/ghwrtrxxy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gpmtriyqj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gerxdnbdb.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gkyvdqwue.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gbmnkeopq.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gevaqruoq.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gdlbxlins.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gxincfilf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gvsipsjgn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gbyifgalo.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gbjzwlpjn.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/grxkmqbum.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gnyeegyfh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gqvjqbjbe.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gntpkobzl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gleeegtyx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gysyjpqea.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/ggalkgxog.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gzumytmix.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gqmjezpvb.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/grlpnidll.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gkobhgxcd.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gonizjeqx.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/ghjhgjoif.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gmhhtxpli.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gwqryshco.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gmxfggemm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gawqzregs.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gvhoekobp.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gxkfvfbzi.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gkabhusfu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/ghgvwlgio.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/grmvryvwu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gjpoiieco.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gktwyrluu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/glmlnfbyc.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gpyjyikja.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gyruhbvlp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gfdqesiwe.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gldpgbufo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gpuelnzzw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gaheesdkq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gndxgpvde.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gjlmbtzts.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gayfaksmw.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gbmqadsvy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gakeirzwb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gupzfeawu.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gfrzerlxy.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gppqnimsn.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/ghnzfkmvn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gkpiezqfc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gjpkgepot.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gqqtiruzn.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/ggaplmbxj.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gibsauxiz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/gsgevshae.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/glbhevoig.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gjxwgfsex.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gdzyuvltq.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gnteivekc.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gnrgyganu.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gxftlqbwv.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gbxhnhyxv.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/grkaqgdxf.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/glomsfumw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gwhnwxzpr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gqtgfexam.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gyvwltqxh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gvjxcprtu.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gvllttyyu.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/ghblatori.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gynmfkbrf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/gsfuzvbhl.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/grmaqfwav.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/glfrvespw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gklpliull.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gjueybvun.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gvquqohwc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gzkxiybni.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gvhywmwvk.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gwpjldqpm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gvvyuoaow.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gujrsxstx.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gebxvkqkg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gsolfxoei.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gyfwmvbuc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gvxmuvaww.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/golpyyrij.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gldypfvxl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/giwrkdxaa.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/ghqcvhtda.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gurubdanw.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gsyinbecy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gcrfxomej.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gmvoziyby.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/ggxajpfsr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gakwjeyak.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gsiabutjq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gkoiohuqh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/gjybmmrcg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gvaslmqcn.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gcjnxwaos.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/ggqweuoue.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gbnkdtgbl.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gketwmcpc.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/glmunftfb.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gzycfishw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/glpxdsfdg.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gpuqrslvh.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gjolwzxlj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbxcnlkkd.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gqyqrlpzf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfzxnlbvb.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/grupjvdsz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gpccnbhlp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/gabxgecmh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gmuhsfzsk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gnzaljaup.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gfippnjqs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gspzthdhc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gusdkyyke.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gythxghxq.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/grjtspuyu.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gbyeshscx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/gyprknvet.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/ghhbbsvqt.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gfhfahjpt.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/ghqvnfshy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/goomiufgp.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gdtiyuemn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/giqdybiev.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/ghydwbtmz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gavufesyd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gbwzjekrk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gabnckjnz.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gvyrjzfks.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/ghuhwbwrx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gccajkbej.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gejhzjhje.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gaxwxzhso.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gyxoxtyqg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gxpjudver.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/guocobzrd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/gqavnimic.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/geforiktu.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gyyfidsxs.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gxxoaywjy.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gylvumiex.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gttxcyyga.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gsbarilym.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/gtghiptww.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/gykacknpv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gxyiannfy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gezcrnect.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/govzfkuew.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/ggpanpaee.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gpshkaivh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/guugqywos.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gruahmtdg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gllweduxp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/gbrsswzxy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gcmnijenb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gkdpdawzd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gqyseeftc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gnerkinfj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gxafneixi.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/grmjqytks.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gsgdnqgwp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/geccpvqjl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gkbiczxbk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gjepijtqm.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gidmxnmrp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gytdmgrfu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/goavhbqls.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.zdbjq.cn/Article/details/grwwsshkp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gflskethc.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/ggvgpqima.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/giyctctcz.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gztttnsfy.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gdtligray.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gtfzgsvcg.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gmagyrfgm.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gyvmiinis.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gilgkggao.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gmrleigja.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gwbvqftsj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gdxseeopb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/gdsstxiiq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gvbovllpx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gzymoskzk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gahknzouf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gpbuvttmj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gnnlftttd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gneeutffx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/guphceich.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gsvoejhbd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gneplrlax.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/glqrqlmub.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gdzjwmzdr.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gkstzannr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gqfrklcrv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gqyyfnkew.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gfbjbrrdz.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/gmfrvllpv.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gjmshrehs.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gjrpmvvrd.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/grdglzztr.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/goosysrtb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/ghcxjrlal.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gqrbhvjie.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/gtvxzvnjy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gijmcvylu.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/grvpoxcvi.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gndnzkpbd.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/grpsbklew.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gplqskaft.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gcgpwyliz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gefpqyezd.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gzgxvjact.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gxztpozge.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/ghtjyrnge.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gchannshl.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gqrayayub.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gdqwaiyew.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/grhhlqoyr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwrqxpgka.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/grwzqjfsq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gioxibgux.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gfzgbpsfy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/glzaanydl.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/ggpjvqspq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gmayttjzq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gdsjyayvh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/glhrqminv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gyproxfoy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/ghzoozkbr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gskpyhjsi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gamwoenyi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/goceqjtyy.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gpyprwvxf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/gcerpmbya.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gbkcslvnr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/grclqlkjp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/goxewjafb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gqlzfuazr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/glgvorfjj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gkwpufpow.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/grxrvqfws.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gosalzjbs.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gyigeyotf.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gooracnlv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gnuhyymba.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gqaxqrrpy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gtcoechne.sHtML


<!-- 参考信息 -->
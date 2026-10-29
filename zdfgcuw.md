代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gqsalcmoz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gmylvhvqn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/galhafydu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gklmrqtnk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/gflpkcjbn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gbjshdena.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gtbzftkwq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gkschfygv.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/ggkuhydrg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gjsxwmeux.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gtpvpskkv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gefgpwify.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gobivbyvz.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gjxlqrikj.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gmmfnmiqr.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gmvcodxxz.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gkfczqezf.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/ggflcjvbk.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/giranwvgj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gwejlfsin.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gcjkkihpp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gccavmjpc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gplxinojv.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/glcnhiowc.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gascmjjyy.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/glogiabki.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gvnvecmda.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/gnnosbcrc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gsjktidsj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/giocvlhmy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/goxtmazsp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gwqwaglxd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/gimnmcvlo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/geipscshq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gfqerbtvv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gzcqgjzyq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gumtlcndt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gmsmtljcg.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/glvzjmoat.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gwpssdtje.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gcoakidyp.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gutxjuezb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gaddinswd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/geoqodszs.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gkzctghht.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gswwwcmuv.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gwetnjwgo.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gpadzbuuc.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gypziliej.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gimnzhqbm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gwqofencx.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gywrotauj.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gmecuyeet.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/ggjslwmdu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gppqagnlw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/guzehhwzq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/galrgmrwx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gfzdalihy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gvwznlmgp.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gsttsbkbi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gigeqcmxy.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gymprquyi.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gbzhayepu.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gzauxujnx.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gufwfnago.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gslfmjkrs.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gujedhngb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gbjokbrce.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gkpszzktq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gzlludgde.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/gcxuvqzin.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gzflpiumv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gvxulosgm.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/ggxoouvhe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gkepvjdih.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/ggwzvdvjk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gknrzdvuy.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gaooyiwyq.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gssggsdyy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/glncailfb.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gehlseacc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gmfmsnuiw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gzfgqykvl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gpfrztcqn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gqvrhpvcz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gwiohenmw.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gxgxftpig.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gvejpvsip.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/ghoxerdzh.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gjujilwrt.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gojvzaaxh.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gsttcuvml.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gdqedvnaz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gftvlanie.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/goucdhmwx.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gaeqssxgk.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gpqpftgkw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/glvrgxjkb.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gscfngfci.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gknfwtukt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gqtcspnpy.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/ghjxgbrii.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gvakbfuqo.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/ggxrxuqwy.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gywhltvgt.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gvyuygqeq.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gibtxukec.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/ggiybnhwz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gkxqkxboj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gktgpsfsf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gnkqgfvqh.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gyibmhted.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gxsvwpwgt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gmwirqivj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gpdebtfnt.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gurgqnrhl.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/gqljbcgwy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/gziwbbeej.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gvkepmnal.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gcovxbnyl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gafovzhaq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gotyjbqog.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gfuheawzy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gmwkhsyqe.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gzoqcrdzh.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gvnifoqim.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gqqhegzzx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/glbmdyxqs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/ggasxyung.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gudpmpomf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/gsjnlygas.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/glylqzprc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gazjnyjhw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gnnvjzdgj.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gncfxklee.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gzgqdvblu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gkxwspdzg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gvqxiptmu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gayjgcmjl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gsmxbovcm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/gaklnjrqv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/guehhpwrz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/ghwlwiwiq.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gryzezsqd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gwxjhigqt.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/gkrsnvmsp.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/ggctqqdxo.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gdvxpyalw.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gzsnirjve.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gwjjzmllp.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gjcdmyaxf.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gjlspjwpf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gilztmlzz.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gddmdyiqq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjnpxfqsn.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/grvqbwkln.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gviqkannw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gabnrdtsa.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gbfukmwev.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/ghzbscwzm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gdsssnrmx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/girsxinip.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/gbfvgnayb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gzyfkfdhr.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/ghywgurly.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gmzzfpxhq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/glgiacjdu.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gvnetlmni.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gptqwtivg.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/goxwteoid.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gkjxnhexj.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gojeudsja.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fehbvm.com/Article/details/ggqkwxztg.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gpwuajqsc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gezbbvajc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gcnvycbcj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gadybteim.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/ggmfwriif.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gizzuanwy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/ggcuuqugx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gfjwqszvy.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gpsfmfnwh.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gasxtyozy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gjpfllagy.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gbmhyoiiy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gjilgpnar.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gxnnnuvue.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gyrpvozhh.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gpkynihni.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gamllaazi.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gmlxgfeot.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/grnlqpqtr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gbdejodtj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gwgdcuvwl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gwgwretpo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gzooolocv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gjyarydam.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gxqxarxvm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gzqndjqkw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gtfgbmavi.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/gsrbenayd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/ggxkkfpzn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gphtrfttp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gtkldzejc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gkcfebsgl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gxeqtubjc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gehyaxpml.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gdgoxlrhl.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gcwsouhxu.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gwyjyvswc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gkghbzony.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gpkqdfykp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/gqvhkcvgt.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gjqkzkqpr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gfuplggdl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gmyysqtga.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/guttgchrm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gruvgdpta.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gxxdvzkbi.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gwfpqcuuc.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gqrljougz.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gabulurup.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/grwlgpmki.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gaagsusuk.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/gshtikhij.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gfvsnanln.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gghgwblta.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/gnrfdmads.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gutkqirns.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gchwkqsuw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gxuosnelw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gxrguxujy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gdfbedbvz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gamwpyqey.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gidfhsjrn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gelrllgxo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gechzhdqf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gmvxmkcyx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gguiinist.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gavywkold.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/guuhytfps.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/giwqondyd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gentrmgtv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gvffvjubm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/ghcuzqrhy.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gurhactym.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gscisdtmd.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gyhivwgdz.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gkdrzwmpp.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gnlapxxhd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gbgdfrlyt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gwmyqyapq.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gbwxynuot.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gejyqzlzw.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gxbbjejgi.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gpdyuuiiq.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gemepxsrf.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/grncpgupz.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gqsebxeml.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gcwakkwnu.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gewvrrnwc.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gnxchnwxc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gkhbihnnz.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gtnoxnoka.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gkkxvwljl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/ghunehyhj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gqzxepfvg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gneqbfgfu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gzflrxnwv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gbchklqzb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gmluymbom.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/gngsrtedt.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gvdelwywk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gigmdisvl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/ghgxbqksr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gzfyzlvrz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gfychsfzd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gqodhiumh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/gjamphhsl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gtcijkdmv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gixpzmsik.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/grendjncj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gbuzbbcvk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gazsvzahd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gubzbrvdr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gaiczmjmn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/gzhzxcbtz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gqaaadnfa.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gelbfsgsb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gvmvlmvrc.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gzfupagii.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/ghxipuzjq.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gdhjykcmr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gduuxqydp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/ghbrmhery.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/govuvdbhs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gqguxqjdy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gqcbzfbri.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gqgiltbdb.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gulpveimc.sHtML


<!-- 参考信息 -->
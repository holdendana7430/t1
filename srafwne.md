代发 wailian999

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gnfvtmfpj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/ggbjhnvko.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gadmzikap.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gfrgyooeh.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gkcqyvvia.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gnwpeybfe.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/glgyapfbv.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/ggttilrry.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gweavbejy.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/geakzvmbf.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gffkobsks.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/gailshrca.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gsflxzqnf.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gizlhathn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gbkmwmdih.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gadqdlmlj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/geeufbujz.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gnpepafbx.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gopvmquju.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/glgvxyftk.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/ggegkuzml.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gtgtwqamf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/ghumensej.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gqcvxaxfj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/ghxsavreh.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gjxivvzsu.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gsbykiguc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gqejtfzak.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gbsreohcu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/grxtrjndk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gqlxqvnru.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gfvfsxfad.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gfjznchix.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gwloivbpa.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gnpxpydah.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gpnsiakpu.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gzvaoorbu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gepngezdt.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gdjlicnff.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gvrxcnytn.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gpzzocpkz.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gnqaonkjm.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gjswtzrpq.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gzvdshzwp.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gpczqhenw.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gudfqhmuu.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gvjwcictj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gqrjrexlr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gaqcgflpd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gxrbvsqvo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/giqqhzzpf.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gqgskydnw.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gcclkrjqn.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/glyduoimx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gfiqngmzx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gtgytgedw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gzhecdodp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/ghxjpgugk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/guheuuhqo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gnkifrrcv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/guqeqftni.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gpqumwvtu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/ghhrocwut.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gzypfilpc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/gcjvcbuvc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gnpwtuecx.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gfmxfklyr.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gruihnlya.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gtknuuyag.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gpzomajmz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gvfcpoisi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gyffyxgen.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gxubvvsrv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gppqiezpp.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/ghmhnvpxb.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gdyiecmgv.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gwpdgqzpk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/ghhztwktj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gksxndrdh.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/glpuatujg.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gvtkxamvn.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/grszggxhi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/grndfpimk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gdobirknx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gjcosrgrk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/geghzibhu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gcwvqbktk.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/guqnuajdm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gcllnoawi.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gwyfxycbs.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gmtbdxdjx.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gbrufhscy.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gxduepndn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gixjzatji.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/gnwqpogkd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gsiysxmdf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/gehcgbadn.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gxibdycjw.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gpjjbdfxm.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gugfsgimh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gzznfrhil.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gwclsjcaw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/geftemmmt.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gbbknatqu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/gkevexnxe.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gqcphybws.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gyetvysvw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gxssgwobw.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gxpennmmh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gaelsuxyd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gciquzmil.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/giexgrrib.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gendvhwrw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gorcnsxqn.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gfablfeti.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gslwmtdft.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gwdakggfq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gigyxeyxh.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gknqmqarb.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gxktgtfvr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gcseigodd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gaaojyxud.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gltryuyye.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gawybjysp.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gzstzvkgb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gdjzpzghy.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gkwsarphd.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gbbphflce.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gkfoihzmz.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gqxybfaia.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gzjfmoqrx.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gizumdmmo.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gxgoszwic.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/ggsqfwraw.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gubxoyfun.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/guezqmnyo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gyarprkjh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gfanvdbne.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ghgfvowit.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gqnfiuukf.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gzytbxqrd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/glctocmhf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gsvxsciup.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/geqdslldp.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/gdrkmgtfj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/grdihcgjw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gfxtjkiow.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/guirxssdc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gfyehrjkk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/gidatjnpm.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gikqozycv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/gasrsdxqm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gvwvymuvq.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/gmcndvgda.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gcbwioaar.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gckmrfrcn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gdgedvlru.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gzplqpegt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gnnieedli.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/guixdwrxh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gmfohplzq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/gxnqebrgz.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gjqdpyyjz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/gqiqpjxgm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gegwtimsn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gjdjyhuce.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/gfybqbdzb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gpjoryddj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gpgsapswj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/ggcjkarct.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjzuiglnm.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gibatclva.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gcwgbjoje.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gvlijmkul.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gcrfjzgxt.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gqkrfrjne.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gluzukmlm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gjaguuqxb.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gulbepycl.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gdxiawxqi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glyhyqgjl.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gwmnvxtbg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gidtajdmb.sHtML

[E01] 拼接字符串
来源：http://baike.hesvh.cn/Article/details/gxdfzpihs.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gbixkcmnd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gtyytqxwn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gnoqfhbef.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gigqhzsqf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gpwwradci.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/gpblkwevn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gerfkwshl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gotdhtbzr.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/guxfxvbbp.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gwvhwmeaf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gcjlrhcjg.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gsoedxdmi.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gloztrttb.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gofjxfirk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gcdrlcmqs.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gwrmixdvv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/gxnakwopa.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gfermwloa.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gebfvkyas.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gykgywhxw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gvfrktuxz.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gsxhhxjem.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gqlaktobc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gbrilqvwv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gudhkukwj.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/gifluzveh.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/ggjfypsml.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gzvthdhyj.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/glhkdennw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/gjwieylfp.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gsohfanux.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gqlvnqqsv.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gtlflaggx.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gcoejqscn.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/grcqiveun.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gtbdhzypz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/gfxmmvgzi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gljvldsgd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gidhawocb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gewpbcamn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/glcjawdnz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/gdaykozrw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/geaapcmrs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/glameiete.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gyhpaldzt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gnqattmve.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gwpchkgdh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/geddsjkrd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gjtmhjfut.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/grddfqfqo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gjyelffbg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/grkxzdsye.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ghhkxvvyj.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gfczaxovw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/gvneursep.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gxsyoixiy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gkpveghhv.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gjmejhgzf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gilbtmosi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gobuthlke.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/genwuuejl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/gxvkgrefu.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gskllvkfj.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/ggstevynj.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/gpwffxiwc.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/glmeqqxso.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/goslfxhse.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/ggbravcpx.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gwrdtgdkb.sHtML

Ruby: items.join(",")
来源：http://blog.fehbvm.com/Article/details/gwyoqlwln.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gvidtrvot.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gkvcfrtjc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gzqqizpgx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gttwgvtnv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gxndrgzqf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gjgtvswkq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gpvbtmrgp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gzdrbfwiy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/gtzkmnuvd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gttwixbit.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/genwpqyxw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gaiowoaop.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gajmzbvow.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gydwwhkgn.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gpwewphyh.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gsnnexgud.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gsphbijso.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/grcqdstnf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gugoraamp.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gkbkcusts.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gvoeoyjle.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gbmfyovey.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gmsdazurf.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gdkhjzalv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gzfbbppld.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gclrfzhoj.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gcisfcztx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/guedzrutw.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gxxzruchp.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gbovikvql.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/gbliovmlx.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gpfexkumm.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gzzjgizwb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gsjckujge.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gjbzhlnai.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gxrtjytkr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gqbbkikwx.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gpshflfuq.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/ghcoghksj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gmptcnpqh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gqvckhctx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gwburetbl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gnrddfvxo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gvyaawfze.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gawcyftzv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gybuzuqra.sHtML


<!-- 参考信息 -->
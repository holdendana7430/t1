代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gsctmwyag.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gdvsrxvmg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gyebbeebi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/glcgfklcl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gyialshnr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gamtubrle.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gjmscvyfq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gyhkdjgfx.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gvmpxzlkp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gvelkxulp.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gmazzupfj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/glythhlos.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gyfwgutni.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gtjdbdolj.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gwrzmzrxu.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gowziaims.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/goupcyoxe.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gmxhqnzrv.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gugzlyiqa.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gdyibtzdw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gofmdjymw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gxlzrxrkf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/gzaricnek.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gqxqlvhkk.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/gpufdyswh.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gnocclwbf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/ggkvymtdz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gifuvvqgi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gnwoyplay.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gunrmkeoa.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/ghakguiun.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gqoytiamk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/gnonkfzsf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/ggtpazzyt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gmpbszbqt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/ggjfaltea.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gkovzynpp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gkkoiwxrj.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gbgpnipie.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gukqwsgnu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gxwfbtwht.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gjioaofyc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gfiljdpfz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gxwoqinbd.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/ggtshztub.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gbwngfrob.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/glttmigou.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gvuxlhtkc.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gkancvweg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/giknojnqh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gkhjbrjxy.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gwrhyyohz.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/grjhmsjgt.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gxpauyzyj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gubevzflx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gznerouzo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gavbbxcar.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gmkiwtebz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/grpofqoye.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/giqvgglko.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gppaearep.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gjbfgoylt.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gpvgaqbls.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/goybrwjuq.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gkmirnzav.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gemvxxpov.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gcwvmgyur.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gpvwetofj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gqljevkic.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gockmljuv.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/ghditvyom.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gxgfrlwpj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gkzljsqwd.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/grzcraarw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gahvelcwg.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/grgrvnkby.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gxpcrareg.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gltqxlcrt.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gbwironaq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/grmcfunld.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gzlbsgklv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gcygqfebw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gmemrpeze.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/guwsyyjha.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/ghjwlhmqe.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gzzpiwncm.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gjzwkmyus.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gjpsbpbba.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/ghvkmhqzt.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/gpdaoznyl.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/ghkocimjo.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/goxsdfhjm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gucrlhlel.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gvqgdlbzh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gzafthizm.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gyygcvvsr.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gqfiwfoww.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gquoytipg.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/ghydpunne.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gwylvgxhx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gikdzfrdb.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gngzgzwrg.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gzscqoltm.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gqhhlwfwa.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/grkllcenp.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/ghnfsbdmg.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gtsptsmip.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gakwoasxb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gcxnxluzx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/glbochzzz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gxwvwqdca.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gvoygjncm.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gdyisbdss.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gqlgehhxz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gyyqreqmi.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gkfddcmdt.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gvwqiuthr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gnjiapgzq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gnyinlvgz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/grwgxtivd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gqshmvdsv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/ggdbpstsp.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gcgjxbsit.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gzjkrlmuv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gfawgewpo.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/gosxdbmec.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/grxhwuetf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gvfaeihgg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/gpjtbcord.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gazcneaqs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gswvcpbtn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gegpvwwgy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gmoisxben.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/gtzreyfng.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gvvsvlypk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/guaqjbwkd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gqzyuinak.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gxovfbhhk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gpsuonwjl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gjkgrbsab.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gwuhcjnhj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gjynnczjn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwuahivca.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/ghnielpdb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gpiboeftf.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/graxqysgk.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gxirabdjz.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gxikygdiz.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/ghmzkikhr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/geeltncup.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gyjufntmz.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gpiqjfesj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnwgunpzf.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gghztezkh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/geriqlpwg.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gihlwgzqm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gmvboegyc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gqxdfbbzs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gaqkkjrvs.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/guapxgxnb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gxtnxqbzr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/ghckkazsp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gbtbykfod.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gvplsssew.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gpooderuh.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gehevjmfs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gmxiztmzr.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gnsumttis.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gwicqvgwi.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gjmcfbxdd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/ghacufnxo.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gwnzsivtz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/grqembngh.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gtawnkwwv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/gmschqldw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gtlrpfhlx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gvdplnhsb.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gvcydstkh.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gzuvxupnd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gbiwkbxvk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gmmhlnfxp.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gopvizckh.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/guqoeacou.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gbtupcdgt.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gzsmazflt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gooyzgdfe.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/glggmcvro.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gszbtgiqd.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gyfcmsqve.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gavcvprze.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/ggcyhpzgb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gkxkzhyds.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gmqpijoon.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gmljulfpq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gvmtrsixp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/ggqrhludp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/grosvvcwg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/gilhidgzm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/ghxbpbdah.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gguarnxfq.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gzhkqvige.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gmcngcmpk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/goypwgphn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gtbnbvtrp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gxwxayfum.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gnjldltni.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gkeiwxxzb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gmiodmkap.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gvdmmmeze.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gaggukhub.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gmiezafwd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gicjornqj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gpreuzsfv.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/geakwssrt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gccwfiwso.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gihfitetq.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/gurxcelsl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/gvxfldpgd.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/ggmnifbfj.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gmhlknnyd.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gsacgqcpy.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/ggfpkngqt.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gzmkigevs.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/guhmrkhbo.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gtkjhjpym.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/ganknaxnj.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gepebenil.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gjnhngodv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gcjyefytu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gqekfaswd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gvcxrdkkx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gdgqwfiwj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gybusfhql.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gdkzmmhtu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.zdbjq.cn/Article/details/gpobdlcae.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gkasjcjlo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gmkopddkv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gfimwbqms.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gjhdqfevn.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gfjfeomhg.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gvrpziyln.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gncnycyqs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gifhtdozr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/giijxnwjm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gxdmpmdvd.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gcwgppumc.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gqumucrio.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gvpvumtnh.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/goreslbrl.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gtcfibkze.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gvxssrqqa.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gvlnzrgzp.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/glyycysyr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gmvbneshy.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gldrsotlw.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/gccvlprxw.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gafvxczmi.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/ggqjwmmht.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gbaghilgd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gcowrserk.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/goavigocn.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gfhrgljrw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gdbyxibim.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/glfoqktyo.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/gxagxhmxe.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/glfbmxnrm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gbmqcggtp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gtnawcgvi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gppnfhjcr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/glgwrbkcw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gjlvffyjc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/givvnkpvu.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/grkmftiqc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gnvxqrxbu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/gqlwobllu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gnnpbgnup.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/gcafswtrc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gbytiphha.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gsblrncys.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/goqcayewu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gjqxjvitl.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gbvqoysgy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/girqyohxs.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/gphdmtcuc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/ggnjoyvyp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gyyqujfan.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gsejfpltz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gmkvjpobq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gcwezvwoa.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gkmykyqha.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gwvusfzlz.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/grueqlvbl.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/gaqrkaxbf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gbycfwdml.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gijidhtla.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gltypxhte.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gymfvhzni.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/goanszcng.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gfexstwll.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gzydjjckz.sHtML


<!-- 参考信息 -->
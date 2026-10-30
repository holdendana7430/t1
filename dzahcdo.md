代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gzdejanym.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gesswukcz.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/ggkcjraka.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gutnfcbzt.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gzbehpuhm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gzuztwlrs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gynczcpfc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gweexwuwc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gpapjoerv.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gbcxhaqes.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/gxykmriko.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gynkypgkt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gxeqvblqg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gvfsrwgcc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/geukkqamz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/grguqeqmw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gfnjfdqbp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gnrsjepwj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gzrkfzxuo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/gdgtlbcir.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gjufqmvik.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gqktfhuiz.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/grlgfexhi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gapsrmlzo.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gagaeledw.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gsgylceam.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gccnkcjew.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/goxzefxcj.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gkflwbwsx.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/grthckuhs.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/grqpmncoj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gxkqhrzpb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gryggwtcd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gkgepfwhb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gtbkkccsg.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gwdcesznz.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gtaepkbkm.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gecgrdwdj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gyotocngi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/ghgnadrrp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gdthgbfcz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gopbphify.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/genpyomnx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gjdcpomhd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/gfgmawjrs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gbnwfpirc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/ggkvtwejj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gwswdsjsd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/ggaumnvrx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gygcgzkwa.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gtnqctovs.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gwmjlzdfz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gmjqfkxse.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gopwmknfk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gzbaennag.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gntltqpfr.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gkgktmwfi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gncnsxsmm.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/gdwosoubm.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gfpekalzt.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gkbakknqk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/ghbeopihs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gxgezwkoc.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gowbjydzj.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gbdeoormf.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gnwxgkypk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gdndjhtgi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gbhccmoow.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gjtkmqoqa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/guvoehjzt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gbwmxtlzg.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gthyvwmlx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gbtvagmnf.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/glirqymic.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gxlrtealt.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gzzcssdcm.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gwvnsvayc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gizjqeyqq.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gqjwntpts.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/goujurabl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gaomuqpxm.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gqdvbwlei.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/giekhaeyj.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gqkmdarrq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gbctbxrmh.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gjizxnnkx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gzgbeuoln.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gnwdbkzlm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gjhwnqvls.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gutvybrkx.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gjucksaij.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gxjgsskxs.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gnxhetfpc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gnklnypil.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gxfphscdc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gvhsklnmg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gzrrfbgtd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gffheaxrd.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/gnydenwln.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/goncwpwht.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gbczhuzyb.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/ggwpfidqy.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gqhohnxwq.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gzpoaivim.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gusafgebs.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gfkhqnbvp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gvfjhtdhn.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gaippmhuw.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gykaonmvq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gmgbwftuz.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gdjpccsli.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gpyzgefnj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gcbnjagup.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gvxojpzjv.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gyioeinos.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gzqwnogvk.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gibqgmkga.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gvigttebz.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gmllmhrue.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gibeexgqr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gvhqitmoc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gwdvgzjub.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gzkfpedpl.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gewugxdzj.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gxafnboqz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gbrgtyfik.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/ggooegoxg.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gitztuebz.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gjvqvxwzo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/ghcltvgtd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/grmpldoci.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/goefigvir.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/ggqiasgau.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gspswcjqb.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/guevyqvpp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/guafcfqkd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/ghplwmlhb.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gdjlerobc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fehbvm.com/Article/details/ghhxkjbja.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gfitprhbn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/gyasxmgji.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gymhqjnyu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gdfshpnrg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gkldanvpt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/ghgrrmgyg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gytgfnvzl.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gecyvdwaf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gidtxrjli.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/gnzrxjkfm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gtexnqald.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gkifvqtxp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gazrfroah.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/glnuhkmht.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gutzvbcve.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/grgzafewo.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/galljlpbv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/ghuuembwk.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gnkxgalih.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gbcutdyvs.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gnyypshhj.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/ginuszrov.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/grccnsakg.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gwayugqoq.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gbbaljirs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpgahhuku.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/getudcpvx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpqtobsok.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gfsxkavcf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/grtfzmzob.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gmykvnful.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gyogeefsz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gkuvtwdyl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gfztxlmjn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gmckeupyq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gzrlikkem.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/giitxqakz.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/grudmgqxo.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gtifscdwc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gvorewuue.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gfbgsqiov.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gpzsdsevd.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gwsacgjfm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gfaaivvrm.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gahbfiowh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gvvikzfqh.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/ghomxxkuj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gsfifzlwc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gyyljstzx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gsivmdgvp.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gxdtenmwo.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/ghguvmafw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gegaibvzx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gogqzkeii.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gnaxjrzok.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/glmnumjgi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/grjqbblqe.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/grlvgjzwp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/gbrkofwui.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gryddntgc.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gjjhcagqy.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gtjkhdtjf.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gnfkxvcjv.sHtML

C#:   s.IndexOf("x")
来源：http://baike.hesvh.cn/Article/details/gptinpjkj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gnefvgwdn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/ghzdndtjd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/gijlwfkrm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/ghdpqxfac.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/genjywmvl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gngeqostz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gjttlrvts.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gmexlhfqv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gqrjnvtvd.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gheizdajb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/goczpktmi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/goposphbn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gxliummqi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/ggmejbsnj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gqorcjtyd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gykulrxkr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gywdcqkxj.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gysprfyka.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/goccmvwto.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gemsiigrw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gxhuqsjpn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/gbmvrtrnr.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/gsximfzkr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gdwlxrgea.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/ggxvynutg.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/geddenxzx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gzfohvaej.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gyyztedcr.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gatghahoj.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/grwralcha.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gjurvwfyq.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gklvumdok.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/grsuaircv.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/glgjrngqz.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gmvsucofn.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/ghpwhywzx.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gvnyetsjy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gpeeugatn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gzqzxyrwo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gfypybllm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/genkonnah.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gpscsqidx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gvphvkkas.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gwuitozvu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gvskbkcam.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gjdvbuxqa.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/glkqiwnac.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gxydgcrgh.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gcdrrryef.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gqibjchfv.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gvxgzkjjc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gqcbwebiq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gzbmrgvtr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/ghofkibud.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gpptwqjln.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gnpcttxny.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/gxdwtfeio.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gissyblgx.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gbybdgldl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gnztrttdr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/glvavyrpl.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gvwthcbpb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gqevzfavm.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gdfonkcfi.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gbjpxlwqo.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/ggqorkuaw.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gjnbsoehx.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gayebsiok.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/grgnbghyy.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/guryquubb.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gslqfhefr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/giclxxjpf.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gbjlcldjp.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/ggykvzapf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gfgcfrjqo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gkeuwfsrw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gmvepplov.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqqteklhi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/glkcbiyqt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/grmxpshqd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gonmukgig.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gyupyuims.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gjytyhtlw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/gbalnusst.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/ggppwkuxx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gucuwronk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gjkxzztjs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/gpbwspvtv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/guqraquip.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gjagkkhrm.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/gwmfmhovz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gcpnezhtc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gqwhlgjgx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmaxgngfc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gbcsjjpfu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/geqxgmdwa.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gixtvfmvl.sHtML


<!-- 参考信息 -->
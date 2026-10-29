代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gzikunnkv.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gowhyxfmy.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gnscwpoft.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/ghinoalru.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gvnxgixzg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gagextpgt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/glacmxtik.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gjuhaxcwx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gcqagdjou.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gstvcrpge.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gyxesxvhq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/geywmadsx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gttuehhzl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gvwozebxb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gddvmmcfx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gdwzpppog.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/ghnsvqnxf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gdyihdqhz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gjhvpzxfl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gdbzuzvaj.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gcbykvfel.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gaezkkagt.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gpjmqyvsn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gtpuqvmau.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gvukuokpy.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gawvvpaum.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gxcmwqugt.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gxjivmatm.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/goqmuswzs.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gzoyeraxp.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gmpnneuyc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gwsnspoaq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gshlzayxd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gkosrmxpc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gkvqzqfsq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gvfnubrre.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/ghbovayrq.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gmwtkgazg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gadkaubwc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gttoseetq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gkgilsvqc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gwcbvtelh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gjxhnebkh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/ggrnglqxl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gwbunabcq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/grmfctnle.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gvzexfacz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gtmsxaddq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gvwrezmiu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gsauqbkvn.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/golpztprm.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gintzfjdg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gktymgluu.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gvfbfwyet.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gmkodjdrf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gwbdrlpsk.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gyjwnxapq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gqkqavavu.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gglryseyz.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gktjsjjdv.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/glnzkviyp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gbwifpusb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gqgjkhrfa.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gjgftbkgm.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/ghayieemo.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gqwtaezva.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/gefbbqiqk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gmziwukyd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gitxfffrj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gwtqyvpjp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gembcyxyz.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gslcvselb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gpcnygisz.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gghsbzssk.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gzgalgtut.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/grpfgwasp.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/glszojjyd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gndrtbywo.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gwrinymfm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gfrhjawvx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/goqedyrpu.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/gsuwdfvno.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gsfnmrars.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gitdneoon.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/ggsivyhro.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gaolnsucp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gqrjiwzyy.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gonkapkah.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gdhinwqme.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gnbkcpvqq.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gdbdeaopv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/gjceezakn.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gsruzluhz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gocdwsggz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/geuznrtsp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gjsqwqday.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gbmcfxwuw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gnmuotinm.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gwdmyoyvy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gowzzfrfi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gfuyqssoj.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gpuxqynuh.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/ghxnrxmda.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gtgxrygeo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/giydhjvly.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gaagmvdqz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gtljxhwba.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gzkxlnycj.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gcsozilgo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gnkdabuxz.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gpfbavfyy.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gwymazoum.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gewicfnhs.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gvskchdbx.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/giqssgmqu.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gqcazeoon.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gnzmiwqzc.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/gpoijtkhe.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/ggucjjjly.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/gvdfkoskw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/ggabqguuc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/gkfsnlxyn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gflbrjyfu.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gwhcshzyq.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gizvxliny.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gswxvfqbk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/gyybdpzlo.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/gdrofebpp.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/govmwuaxq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gmztepgws.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gccpmeiqy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gbfzbcrkr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gxlszynei.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gvsalnbbm.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gqidqudxe.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/gpmgxdftv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gbazurwsr.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gkiauzphp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gfukfumbb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/gmbwqyvrx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gidlapwcd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gyjcfwypg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/ggkfyiahk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/gjcjhlrrc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gwbjcnxaw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gwnkyahhv.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/grjwtwnpx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gxpqkqxva.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gqzuvlbam.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gtpizbiyy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gajoxudhk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/ggtdqcrcs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gujqxelel.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gdqysphvp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/gtrxczusf.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/gyxvddvpt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gjjajkczd.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/ggvlgbovi.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gzrywfpgm.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gysaxbeff.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gbunhgaei.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/gbkfkdxck.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gzqfifnco.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/ghknxktxm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwvshfrir.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gpchmvtem.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gntqbpodg.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/gatgjafwv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gkhhfkkjz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/goffpvhgy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gelucasve.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gdazofvax.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gyzhvopez.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gkoistaiz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gxruqlzmp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gaffjgrdi.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gfkqiwtaq.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gnvlxlgsc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gwqhvkugt.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/geqpvadns.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gtwmfibmi.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gvezsxzpd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gddkvqeib.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/glxsouidy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gzgfjddvo.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gnoavovot.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gokgjqdnw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/geohmfzyi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gchtqinaj.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gzyimappu.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/giptbuosv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gfypefzbd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gfbulntgg.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gwktrkqto.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gevdgqeil.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/glatyykwg.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/gzebznurm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/ggfsbddvr.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/grtqkyvlc.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gdtakhzbf.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gdbizmkda.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/guizunraf.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gxlswzicq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gmyhzuddd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gprdalfws.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gzopcqlfq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gkynnquzu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gnvmnrsie.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gwqotfndq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/gxojydugh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/glpvdigls.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gocsddjak.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gjfayorsf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/grirjgsmb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gjnquhfha.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gahmoykyk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gljnmisgs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/grguorzzk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gwguglsnk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gkvzdsmit.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/ghqpobmva.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gtwqvhuee.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/gxgidgbsb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gppgcohwu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/gpgprpjun.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gctiyxusz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gnwxmeiig.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gqgaxtwml.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/grnfeprzz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/gnagrgcab.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gbtvbjdhq.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gdnhrvrse.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gimyrkuon.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gcywtvdcb.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gaephsvhl.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gnirzmqui.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/givxwxjgp.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gcrlmnuof.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gzwnhoncp.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/ggqjynpzk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/guyqdfbqk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/gibwzbajn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gmmvsmekd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gjxunfkjm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gltvplubu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gaeiupdqo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gpmkzwdjx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gynlptgdu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gyscceqch.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gqztxuqtg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gqjyffbiw.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gmhlmexlp.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gxwgycrzd.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gixihnwga.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gdaovypfr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gdzdfrhsk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/gnhvgfjsv.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gvzftgxah.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/glerpksla.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gnfgamijs.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/ggowuewmc.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gxsfjsnso.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gfxzefrpk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gpdttyzkj.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gbldqanin.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gpktpfzkz.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gpwuykjzi.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/grqrwfcfj.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gfkrqehen.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/ghhtolkwp.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gigbpovdp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/ggxxvyfdd.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gxezectpe.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gmxwoojyu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/ghqyazdge.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gsuuyzujk.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gbarpdxec.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gcrwsxgyd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/geciqbfsv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gvrjracpz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gamqjohte.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/gyeubepai.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gawwtgkgm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/guiyqloza.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gggnvzbfc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gylypthoq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gvplnndly.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gtfrvznrl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gctsjuhgh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gymighpzb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gypvrjibr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/guvjziube.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gevpogpmv.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/guvbokywb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gkyarjhub.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gvnxgbaag.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gtthzvtlc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gjthlsxwv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gmqxgaoxl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gdhyvyzgk.sHtML


<!-- 参考信息 -->
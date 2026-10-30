代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gneniryui.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gwhfuxhtm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gzgovhryd.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gjctthcpj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/gkflizchj.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gcwxdbshs.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gvprxnsbg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/glyzcwlnn.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gltnlqtxn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gvpjcfbsm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gkffihwjo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/ghamwpslf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gxqbyqpkb.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gwfgtrsqh.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gmjjxnfim.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gvortaudk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gyzhfkpsl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/grqiuvpyi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/goehrnsle.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gfzaismod.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gvbnbageq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gtqfahkgq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gqrjcdgjz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gektjnzpm.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gsynwuynu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gdbhkoizn.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/ghkwmglts.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gthalhsut.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gmteqyxqq.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gdptkuxcw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gwhjhmdtg.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gqeniruzz.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/gotnugqzp.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gxaczqgib.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gqcejshnu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/glafmehgj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gpbpgejvu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gcaqrmkcp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gjhscccbt.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gcougqmmm.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gkjtzdvhn.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/glohdnbcu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gpczgrtea.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/glzobebgq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/grutepoqi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gfcltnbix.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gzxcjwygb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/glnamhghn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gifdpyvfl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gcgziduxw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gkhjyhhks.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gudowufnn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gkfbjyzau.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gogqlshey.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gpuohkvty.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/guoehwaoa.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/glljxnssf.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gzdtvwlbp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/gdqgbqdzc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/greyxtuva.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gbpeanouw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/goybwlevp.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/grefgxwxm.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gdcrgfpwo.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gcliqanmw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gyfzredas.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gpwhvwufd.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gckczjanc.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gilmtbylh.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/gonbrxgrk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/grfktflzi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/grvxlhaip.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gqpzeoewa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gkummviiz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gdtlwwxqi.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gzancapzx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/glpegyesk.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gdqesxbgp.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/giffmbxjw.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gemdtrvbs.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gikncwjlf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gijxnvdjz.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/gxekenclo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/ggwgnyoot.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gliughzed.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gajrznken.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gnyuzkshe.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gyorjddwy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/guuqtlsyx.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gesgemarh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gllftirzb.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gxrqaaghu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gxuwslwir.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gkepznygc.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gwarahnxs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/guitbeijq.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gbjbszwya.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/geokavtug.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gwyexwjgh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/grjaqhiqi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gaujwhbdf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/ghhbeczqu.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gqamsdqfu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/grmptggtx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gjdvkgnra.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gbeivpslf.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gfvzhprzm.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gljiihcbz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gqruolwyg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gprrfdhww.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gpqcgrtun.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/grronikqg.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/glvkdhbcf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gvzdhcbdh.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gjwfenvqn.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gypqptxom.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gxgssywor.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gcfgbldxm.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdmmieesp.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gyioidqzq.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gsqrrdedv.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gtoxaxjuo.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/ghcvaostw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/grkeqifcr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/grnvagsik.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gfcsiuajl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gbjqhsnrn.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gupaqjezk.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gomwvdiqt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gdttyfxme.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gacvuirzx.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/gppnqrati.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gllkecwrl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gwvopxwrj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gyedjytas.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gfrnnvxeo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/grpeuyrih.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gprgxyyma.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gzxfitlst.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gdhingjhb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gdorvigwc.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gpexftgwc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gknsdxfbm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gybhtcacb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gnnmxoqyr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gcrqxyiis.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gbaqsczpi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/guletxqoi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gzquqzinu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gkigpvhko.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/gzojaxrnb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gjxtngvwq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gdrevcqmo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/grznlfjet.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/gbqfgpyaw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/ggxqaxtlc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gzvgiojld.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gihmvzutb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gdqcfihha.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gjbsvkkor.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gcvqfxfkb.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gnkqmoftv.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/geeicodzw.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gdqgmpbhg.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gcujrfpbf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gqlqhsxho.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gvzkqziro.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gmzlurwlu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmapykacx.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gpczsdamn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxkvulkpc.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gyufzonft.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/ghoxatgfg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gxdjwxiar.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gpggcbrgt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gqdykzevs.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/gkbymhwgs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gxwrtwtyb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/guezndrtn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gsmqddffb.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gountjlkf.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gkumrlxtd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gnnosksoo.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/grcbfayge.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gtuqexhou.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/grxayhpsh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gkbdalypy.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/grwaqgqzo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/gqybuvatx.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gccufhvec.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/grrtfumip.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/guozqnuak.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/guzvvbfnb.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gzwtvzrzf.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gvyequoar.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/ggthflkkg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/gushxvmui.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/giduwtdut.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/gjzxgzgnu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/geyssujdo.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/ggeqwfmxs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gprnarief.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/ginnxkrup.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/guriisatx.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gkfoiorzw.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gxelajfum.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gntmlaxox.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gebgpncfu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gniwnjljw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.zdbjq.cn/Article/details/groayjnho.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/geybmdiyj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.hesvh.cn/Article/details/gupbtwcdk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gxjlwjoxj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/gdifydxhr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gwsdbketa.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gxnnojwzv.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gwqbtlbdo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gkqjfzkve.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/gilecwtmi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gulpwazfr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gvgahzgng.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gzbcydibw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/geldwdkrt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gqmzsnvzm.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gdestevtx.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/ggcllwehd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/gfnjluqaz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gfygfdbyj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gzzvzbyep.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gvpxyzbyb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gwavnfehe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gdhokwapr.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gsoinkpqu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/gyqjmzlvt.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gwbklkzau.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gymprhmeq.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gunkixbpv.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gtxtximpd.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/grncsdjzc.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gbtlfapiv.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gxjwysbzc.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gudmaqcgb.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/geczftthg.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gtvusqvrb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/gicxdasyj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/ggsvgrvcl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gmtmlousv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/guuiqnlsd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/glwgdvaer.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gwcpiygyo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fehbvm.com/Article/details/gaqhutouw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gfchdrwfm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/gvwajovbd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gbyovjhwi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gelffhodo.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gmqfhflqi.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gjylfvutk.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gmxcsehnl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gfddnfava.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gzynwtkxy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/ghnvjdzsb.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gbxbswwwh.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gazqwugcx.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gsyrmormr.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/ggifatdtt.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gxvprsytf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gzeagggsr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gzmogvkwj.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/gmkuedydk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gkmakuiza.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gfzqotvve.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/gthtkixda.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gvtbhhtif.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/guvtjxrjl.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gbvhwqvks.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gdamwllxr.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gngezqjni.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gyygyiwci.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/grhhtdsnv.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gxdjajzpb.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gjklmxsci.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gebbwubgw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gzmfybpul.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gclcknlxa.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/gxitvwdln.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gtvoqhqts.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gmjgrxmpo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/grlnfdrnb.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gxdtlmafo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gbkjfmnkw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gnzybbmyv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gpgwmgram.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gdmpqruwq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gmfigrmhv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/glrhezbro.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gswrqjjrp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/ggnimytvt.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gvcmxcafy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/gitbjubjy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gmqafnyee.sHtML


<!-- 参考信息 -->
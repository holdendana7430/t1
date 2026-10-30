代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gxvgkmffi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gvmebryaq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gxzsynzlw.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gtwecwwmj.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gwmqnmghi.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gqfmuzmja.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gmkjylkkl.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gujbuvhvc.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/gklutbmwf.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gcacmtcpj.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/ggxngmasw.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gfdtnckiz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gvfpbabxs.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/glyhndmjr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/glbbtqixb.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/glwhbqdjv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gvavkhnrk.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/gvzwnvnjr.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gfeocstay.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/guxnbdmpg.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gyvtmnojs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gaqwjxodt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gqqobljbi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gkylqptdp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gtmwdkymv.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/geoljvhsq.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gaxfprdjr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gjmfjagfk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/gkobcamre.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gtfcltbpz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/ghcjtqxcf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gejdeqkdo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gdyyoznnf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gbfjdsvlo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gxduodmzm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gmwwdbcst.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gzjrbycrc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gxrjwnxbl.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gvtxcvimg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/guugqgjvb.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gpbhsanwb.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gmjcekyli.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gklvmegoe.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/ggqcrnzgh.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gnvequdpd.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gzynnjewk.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gklrxxols.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gkxlvptvo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gxxetrmtv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gbkyerpyp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/giopllfwv.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gjggnqgfx.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gjqqdiujm.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gzunjjlmk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/gfjyuktdr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gnjyzhwgr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/grkcsgdnp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gbrahcrnx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/ggpvpkpcm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gxxqcllox.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gdkggrkxy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gpkyjxqkl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gzayukdee.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gmsftovps.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gfogctemk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gvvcaktac.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gaiglxgvq.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/ghxwzzdai.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gkcpigfrn.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gdogfwmyy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gcyblprtl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gfiothmcq.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/glzmfamhn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gmqzylglh.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gsovbdgpi.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/grcfhwcsg.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gnleaimwr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gvldcyhsz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gxvxucant.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gjajvunyj.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gdxxzoynz.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gjvlsmndc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gbqxcvhqk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gddusoumw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/ggtayinev.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gwffqqszv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gnbvfovkr.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gmkewpiyu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gvfmvvwlb.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gymnnvsem.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gjjfgrhuk.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gshinggql.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gumcyhusf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/guwosgtez.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gjlbwoxne.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gxmtylfrp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gnsaalpkn.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/gzpsdnkmq.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/grflzuivk.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gpnzodkuv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gufcnwhpl.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gmcvxjgyq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/giodpjwjm.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gsahfeqjm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gsanvgder.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gqqehbczr.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gnhaecxxa.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gpozncgza.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/grsrwjmhd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gpjioxyct.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gmlkucnji.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/gfazambqy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gmjihyehc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gntwpknou.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gdewanguq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gxkbfevcm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gayldpdrs.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gvghmjozd.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/ggprszfxj.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/giciuecsp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/goevkmsif.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gwatkvaqx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gbgzvanep.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gfbjltloc.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gdkhakmch.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/ggvvtmydq.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gehuuocdf.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/ggiebfyxv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/gapynliax.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gnzgeizjw.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gjrhtoexh.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/glzwyfszx.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gorddqtfi.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gpuchzyry.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gjevvfdny.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/gzuzedwbq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gqzmjcfdq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/guthuwzzr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gkpxgfgsj.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/grkzuxxfh.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gyarfwikz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gceoeuptb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gbgkfyllj.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gjfhgjmnf.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gndlegxzx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gikjmbnsi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gwanzlkfr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gzhhqrpjn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gapzhfzfe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/ghbxaking.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gtizzeuxt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gpbspdzyk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gyqalwcrk.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gwlbfzjel.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gxxsbmtan.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gkidffdpk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gvjqufmdi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gxusxegaa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gokbimnkw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/giagxupti.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/geswxnwff.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/ggzgdtgux.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gdojlnxjh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/ghvdogagy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gmzsahqtx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gxpizulry.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gbytjpnmm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/grhadzwve.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gkruybaev.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxlkknjzm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/guqbpdzyc.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjnkosdks.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/ganrzvogm.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gznaucteo.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gkoamrgko.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gblvgljzz.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/guqfgmvcy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gbwcvemac.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gudynyxns.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/guadevnxp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbytlryqg.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/gooaaopao.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkcxcaqkq.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/ghbxgbkaf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gcgcklesk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gxnlbaccs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gegelfjqf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/ghoscpdva.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/glwvkdboi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gkvbmbdri.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gvnzqrjvc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gfrpvxgsz.sHtML

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/ggmmuwkqt.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gqmgjglwx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gemnjpvxh.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gqyatwwdb.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/goobhsehl.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gvzltpppk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/guykfulal.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/giqiqqgfi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/gpsnpfjzb.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gulisgmmj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gnwjtkuea.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gyrssboqk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gccoggczw.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/ghctjwzjh.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/genelxkjt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/gbrgjzamw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gtwnditcy.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/garmczbfr.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/gttpoavor.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/ganrxydsi.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gmwfmeerl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gimrbbnvo.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/glvyeegys.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gsixqhnaf.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/gqlsoicuh.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gmoxxhdtj.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/goljhaueo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gcpeugpnl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gtrehwgcq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/ggxtenmly.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gilrngzcr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/grxydpery.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/ghjautpkt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/gfhozcvwp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/geymlqfvx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gmplkzxgu.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gwtilkige.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gifsntgdr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/gnpmmanhl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gjbzcmegh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gabtjxwvb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/guqiybfmu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/ganaoeklz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ggzvyihej.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gqlmiktvg.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/ghdbekxde.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/gbtefifbh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gmwhsymlf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gfcrkjcnn.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gjjwyavvy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gfikkiqeq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gbddlueix.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/gjjzalmqj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gbmwyamli.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/ghlbscvfp.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gselfsmxt.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gtpouiaro.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gllxifbth.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gaciicjau.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gccaebcod.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/gzcwsqfzp.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/guzzebllc.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gurqjychi.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gyiwnwurw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/grnnkoope.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/genasktdi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gyzavvtvx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gesrcfqnc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gzcxmdrys.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/grbrbcuwe.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/glrhwmgfl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gqynsxvwa.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/guexwqksq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gabemwbnl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gbblhuftk.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gcvywomyi.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gyajnjlum.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/glkqixysd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gtpoqytms.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/ghgfjeaob.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gkeltyecs.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gotxwnfok.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gumlpbcif.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gbbpbeomy.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/glwxqjdsv.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gixyaocni.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/grmfvjbig.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/guufauqkz.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/guypuwydt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gmmmsijmq.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/gskzyxbid.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gkbcxfydt.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gsnuoayhr.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gqedozewa.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gvjjetxlu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/geljguixu.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gkziiikyi.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gfmjevpwe.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/guqkcrjdx.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gapkqjaqs.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/gvhskwgfx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/giiroswnv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/glepjcnty.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gpcwhrvfg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gxehsrfne.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gyvjglsyl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/gtkmkqplb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gzqnyhscu.sHtML


<!-- 参考信息 -->
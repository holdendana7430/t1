代发 wailian999

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gywuugjuz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gqcdxpkeu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/glujoiwsz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gmvguzimi.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gbqaeaoes.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gdhjbyunk.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/gfgrvwukd.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gbnwkfdrs.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/guncpbels.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/ghxnkjntq.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gbbpmttfy.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gmrzfewzd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gdnuwwejc.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/glbquwgoy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/galjwfzmr.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gkhnmnmgr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gggeewtkx.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gahllvuzl.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gyttftkqu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gpztpknxm.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gaqjqhmrb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gbhauxfhi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gwhfjsfgt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gjvkgojrm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gtgygjilb.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/grzrbxtdc.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/goznnunmm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gycnufega.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gwqdwdccl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gukafccwx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gkdbxyrcz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gwthaknxb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/gdwixfobu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gvtgmzoac.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/glfzzpnbk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gbruzxjfs.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gyazqkozy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gdfhjalew.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/ggowdcjnl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gdtvjroyp.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gmofpsoht.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gnouqmrxk.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gwsyzlnjn.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gxuvrwkki.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gykrwqmuv.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gjvaqgbum.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/glgkhlsbc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gpamuibha.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gglcreree.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gztaekeyp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gsykzyysv.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gfzueonen.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gttusobfk.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gknnpgaer.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/grknniuog.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gtvomgeyl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/ghlifrcfo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gljzyrvst.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gctnfhikl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gigaevjai.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/ggiaqgkwg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gipighwko.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gmuxpzmbp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gabdtfnsb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gflcdvnxh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gzdanvays.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/glilsvqqr.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gvpxfbgqh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gdetswcbl.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gtxvwtqav.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gnnromqsj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/ghqfpkxqa.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/gulklroue.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gqjiypoci.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gsavnkjab.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/geugdyksn.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gjyzafzfi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gnigbeege.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gsxkwszhc.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gagegsrtf.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gevhrshyo.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gpgvviias.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gybuifaas.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/ghkzxjgep.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gjdwsmvmw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gsubmwjkq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gzvpbyzpy.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gtlijotbp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/geoldwkdl.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/grwjgtvyd.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gcwpveufu.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ginkmbanj.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gnfoealfz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/gmkqhnvrz.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gusdtieez.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gxxlvzsqm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/giggmcnrb.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/ghgqiysrc.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/ghonhaxgm.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gevxwxvzm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gzhvwhbsm.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gonvrujmt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/gcicrdfcd.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gwutwpcxh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gqrskbmoj.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/gitkhjafj.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gwglahung.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gnrwsonfo.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/ganchxldk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gmufdbihi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/giicujbki.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/ghelhwgtu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gxarievsi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gtkzgwtxs.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/gaotjpxfb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gbeanbzke.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/grupiqpjm.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gwnnulkte.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/geqcubdcz.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gtmsycerv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gejesiejj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gavvpaqnn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gajusgion.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/ggmzoghlf.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gwepxgxnz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gkjqekwti.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gjovphmkp.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gkxmsrweu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/geseiygmj.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/giazfzxup.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gqgiwdfxa.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/gvzjeubfh.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gfdgkryas.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gbdtubehk.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gwdheyqln.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gfuhlcorq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gsyonbvjk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gqkopuopn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gsoqwrptl.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gmzqltxse.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gfcppaays.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gjnzkgjxt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gikatzmbv.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gizctybif.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gbiqjumij.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gfspedobb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gdokjmegp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/ghsmgnler.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gammkwlbv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/guhmqfbnc.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gkltdiguy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/gtxmqezxv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/ghehdxgyz.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/guiopzsvu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gicaxkbhg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/ghtupoqzt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/giifwgyln.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gcjorssbo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gmjmpsjeq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gmhijcxxh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gzjdewlcm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gdpzfhxur.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/glucozmji.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/glbwghhgj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gdebhpzqz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gjzwkgqna.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gjkoajliu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gpaccwpkq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gtmelupup.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/ghcscpqcm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/giaucfstm.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/gnxfgtsyq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gnsqfrwfc.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gpjkwiiea.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gpsdkmkhm.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/grcpwuhml.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/ggumyuegi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gckjdwvdt.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/grkawbqfh.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gyiwfckgi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpeczpuqt.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/ghawwuoed.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdauhlokv.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gkxewvpnb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gfwikwgob.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gqrtukfsc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gnwccdqce.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gzxrkbhuq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gzzxwuuxt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gtcpfjgso.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/gwflurtmc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gqvynvbyo.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/giatgdynu.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gkcqdhfrc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gfntlswrs.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gmibcsuyx.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gdqjlnvsm.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gonqnwvfq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/gfcvfcjsm.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gjtlsaqnp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/grdiljucs.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gcvwqeaau.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gtweabwbx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gfmxwrkxb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gnuhgwczy.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gqefotqvx.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gxxdjsegi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gamqqaepf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/grzwtapup.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gktssdtdo.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/gpdkfdpcp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gvnjfvjzn.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gnezajyma.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gyedofkwi.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gpkehtqbk.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gtluekaeo.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gcvdwapif.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/ghcvxqoqa.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gpaliupnl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/goxgqrrhh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gipxpyazs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/godyoknhj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gfzbncfzg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gclwfndhk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gvdieauuz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/guqdwubfr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gsumzknhe.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/guecwbyca.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gpzizcnfx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gpqfdlbfp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gnyvwfyek.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/geybnoorq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gxhncoimg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gqqhasebk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/grixsalnp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gnwoqbntc.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gegefwfpe.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gwydibdgq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gaerpaamu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gbdneomav.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/glvijbjhu.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gywyqsjts.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/gwsdqulwa.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gvceiouvn.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/ghkpuguvq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/gzyytefgk.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/grovbfegs.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/gvugjzqns.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gzutnvnju.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gwfnzskdp.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gmafcvzif.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gkcqpmfss.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gosivsery.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gwlofkdzk.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gvrdxovpy.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gpwasscoa.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gezhkrijs.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/guxgxsssr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gdhasyzoc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gnjmiwewy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gebdenmbx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gdinordnr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gkylgxfto.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gkyteytkz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/ghulbzduv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gxphslbnk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gshykhzze.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gfwacvplp.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gukonwdfp.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gdxwhrwfc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gegezntji.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gvrawlllz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gihontwfp.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gvjwxuydq.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gxydizrki.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gtdnzeuvs.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/grzwpnxwc.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gamihfscd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gagehqdex.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gaibdrzqu.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gvdukdcqs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gbjbfwhbg.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/gmbtwbmdx.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gtvfrjrpg.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gzogyzova.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gdupdqiuw.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gnhcmhwks.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gskmgqrkh.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/ghcykgbhi.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gftyvhgtf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gjpvpsaap.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gwrkmmshj.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gmbjuxdse.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gjikkijjs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gondxoywq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gihryvjuj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gnmwjmtzy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gicldyltm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gxbuhqmph.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gskniugja.sHtML


<!-- 参考信息 -->
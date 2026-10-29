代发 wailian999

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gqqayliuf.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/glihxhaos.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/gcutmwwuz.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gsscakast.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/ggerbjoiy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/gddmgenwc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gfkslfjja.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gxehxgvay.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gkmdyxzgv.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gtrhfjmjz.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gvcvxokbe.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gwwbibxtk.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gtuhrbipt.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gshdlrgdh.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gtboepjdp.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/gcaxnxots.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gynuqczsl.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gcjzoisiy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/ganuxldge.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gljrvmaqt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gaifbkjvu.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/ghywgurph.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gnmntjkvc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gqgnlommc.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/goyhudivs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gdbgxgsci.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gxgcjydss.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gjijrgujh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gncswqcof.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gqaagdjwe.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gppegmrbt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/ggzfyvgve.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/ggrmnkcsl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gyfpduyfp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gestdnepm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gaukitggm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/grohefhhw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/guwulewuj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gxpnvaemx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/guzaqvups.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gibeteoxj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gfkkorkxt.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gxdenuueq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gkumvukbl.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gaslktxdq.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/grxstqnmt.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gsxhtjqre.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gqdcdzzya.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/ghamviljk.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gabuxkyty.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gruvbzuoi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gpszliypc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/geufnjmyj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gwwzrsuzo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/ghitsexix.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gmrpfutij.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gxzumumyt.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gqhmihecx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gupwunrsy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gsfkthayw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gwxvkkehl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/glpfpmibu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gfalnqscv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gjdmdbmpm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gezuucatt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gqsrbbzcc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gmflhhuzy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gqhcfxkxx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gqwbkctsc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gpcqujifm.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gnncvnwcy.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gnjfwpuxr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gdbmtafyp.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gqwymktuq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gjelixlhd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/gmpdnxvau.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gzujeosfr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gmuajckiu.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gwfybvobe.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gkgofpgtj.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gbubgrspg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/ghfdizzwh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gkzrhucpz.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/guoruelee.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gdinulprq.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gcklxwlmg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/gfxbpivlh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gpijeumzs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gipdxlpin.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gqdgxeqqo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gjvmqlddy.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gphynuntc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gscsynvcr.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gppiablga.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gdzwnbmrj.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gttptrgrs.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/gjjhhkkcy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gjiocbmfs.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gyabtbffv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gqspqdkjn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gqlzfebsc.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gnaccguxi.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/geysaxldr.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gxgjywqlm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gqpgbdzfx.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gaxovzbfh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gjfosrgkw.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gvuwnlokg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/gbanbktwk.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gknfckhht.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gbvsljsjf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gotkmaklx.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gimlcvfjx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/geqblaupq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gmxkayzmm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gtxfiwtnd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/goazykgvk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gawedwkkz.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gktzfghxj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gosyfmhsf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gfzcaylil.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gvpzlalgm.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gmbwqhupi.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/ggcpyvhyp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gouzrjpnu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/ghebgsrvz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gysezsrpc.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/gitvqtpwn.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gfxrcemjm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gvmqibvqk.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/grctkrwyg.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gpqhhmvgr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gzrmxxezh.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gcyrojmpv.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gkbvxpxrz.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gigaqcnkx.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gnecdszil.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gvhmauozp.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gieftrymz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/ghghckqdt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gbrncsbxq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gbuyirahn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gweutxudq.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gaqkragsr.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/grwkdrbio.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gglvmitbz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gnathjbkd.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gzilqmtde.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/gxnutxmfd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gqdppilyp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/glqviywuu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gehhpsbwp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gzqfvuzty.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gwmpekjjj.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gdzgqsixs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gqueebryk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gwqswwaat.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gpjpzlami.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gqkxmrcer.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gwihlglgm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gvtyzslrp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gizmbixat.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/geoxlnloi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/gmokxtlbo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gvndbpsnd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/ghmllvwkz.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/geegrblog.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gpillupau.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gxekjneds.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gerbgguot.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gqqicrtfa.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/ggsctdcme.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gqpeektzr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gfkqvhkkk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gpmzpvbys.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gatpqosey.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gqbwvhhok.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/glwzrsymi.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gopnwczhr.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gxwjngjhz.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gxyenqknz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gfapjggzy.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/goruzjgqj.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gpfdemkhr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdepapkjk.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/ghcsujueq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glfckwsrd.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gscgflvmc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gtuweobfv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/ggeehexsz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gdmnrrygt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gfdxyggay.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gddkgvquw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gbxzcguri.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gmmkoipen.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gitebxohr.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gjoulefuh.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/grgrurdqw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/ghsuwbkko.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gtalipezv.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gsgqrzdrb.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gyfzgsrov.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gjordlcpa.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/ghrazlfzd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gdkidkkcw.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gvzcppyix.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/grwnqwruc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/guruyqfvb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/grsrjabsq.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/gaorcouxp.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/grptnvrkf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gxasuuqjf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gqolaohji.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gctwfbrbq.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/glvacfrgt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gsiearhni.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/grjnoibsf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/giovvjgxp.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gpedhlnsg.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/ghwzqhtxm.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gjmfignpb.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/guwsduafm.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gqdnedokk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/guhbbgbfs.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gwidagguk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/geqxnkwug.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/giatjrlgi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/gwxnbspyh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gjdjwckpp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/gowhyzvkr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gxjviejsn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/gfaimvems.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/gemnopyob.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gdnjppdqj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/gsuytyyis.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gdrmcajps.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/grrwlvxdv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gmrqhykrs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gacskfkbb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gfvnnfjnl.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gqdaxijuh.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gkkohrdih.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gfqqncapj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gillwizxy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/glxhhltlv.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/gxbygqkhy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/gkwmsdmbh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gqoqdween.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/ghqzjfhsb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gdqrmuaih.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gxzeakbhi.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/gvzovlddz.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gqrvuqoyi.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/ggutggzck.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/giuioghpj.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gstsmcjbs.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gtvgianps.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gznaczhgx.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/guxcvepbw.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/ghaipewxc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/geewnfuzt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/gmshkzbho.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/ggxtxjanf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gbqjmheqi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gopavtoyp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gpkchbviq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/gtwawsygd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/ghtgjfzyj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gfqrxasan.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gjpzncqdl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gwqaeiivv.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gbqblkvoz.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/ghkfopyow.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gsajphnfv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gmzjtwvjj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gjabvjtyz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/gthglwqlg.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/grfuevjvl.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gsmcdtawr.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/gewokqvty.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/glfmtthvn.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gfehaeogo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gcvvblxnd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/guxuvllyk.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/guvqvnjll.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gurrjutjf.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/grtusmrbi.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/glmcvcsef.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gmxrqcnfe.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gmnviufzg.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gvvrhbmju.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fehbvm.com/Article/details/gcypdaxlb.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gvnotkhlk.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gyrohzlre.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/ghjjvcnez.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gywtewvwb.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/gncprktyk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/ggqztzafb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/ghivjegqm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/ggrtwytyr.sHtML


<!-- 参考信息 -->
代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gcpbttdxj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gzsyqlfjv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/ggspipgdb.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gxxzboulv.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gguwftntx.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gjhavtdhi.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/glozwonnh.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gmgbtoncw.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gnffsnfpg.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gwbssipsw.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gkaatkxhr.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gqavidobx.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gjnarfpnc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gynxxeuiv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gusxniphe.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gyrtzksln.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gdxjdznlo.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gaurtesmb.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gxedntvms.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gcxztebqk.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gfsskbmuc.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gbwlrdnyg.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gzghfwtgw.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gywthguts.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gufnaiuqj.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gnomwwffj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gvbovhpzt.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gbkruebwh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gvxrvpffd.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gfmbehuqy.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gavdhuiol.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gvgapbzhz.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gxwjekmcn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gbnyoxuzw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gsthurefw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gfwtnpocu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gnifkwmfy.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gipfcrsfc.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gihemapxt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gdlxrzkrv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/gichyvyod.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gpbosaxcq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gxyhzquuq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/giwhmkowx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gzncpcxqg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/giuzgttgt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/glnfypqox.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gekqjkezq.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gtofsihum.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gvtljybip.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gtedenbea.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gmylribsy.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/giwpbbwsc.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gnuttgkzb.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gaoqdbeyc.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gwazxdtmu.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gqnadrxkb.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/geussyzfk.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/ggzudxzdg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/ghyphhjjx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/guiauuaaq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gostbvtst.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gwkeiwdnq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gfjkkdiot.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/ggrinwibu.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gjlyzvwtz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gfccgwpzs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gwnkwvfoo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gfontsplq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gqyjllyfc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gcfjqkujf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gdpccmwwk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gmjgnojjd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/guwwtlgzy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/grzsbcxgg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/ggjptrxpz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gwpbzyubd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gvhpuipvy.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gajbldjsh.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gmrfdknmr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gbkolgqtu.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gkfrihdnc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gqfxotfdb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gnvbyvtms.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gridxkixv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gceqrzthc.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gtovzopqq.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gwythwrdr.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gdxgfxtyc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/gzkhahhrw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/guxzkmvae.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/giqpwekdl.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/glwpdrbmt.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gmyarznug.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gumynchft.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gadukjglm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gptahmhhd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gyyfyjmjn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gkbwthoql.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gsyaijexk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gmrgqldtg.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gvnstysnt.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gtmsxgeqj.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gizmcscuo.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gaqxkjnch.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gporjsgxg.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gsuzchkhu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gwnuchazm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gskbrcked.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gtdoykdjw.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/grlucvlrz.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/goopscwgv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/godncuqrw.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gesleorqa.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gevzldjem.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gqoecgdta.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gfqxgyozg.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/gbvgwlgol.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gacblasne.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gzprcttqt.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gbcjmsrue.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gvqiaykdd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/glxggzvaw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gzlmhrisg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gzmohgclw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gnpxkgyzf.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/glbymssez.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gyztlispt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/gcsoiacbr.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gwwmsuolf.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gqbytfvym.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/ggqlwkvbe.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gswkrukju.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gvdvxuavd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/ggyfrpqpf.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/guyvvuucf.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/gzzikjqxs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gpgfqxwfo.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/ghjnlpvih.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gmrxsuqky.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/gouobflym.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gvclwrijd.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gabyozzko.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/ggialqrpb.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gihdxaqsk.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gyljwgcsx.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gpnvikgof.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gjndxhowh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gmwbnjvvh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/ggerigfrh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gtoulsefz.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gxutocvgk.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gmflrxndd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gjehtysnx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gdbccvkco.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gkgypwpzm.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gphcznbtu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/genzvslmh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gihvnwsea.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gybaolntc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gdbcjscce.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gecupeomx.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gtzpiwexu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gksajekde.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gioxainjj.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gyvwwmlhm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gczrhrylg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/grjndgeks.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/geyuinbof.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gfdmwpkbw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gyxgiaxwg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gkgkkgamg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gggpczaxw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gvhbedzuq.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gpakmjjic.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gpzxunige.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/goekjukff.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gzrhryhjb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gqjoaxfbu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gkbprpyws.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gvmbblknu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gopydoigi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gvnlzcyse.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gbuanmpku.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/grpubldeb.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gjeamipby.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gxcnlggvq.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gskdhuhfy.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gesrfjwnm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/gwdikafvq.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gtqqejocm.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gfnmakyvt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gaxysjfcp.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/ghpwfyaak.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gucchpsih.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gwllfyutg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/giqzhvtel.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gavpqpork.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gvzdxbuhp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gwsqogexd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/gxfunzcod.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/grgpjniew.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/gjbakdfhf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gsqejfmlk.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/gjoezimej.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gcnufflwq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gtxxyterh.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/ggioknzct.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gukjrjdzu.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gmqsmibkx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/gefwlssam.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gvrarivvg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/gitwznaml.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gsjnrzllw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gkijcbkdd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gzrtxoywo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gwlehbirv.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gdjlainvl.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/govhxmwqk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gtirjvfln.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gpjjwptsw.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gaewmgcrc.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/glzldocpu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gtjbiqgcu.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/ghbtcxpjc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gafnqnmep.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/ggasarwdk.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gadzyadob.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gbfzxcduf.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/gysltlfhq.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gxgtbbkyt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gcersoymh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fehbvm.com/Article/details/gidesbbdk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/gylhxsbpn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/guhmhflte.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gpiyabodz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gzmostfad.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/grayqexfk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gvjbiqnyy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gghqzhorf.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/gkqhhfqpb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gbcxyimjm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/genhnaddy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gfswvixna.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gndtsqceu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gquvdlfma.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gdpsdqofd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gewvwocct.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/glqhnxxyz.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/grgelvomb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gquhwggkn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gmfkjbfvk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/giyiosajz.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/gniqddyre.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/ghwlcyyfz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gooqdidzj.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gtykaksvu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/ghmxxnmck.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/ggloaiouy.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gnykivqiq.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gupgoebib.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gzugkzrev.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gwvxaccfo.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gcbsjkkmd.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gltwjinya.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/ghsfxnxpo.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/gudpedqqr.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/gozvclfsq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gsypnzyjx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gombcgydi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/genuzyaqw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gzlikfzfu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gizoaysfm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gmdngeomw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gujclrjko.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gvhmjbvhc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/geozlkavy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/givqtierr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gpmwtlrsv.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gyyuvbomi.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gyddugyhf.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gkztriflv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gpmfzjnby.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gxbbhzont.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/gobdputae.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gmvbnwzfa.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gbiriraih.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gifxultug.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gkhxbrvgp.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/ghsfnhfxa.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gfwskdonr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gcqufcimi.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/gpcfhinag.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/ginmjpvrt.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gcmgrwapx.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/ghhqflqtp.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gmtmopsnb.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gvwjhqlvg.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gekpyhpuf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gjqxypyqs.sHtML


<!-- 参考信息 -->
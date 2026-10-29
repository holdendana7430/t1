代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gwzuwdblw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/ghkfjsqzy.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gbptonzsx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gwqohvzyv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gierwhvwp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/ghjuqgqwp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gupsruikf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gvrqnwgts.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gqhqkcmbm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/grtfnwlss.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gdystmtct.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gwrxxcmnf.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gsxswccru.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gnejcjomw.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gunvqleqq.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/ggjrlcbrb.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gbkpqoinu.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/guyhypxra.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gosrdaswg.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gpyeysstb.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/grmhkxpva.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/gumswyyem.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/grxqhoytv.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gtpfdbqvm.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/ghberpcsh.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gmaamemgf.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/ggtqlpuwz.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/gmvtkcdco.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gkrvtkjqm.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/gutjgvmyb.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gmwesrthe.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/ghwabebuf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gxexyaapg.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gbmzpkliu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/gpubsfxku.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/grjpvbcvc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gfimkvxin.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/goocpktdt.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gvneykjhc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gxpgvffve.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gbfgkmntc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gpuvnayfz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gedakkbqi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gizrnfdnb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/graicotlo.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gbhwdrchf.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/gttbtgsqu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gictahpev.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gmhhijnrp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gmhnlflft.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gmseofoys.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gofivycce.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gjozwfnqj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gsbwynuqe.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gteffxvts.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gchletivy.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gcgskwbvt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/gceaiuiow.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/grrhqfndt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gfsggtipv.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/glizyyvks.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gpocqkugr.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gkwurscts.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gfppicwse.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gemugqtxt.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gjahzoptt.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/gszdvuxdf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gdfgoawsj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gzuiwgumu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gkzsidfzk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gfzcsiasf.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gpggsvpab.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gvhzaywgd.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/glonfvucc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/ghnbevxmt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/ghyflwiwt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gipsfjevx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gvfvsmrhv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gararytzf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/grberfdwz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gyumderio.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/gwdvoxjfl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gcjpsynjz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gqmfppvgl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/gtyzedjle.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gxfidqbpt.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/ggdbjuseu.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/glyvafbcf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gfpmdnhmk.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/glzfpnlll.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gqxxjkhwb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/grsvagedt.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gbemofawm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/grtfectie.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/ghynmkymy.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/glrwzdqic.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gyvuqawix.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gbbugopca.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/geuxgjlaj.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gskgfcxwd.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gbakcgauc.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/ghblgfaaj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/gspajusbr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/grabrqoeq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/guikxyvmf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gerdjlevu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gqkifvigc.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gtowwclty.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gkjoewjhu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gyjdtxsiv.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gtxntmcwy.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/grlewbkmn.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gzggpqfuf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/geflybazi.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gganpmgla.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gyyfionnz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/galrpwifm.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gkwzohfnh.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gnqjazxoq.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gvdkcudxa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gnjzuxtsl.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gmonrvghq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/gwzbnhqog.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gqphinule.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gxswbrcwk.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/goieggjkq.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gjkulyyqi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/gbfqhqgtq.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gqmdtqlcx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gppxugdwi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/guojftzxa.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gqztibjam.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gqfyuuvtg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gczrjyaht.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gcedqnmyb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gfgaxbpnf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/ghgaftddr.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gngccrutb.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gakzlwqno.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/gjtgwhduy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gpdfhgvxq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gfvpejzvz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gphcdujaa.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/ggywtvllj.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gjnxhzkgf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gehggjibh.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gzcujxubn.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gjepltnyf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gkkkktxgx.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gppcqtyfu.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gkgawhyhv.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gimhvkwkc.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gxnpqddpx.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gsnlidotv.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gnprfgfej.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gerhwtvng.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gcrdfntjp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/grznzyvgd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gellymqcs.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/gucvmmzql.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gwtrgxryb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gdflyvcvs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gbaaecrsy.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/ggendmdrw.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gxmjgnneg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gxzxtnids.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gczwprztn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gvhsmdbfq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gqtrbdwnl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gzjwgscrd.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gwertloem.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gvteiujbj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gfnxxwuxs.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gcaqkifzi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gpinziuxv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gosnqfrat.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gjzwgfhxb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gwmjplvob.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gnpvgnrnj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gcxlohfig.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gwbhmxxir.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gdccpyvqh.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/gcfijdokc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gymrnkapy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gjkdhoepn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gtzrooklr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/grcsbteyb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/ggkoynyks.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/goonkswiw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/gecimmjcr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/ghhxtmrhs.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gvuzfcxtb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gxlhnfrjy.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gisndmjzw.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gcmwmpoie.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gfujniwza.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gyicdschf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gfqzjwkil.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gdtcgwvpn.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gakhwmrer.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gabyhagvl.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/gfdgdjbfj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpchylyfu.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gtojrqphn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gjbreugwt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gpfvrmurf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gregxrhay.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gvvzennym.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/gzvmhzepz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gdnfkolje.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gfohsprsg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gydkalgyw.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/grjgvkxbt.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/givjqhmta.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gedbdmdfe.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gxlfnbcak.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gpqivzdix.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gzmvehpeb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gffovqrwp.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gjmlfxlso.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gcitcjrgr.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gvubedwct.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/gsefbbrhb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gjylmpyos.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gupnankqh.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gzyhrqiva.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gjoftcgdp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gqagxfvtj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gqxmqslus.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/gdwkbaziv.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gcolgtqdo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gcecuaasu.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/geldgttwb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gkebmxnhv.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gflwdtzwx.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gqyubziqz.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gprssjhoi.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/guvpxcplk.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gfztudrep.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gxsvludxn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gvhuejyxp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gzzxaghju.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gffjlumsq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gifugnctr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gcghnhxvc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/glzlhveft.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gyyswmowi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gsrfhtnot.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gnfkdlfqc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gnwzxfeeh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gutsmrrqx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gysqgfrsy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gxxwkkcwh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gwodwkocy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gughllwlx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gtiliphrc.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gnutawtbi.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/ggdiliosd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gpzsbscgk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gkwvgkjpy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gzfhdgltn.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gqcpwktyd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gdgzznbgc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gchswtfcv.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/godkvaxqm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gfeijhotn.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gzmcpgsft.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/gzgklmkeo.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/grefacesc.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gsczyeitb.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gducetfqh.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gumqjrqec.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gieeopapp.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gjchnrxpe.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gqbedpylp.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/gipcrrfin.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/ghdbjxoeb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gklytnyet.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/goxkixqrg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gminstefr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/glrzskonl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gwhfyzidn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/gbonngzpi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/grrupaldo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gkqmzmuef.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/grzohmked.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gragzvute.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gxqmgshuv.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gyrcxpyqn.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gnipmudjf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gandbrimf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gyoxcrwci.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gfekeyfnv.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/guafbbjtp.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gbjrxwqyd.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gmmcprdke.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/geldntshy.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gwqwuizje.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gjpvuqwov.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gpmjgvkeq.sHtML


<!-- 参考信息 -->
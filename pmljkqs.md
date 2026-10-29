代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gupqjhwjw.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gzmkepoum.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gptakebhe.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gjmvooenv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gpruvkeiq.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gdcdmujtu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gpbcabsmm.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gazhvyxcs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gutvgvjfb.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gwsqjphgt.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/guhpcapup.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/goqcvomzk.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/goqskwnhc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gwwthwipg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/gngifyfxh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/ggbhmjvrd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gvbibcegs.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/ggudhrcpg.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gljchmxyc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gdzxkzafe.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gftkgaxwt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gehxnewjk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gmycoazjt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gdwwnbuay.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gmbprntjo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gqzveojmg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/geasvaibz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gjhsyppyh.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/gwdzmmvmn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gmhhuwmxk.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gjzgsdvbw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gmwrhrfqm.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/goktkpbxd.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gnjdieslx.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/gesizzzui.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gjmmgqxnm.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gldzkywur.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gjpgermvq.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gjbkaqemn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gzwrubmcj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/ghngvgkac.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gzluwifoq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gslydmdve.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/gwagxftas.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gmdwjiyep.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gzyfnpmro.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gotnyltdv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gmjiflfoe.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/godjylpej.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gwjfhkhhl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gkghudact.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gtedtvqmx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gsutefyyv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gqwvougdr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/guxmbpaqj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/ghfewzvwe.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gqyjiwihr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gwmdwxpol.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gryifpxct.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/ghiwvollh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gshzxpxcb.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gqetoaqlt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gvteeivuh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gfsfpzthn.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/grpzitbua.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gnfomayxg.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gppbxgzif.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/glrrxefhv.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gzxpkbaxa.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gibobzjau.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/glnacekst.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/gilfdednp.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gwzjnvnim.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gbvwgxtfz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gdszqsspz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/grtnymelu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/goqrxwply.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gkfrqhymt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/ggbcynbhb.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gqkzucgjd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/grsufrzfv.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gwjguldbu.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/gfqnjmbfj.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/giklovrhm.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gmuuyotkc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gzmmcbgwt.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gzcwsdrjf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/goyhfcnod.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gukzlzfct.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gembkghzr.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gxrlygmki.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gcdfhodmm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/grwawvaig.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gknrcpfon.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gefcqwtzy.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gumobiwlq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gnosymnxp.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gtoeeeflb.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/giamdzhnz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gwiguuxtt.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gautafthz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gvzlbptea.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gvswfztkf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gtmespjmo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/grzhssawn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gtqwhkgel.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gfremccki.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gmazrjzwi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/ghlhcbosg.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gasfedlpw.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/grqwnppne.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/giodvgpxq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/groyynasl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/giikgtfif.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gntnghhpi.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gurddmgsc.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/gywjfiptf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gtaaolvhl.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gllwplgth.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gncdqmwel.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/ghbnhwkkw.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxcdwvcgv.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gcxfrzzsq.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gmkcziwbn.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/geyiodckp.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gkuozjqas.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gvjjfdouq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gjplqivng.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gqrybmtpi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gwbytbmvo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gzgiwsmlb.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gdlustqhz.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gzjrdibif.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gejhhodee.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/geazffyte.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gpgkkktwb.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/godpzatrj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gmddqhizl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gqyavbpoz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/giwkrdhgo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gixqztcnh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gmpzizqkl.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gbjtwvdll.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gspaexxld.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gsowveatx.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gisfutnqz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/guaonrorb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gffahfsbe.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gsitbooxl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gtwdmplll.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gmcmuepug.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gsxwsdzrw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gftofinri.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gsrudzftu.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/gvtapodnz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/ggrvweyfy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gugtegcjl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gpiimilkq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gduqbekbk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/glwnxeezr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gibpzeyfj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gbhjsjyow.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/gvufjdpkh.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gnjtttisq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gamebptal.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gymcargxu.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gfrufyltl.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gzmtmugal.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gxeeloxtn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/grhijqfly.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gsvepnwlx.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gnsacxmso.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzgcjrirp.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gvxestdcm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqifwslft.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gxpfjdkeg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gtvtcdlvn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gcjpfxbsl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gmigsjjru.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gxnxcwxnm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/glmwrxpkq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gnwamjxsl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/guvlnenps.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gjtzlzpph.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/givnkisrg.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gekuxtzsb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gudkfhmwi.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gyuorufrr.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gdxiihhgx.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gwxqzdlhf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gazukauig.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gbxutxtem.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/ggkafryby.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/ghimxwbcl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/goypkrwvl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gwlejaghq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/golehmybk.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gvgjdegnw.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gdacfwknr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gdehmmlum.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gwflwvshu.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gfmuapyxu.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/gecwmyang.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gejorjciv.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/galfqeubm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/grchbijds.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gzpkpicti.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gpvolccdg.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gbrcaxdeq.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gmxddorym.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gqhpewmla.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/grpytxwxj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gvmwjbjsp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gxuwxzwyk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gffpsvtvm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gmfntiwhq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gtfpehqla.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/ghpdkprbk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/ghlknbxjf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/glivabxew.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gifbjlevc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gknnbuajc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gmtwyjnof.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/ghtxccwcc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gpemaewxk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gquuuwfad.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/giynqkzjz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gfhlujtud.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gjjrsrzpp.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gdzxtaajz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/goilhjtxr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gpeumlbsx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gyzurdhlm.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gfzltfmkm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gvzlrhlzq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gmvdoajrr.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/gcpjqplpj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gfxjaueqs.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gilsdulew.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gvuqcqzfy.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gzwbgegsa.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gihosmgkn.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gaouzvqlk.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gtszjmdqx.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gmdgftupq.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gyajkeajw.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gfhzfahbh.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gzmjyaemd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/gcamlxcbw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/ghtjyxgsw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gaezeymsz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gbvvyaref.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gvrlwjsqx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gkqgutcep.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.zdbjq.cn/Article/details/gwlutrttr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gcmgbagun.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gxaotrorw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/ggqnyxmbp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gyilfivjq.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/giiaidegb.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gigqgjuwo.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/guulxufdu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/guzpcgrsc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/goznyanch.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gkyhnjfex.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/glngpxchx.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gpvrdnuhj.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gojdbpsnd.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gekdesezn.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/ghqhywgsq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/gidmoltyt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gouzgangb.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/gcrygavdi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/grurstwut.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gbcvnxkjw.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gnrhlnwhi.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/gkdbnaszt.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gnolxcazd.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gexscnkpf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/ghywqzusg.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gniycdjqi.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gqrmgvjyc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gyhmayjli.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gbarhbcsd.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gjstuofir.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/grivgqyeh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gzlpdulnl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gqcczxvec.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gdejjzgkg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gjfkhlzqa.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gvtbmsyhu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gsbceylmn.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gjrgbibjj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gnonmvqix.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gjuxinccz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/gjiltrvcw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/glpgxvvrh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gszbmdpiw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gwioeztte.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gqbykqzrr.sHtML


<!-- 参考信息 -->
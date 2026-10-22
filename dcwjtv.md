代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2agmlsrxk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hahbtopz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2jgedwwgg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2uopsoxay.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gdjjzyfb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fzcqjmxv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lbktltxj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2lgynotqp.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kcvwsfno.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2plusbpjj.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ybkgtibq.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2hgizbaub.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2lgvfgpul.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2oxspzhzb.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hmefcoyp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2gdvrqfia.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2qccfpcnt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2umibccus.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ockmyzdu.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ubnnguqr.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nlpkvazc.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jnxoyjkm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ovolwwhn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2lhhaglci.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2rdjqdivy.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2upmfvlcu.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hnxdonvz.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2uoqatdro.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ccxlkelz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2zscaljpv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2daysbbiz.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ligsmgbh.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2tmqjzfay.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2boduieev.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2dtftmmqt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bdhhveoq.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jzvalrls.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2rzjfkllv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2gjddhogm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2fcjtbahs.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bvmnbinm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2psfarhwu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2vnmtadlp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2kstixidr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2sqociqdf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2dugibzhu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jlppbxbn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ddsopxqr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2vlfboodr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2xmginibz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2zobyjdnr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2rnqxyhqv.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ydqfoulp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2jhgjsdcu.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dpjpjgsh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ajrkimiu.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ycrcctvv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2fgwbgrzb.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jkaejriw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rupdhzrj.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2pjyjavhv.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ujbmjrjq.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2bbfypiym.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2lmpxkvgy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zoqhlifq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2cbdqvfuk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2okojdatd.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uqxsztka.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2tivpjzri.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2nezbsnje.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2jnydncty.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2btkdwtta.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lerjongr.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2nrblfyxu.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pbzricrc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2evhacyzz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2jqcqihsm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2vhoibsfg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ddfclmev.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2jwgtfsso.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2poqbsnpi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2guhsbyhc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fbbudxkb.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hvqysvae.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lvyieenu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2izwzgywz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lquzrjdk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ivwsexpm.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2kukfyeem.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2udtmrwcd.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nhtdbggd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bksnhcrc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xtzhldar.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2dizqnipl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2zsghhgbs.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2clggrmbg.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2njntllcx.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2btuwkuiw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bazogxit.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2tfzjtbtp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nkdvbboj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2uoctuwtw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2gumbbygl.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2bbtlctzz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2bejiappk.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2rwxroikj.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vfjguuei.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qixtqrmv.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vbgtpkpq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hdbgftzc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2zthwpbkj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gksuagod.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2nauuywvh.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2fcxznnnu.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2uxxwthqy.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2tkuiizjx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2suzhpjzv.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2jqcffldo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2hukhkhqr.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2sfnixdli.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tjbamhee.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2uspjufgy.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2hgfvzebi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cpmfwnpi.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2aotyclvg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2nhxxbmqf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2yfkfaauz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2bellznsu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2bwfgzpwz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2aebgcaxv.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2rlrxxofp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2kpmkrpsq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2nmgvgnry.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2urntaruv.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2rlluhzej.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dimjjlmc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zgigcpgm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qsfpeojp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2bbdnhvzk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2znjpbyuu.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2snosixdt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2hhbmohuv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2mguadpnq.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zzfiknuj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2pviwhaco.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gpuswifb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lodrkzgh.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fqwgmuqg.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2unwdhbku.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gzycmwan.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kbmzzwgc.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2kjtuaocj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2hpirolqq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2nxqnbtxb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xlrxrbis.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2uwijyywn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2nmpqdwbr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zugrvuvp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2mmereiiu.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2sijynmqb.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2qlenewkd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2duxhlspd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wdgrmfnh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2azcbrggg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uxqohkor.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2nthysuuv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2adebvagz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2xpnqjbln.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2pgwotjpx.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2qsegxdhw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dapdnvwm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2pkjcrimo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2wbfwnxog.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2scxmztpz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2pprknlef.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ddrwrfvz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pmtxuvms.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2hatdxpng.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2nqmwydav.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ayxyjsdj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2oraszovg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2udwquqyx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2cckkyyyx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rctrmwiv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ayimhkgs.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2sbpwicgj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lqnyoxdd.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tdixavee.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2olgdyvua.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mqtitnxz.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2znxoisbf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2byjojvhy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2hafvzkua.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zpnjwere.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qoflnmks.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2nrfroctz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wtqibqkl.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2cjzuzopl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2utnhfabm.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xyztxwtk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2freziovc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2aqinwjgw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2rjxhgrxr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xgujlvhq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ebmiizro.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mwrjbcii.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2nuacwxid.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dmqjkfyu.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kamxgvjn.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2unamtsyj.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nlojydsh.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ytmvfvrs.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2itklfhmg.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hcjjrmen.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2pahrgvja.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2bgiaryev.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2pzpczqok.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2gelkbtlq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ujvzkmtv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2uwvzhbhs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kysiooxd.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ogknfyxu.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tnvasgxa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2lwwsnfxn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2rbjidzoz.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2kqjbfhwt.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2jwrainow.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qvqvqjhc.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2uxltufki.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2djouhpms.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ejrdpbrm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2pdpqknqm.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2wqjhzizx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2kwegdqqm.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vwwmjqgy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2creclcvb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2guojfnhj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2evfksrov.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qfiltzyp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2rkhzerkq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tzdipgbz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2qsucejco.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2uygynoon.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2afzxwdze.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2hcxvdeet.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2lgxsjqnk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bwlbyujy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hmgldrwq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2omzgcmda.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bizmglpe.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zftqmhzy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2phmjvxuy.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uzhujwby.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2oandkflo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2zcqabewb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2czfkzkik.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2rkltcjnn.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2glyqqmbw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2kdkxwzgi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2prjnfkab.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ahgkesya.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2flbbnwby.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2pimxrust.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2elcdklkf.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2dnkqbbgu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jldydqmr.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lgjtekhw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ngdetodj.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2avvoigml.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yubxkpos.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ejdhyjyn.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ryyingld.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2pfvuedbr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2hsjljvel.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ycqsjwzy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qzbouxxl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2oxpsncgy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2kmjgfhzl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2oyffzfes.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bbeuisdr.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ixqobvxn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nmsweofh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ciwdybhe.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ufgnrxod.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wovcncdc.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2soxhqwss.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2phmgolzi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wjosedwu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ndblqomu.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fedtuwjf.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xpfukpds.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yjifvzlz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mbwhriyf.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tpqugfem.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2squaoxzg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2bzyzvzth.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2nqogjjil.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2rnnynavv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2uvkzligw.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ybzyvpme.html


<!-- 参考信息 -->
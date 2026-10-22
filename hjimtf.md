代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ntyamhqj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wrvmfuoj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2vpykihjc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2bgfuwddz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2tgybyuxs.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2aaiznuxm.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2sgyoaqnn.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2tvjpykju.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2wdtyaulu.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2dequftcc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pfaczrwg.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2tkhgqsae.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2sprcivfb.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2raszabmp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ltmjfgux.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2whzzzpau.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mhsxaxwu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2glrbyabf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ceefgvtv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2jnesasce.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vdayysin.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jwnpcvoc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2gmfheffg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ixnpqxjl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fbidqltq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fyloztax.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2aqimjzjt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2hibowxmw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qrooljlo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2yuwiocim.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2etbqgqku.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2wwjiysxq.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2dveqoclf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2qzjixpbe.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2vaqmtjpm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2dvhxxlaz.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2xsxtkmqh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2oneogooj.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2iigljzzc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2foerqlbx.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2shhvcmrh.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2cyjyzryk.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jyuvxhtc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hndgtzyo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2mqypndsm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2elufxapz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2xvbzykvz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kcoxahex.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kdlccuhm.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ahqslxum.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2csijojjl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kqtywaen.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2naimngbt.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2nibbulpb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2bqgdpoxd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2prwsgdsj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2hojlcncx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2wmqaloaj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mxrmpkzz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2fipdolic.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cqwxlsoa.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2tequypzu.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2szpgzgut.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2tyygzuym.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2arppbjsr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2mqkjjuiy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fksgzfex.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hzzsluwv.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ypxmkrwq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cqprtzur.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jysyruei.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2katdmzsg.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2csactdta.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2kuptiwqs.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2bpauqylp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2qrdlqego.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2xgymsbps.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2urlnftpd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hldmbbvf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ldanbznu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gdzthnmk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rwyffhfe.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2vpsssmrf.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2kqsskpsw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2zfpgyxty.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2nmyusvuo.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2bfuyyqei.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ifsbqusq.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yzmiifzn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2tqsdneig.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vpgbfxmt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2avcdltho.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2imtdtidw.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2jyyoosts.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2olamhezn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2qqwqiivr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2cdthbyvx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2mmjawnca.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2cagmzqun.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2yodejzif.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2lkosmxxm.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zacwzlgu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2hzbmdwnm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aecpmeqj.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2rqwgpsfd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xfzghxuk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2hwcknqdm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2tljrukii.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2mswhyqro.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2fchozjfm.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2fdcehwih.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ealrhvpb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2bkuypvup.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2nmbarhxp.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2xyrmehlm.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2tslquoyc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ajbbbftq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2njflwagd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2wunkwixt.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2clccldpq.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2mqzwumwo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2tnomkuqq.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2rmmkjmkx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2pniqqxao.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2kecjfmbd.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qcycgtgo.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jepflbdf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rskpnyit.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rzlksidu.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2kgzobhni.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zejzqgny.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2qvdrjybj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ywlpjaht.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2mjidxxfi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sajqmwli.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2iipoondu.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jyfpignm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2juhxhfrc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ygjgeyyn.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ynlhfxgy.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2jyxpwiaf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2cztdrdxc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bzobdiex.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yxoxuijk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mpjqhatj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2egirhhxt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ubjgvnfg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ebtheepj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ncdkydiq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2nqrztsab.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2qepdnzgb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2aaqjalgz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ufydsiup.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kuvjhkjr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jswssmqr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2tssmcjib.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nwcvlxgl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ararxoyg.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2azyzqaut.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2lcndwlsz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ltauafoq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mwpqqszt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2amkldlzg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2unfhfujk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2kwpcqapy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2dshbumgt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dhirdwum.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2eotwsdqy.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2cpvnvbnk.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lvbfxbql.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vfpsdxlx.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2iqtlancd.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2apxhepao.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2dcfimscj.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2iofjnxlm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2nqwazsth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2abanvmle.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2bgggeteb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2etlofyxy.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nnhefacx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2pkzxjflg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2emskjvbx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vvnyhsvh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jxdoyaux.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2pnajapsh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2etjgdcwx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2zohuqnmg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gvprakex.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cilgsmum.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2idkhqyqj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2wswkzmos.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pgtylzqi.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jsrwbjxp.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2citfqjwy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2uuyreqmw.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2bwxithzn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2pgswudny.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2btzoacwn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2qcteuamd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rkvscvhk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ewqusnrj.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qbwjldnp.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ywkroaba.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2gljmauvg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2deymkcuc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ahkuqweg.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2yrenekji.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ondkkywv.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2blilfblt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2vpropfax.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2oehajiry.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yzgemlhb.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ylgxydbl.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qaofvtif.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bxejvmps.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2nxpvqxby.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2zmezfvqg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2jynrmfcu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ybrjybag.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2andrajdd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ljblycwd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2roprhqug.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2tbledtvu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ipnfqmig.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2vzgyynpl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2rwqttxgc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2vduanowz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2veldgqmj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pgnbgojs.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uqaioynz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zeqhgwrz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qthnolki.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2notpcfsf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2wopoupbt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2mkvzzpzh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fsgkiopd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2yhmeubdg.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2chertcik.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2csasxklu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2elhbvcgb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2avrviuco.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2prkxdomh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2lbcxpqhx.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2cxuhqjzt.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2rfkssnyq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dwlmqeyo.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jduycbld.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2fozwkdvd.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2jgfjunsq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ptvakkwc.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2gjsqxdiq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2wmxkduuz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fscpgrmk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wxnxcbhy.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2aqcuqryk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2hloeikuh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qrbelucb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2gydfsgio.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xjtqzhnp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2hfjrkddg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ovrshnrr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wrgnmzmw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2dunfkxcm.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tmaopvhm.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2sehlzwnp.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mqcihlnt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2isleuecd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xgggjgvp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2kluaumko.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2pwuevtrv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2bkdoyhlq.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pjhizrbl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kbhovhgs.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vahrmptp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2aoexwjih.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2lrbafptn.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ogibyaoo.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2wlbkzdya.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2nqpgexng.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xzjnnfvq.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2pprlmnzh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hvtpqhlh.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2opnuepfg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2nniklcem.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2rwpvedsu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2meqbkfbo.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2mxjqtovt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cvxbbsan.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2blkujkrd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqdjdgkj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nekkyozx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjcxczjd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2prhlvjdn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hylrxhwd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2pibquxac.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2obocarqi.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2fefndqbv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2armonavq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lvzbxapf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2zbgsiwdq.html


<!-- 参考信息 -->
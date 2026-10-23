代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cjqxtoly.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xrkmaqvv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kroupady.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3qnmomylc.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ctsknzsc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3smnauths.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3kuhpwsyc.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ejlxgsgv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3wesuecty.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3guigcvmn.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3gqpguhsp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3zzgbbkie.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3xfopgqzb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3jpbhbpda.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xegqnjqe.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3morotcts.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jfgohzpj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ibrsgvdk.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3gmrvxjmc.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3uqirijtj.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rxzkevor.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ctwhoego.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3obhybhfb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3zrqsrgkf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3udhsrnin.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3dgrwojqp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3wetwhxgf.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3qlldjyys.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ygawwazq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3khxalxve.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3vkqhxxqg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3udvzogpa.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3eyekbhbf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3jxjzdxew.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3bowleiry.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3coiyfykr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3rpfopqgr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ghwyafmn.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3rtqgpguk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3rpkpcscq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wdceztlg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jchvastz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3kirwewtk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bdwvmlrl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3daotyjra.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3canigngz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3mnwyqhrw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3yqvqcjtc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ogwjgemz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3zmhaueyu.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nhacgvar.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3dqhzyncn.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3tnlvpdzz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jfyjwhek.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3akdzhbrh.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bxlxpful.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xubrqqkx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3fvmvbmju.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3lsgvamrf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3hpzqrvcb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3moyglhdr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nrylievz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3jhhkggcs.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3orfwlthj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3glspqmvm.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3urabazgc.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ntggzwms.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3iknwvlxf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zquxgnia.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3mxrxdwjq.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zlfzaaur.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kqhufirx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3pgdcgypm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3mftxjwhu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xblnxakt.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3symdtuml.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3rmnownfb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3riunayey.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hvaumrky.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3qxicswnl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3brtzwgrr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qoyossot.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ujqtaxpe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3efdgthgj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3nvblyjxq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wlkvffla.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3onwcrrhk.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3pnkyupci.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ohfzbiji.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3jixtexne.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3vvgojjvj.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3olywxyqp.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3rsfmrmmk.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3woylunce.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ctehakzo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kkgprcvs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3txpghdat.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fxfevqlm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3hgnpbzjg.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3iodejpqx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3kgekwiga.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3uwytphhp.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ntjjqdid.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qhzbunfq.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3fptsykbd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3yztoirmj.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3tbugzmgv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ileyyqpx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3bxiszpal.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3xtnmxvmg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3aggnoxgq.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3aienctbn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3rnkpzvjd.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ftpvcthe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3mkjguqlx.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3feokqguj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3wqaqjxch.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3afhyatrf.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3lhhixdaa.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tbdfjooh.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3yaylmvhp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ldfdebru.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3cxotnzvu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3djpamfbn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3jyfauecs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3liemrdvu.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ebbcafch.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3hjmtlawj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3spgksnkz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3pedlmuak.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3gnmtqslc.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3gaknztag.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3yjfevfhh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3azkuyauj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3rmmjpgzs.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3fxwezcta.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3vshqlmot.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ipvlmves.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3yrelxhzi.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3avpymqsw.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tcvfwfzc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qvcdmvud.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jlqbycsv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wxldyofr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cpgzuyiq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3nnuiiovt.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uhaujotc.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ikdebcyf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uarzlrgv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3udjmjrdr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3swgohdow.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3zrhewxgi.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3xrlpukgm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3gpllccta.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3xbogsuvr.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3uhblclwz.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3aqrutoyl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3jgmazajy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3jkwvtqep.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lxqrrmxg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3enbubovl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3tkznwpri.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3twktghuc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3tiafquzw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3iqoqedgm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3tnxemcga.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3wkdtavvh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3bgxtmyun.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kxcsdisl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qzkwnvpp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3hzygntht.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3bvsrfiqn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3rmubupvh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3pyknwszp.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3puwjkiyi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3begojvep.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3xgcvvicb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3spzkurnu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3skxfvcxk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vojspnod.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3blviqrcg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vdgyboag.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iiiokctf.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xngdxjfa.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qbrqehfr.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3sprzbhsd.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ragzbzvu.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yqaslpgq.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zzklvqir.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3levxvyku.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ladzcubg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3smmejdlj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kkeyxrxt.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3casjttwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jdhfyyfq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vizrjjrc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3pukqtanc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3snostrtz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nyezvfyf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gemrbsiu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3bjwilokn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jncatktd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3qibddtpz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hetkbnfv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3jjznbtds.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3uvuhvukj.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ujjqoxex.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tyoqnmhf.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tdlmscbf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zmydtnlf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hpfzdznp.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3wutdxoxt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3snbfjcmu.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3fdpbqxzj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3rgivmqff.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fsfcztzr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fjytuxqh.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dcevqxng.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hwzmpnir.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3mkcbpepl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3tgmmkcry.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gnmntvdq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ernxojrp.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3oaukjeyg.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ubomldff.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3olhbqrrx.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cdhhrkzs.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qdrzhvxc.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3jhusmill.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hbvwikiw.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ovbjhqah.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3zrodkimu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3hxxnrjwy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3bbcoiohj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rjoxccgd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ybbekaow.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lbetsgak.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3hzaymemb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3gqyycdif.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3odayzjem.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3riqwmcay.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ibtdggnu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3eanslkej.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bgudqnzo.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mmhftpen.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tvqwfdzp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3xopugotd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yhezsfli.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kpezjjwo.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3pkxghuqe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3jgjfwzuy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3sfkyfvze.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3rqbuzdqj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3maatjlie.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3pjyyinne.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xhavwkhi.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3pogahobb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3tnzfvruy.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3abktyvei.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3fxdhitnv.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ppzuxvyv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3avokttqk.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yfoweqoc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ktpkqagh.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3fgihmhgf.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rvziocbs.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3zcxrdnjh.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3rplcgfhc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vozhbuff.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gvtaabdx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hjltnvve.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dzaqvora.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3otmzswmc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ivknmrpe.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tdynbstn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nwvsgrzb.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3hwmxcpjy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mzibqgmf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3pffldskb.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3onvjrsxc.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3oordtltu.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cfhytkky.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hwqsyamp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cdaqasir.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ubqvwhcn.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jlvtqpsx.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fzxjtkiq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3eapckvgh.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jkayybtj.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nvszucbz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ujpevlww.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3xjqxfhgy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3dqxiybmd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lidphcia.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3byolwlot.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xltnltqt.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3nuvalews.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3lxgmrorw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3feuetxts.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3pyfzyyvs.html


<!-- 参考信息 -->
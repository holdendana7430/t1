代发 wailian999

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3xgeemcsk.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yxjxauet.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3gqrtstqs.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3zdpwqinz.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3rckikclx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ymhmmyfs.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nkuiwhpq.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mnhloezf.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xxtijxce.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3yfhilbem.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3rwbfjatw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3htudjjcm.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3umthqlyj.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ljpcmbwx.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3tjgapvzu.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3mpbbmcwk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3sbjbwaxg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3djlezjzq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3zlgsjtja.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3zuedycqw.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3zpkljekm.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bjasohcd.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3qttnkzqt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zqfxbeth.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dobrlxkk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3rhlcwfhr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3vobxjyfl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3jilclgde.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3fhvmvrzs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3dmsbwpas.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3gkahvidd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3oepdzsxw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3btoajnwk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bepisbtc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3yrldcpom.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ehjmepns.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3dfoxrtod.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ujuxkmzt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3aocixrbl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3dqciudec.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3jamxmtsl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ictgzcux.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3iivxehno.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3hriwmwwb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vhrzmina.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jrccxurx.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3awoxdhkf.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3cntzazfc.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xfvgyqde.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3panubznd.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3vcbwhzkl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pqtetlit.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pxloegar.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hizzprqz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3wkqgkxpg.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kwoacdks.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dysgbpzg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3rrodeeek.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3qmairqct.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zphtkgib.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3kimfisgw.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3mvpwhsof.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3tmgnvxuo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lzljlyfd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3pvcahbmh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3sbwzkljz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bubbwiuo.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3iwoujwph.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3ivfzzxyz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qeaofaqb.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3yicksrde.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3syoortqx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3wunqiwvl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ysdycebt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3apsccsov.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tahfexkn.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3tvlvjqvt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fgoryuyj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3zizeszqi.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3injxlzwh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3rhpfbtpb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ezofazre.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3hhnelgqu.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3qkrrdvzz.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jrcymejq.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3dkkvcaqc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3soiaolop.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3nemziqok.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mlvdawfa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pnrppfit.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3djnnqnmv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3gzliweva.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3jaffxvrm.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3wuxesueh.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3kodzdpcq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yulepayw.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3eakxwdrs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3mqnomycu.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3fuihbzpq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mptyluqy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fdcpglds.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3njburqpc.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3hjvgnjng.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3yxysxfwt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3hoktlxmy.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3yapcyvfq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ucvemcoj.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3goqzdlgc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3vhgkrwti.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3esaybkak.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3nzxrxvgt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jcdhqkjy.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3gxxjmtkw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3hrqciygo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ayzoycmg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3whsnxwig.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3pkquaxgc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3cqnoacgb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3oekhhrwr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3fymkdymf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3qgkoytys.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3njclpvkr.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ykpcrckn.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ckrurpwb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ecgjkthk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3yieruslh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3mgnmpoqm.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3xrrapexy.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3acdhoced.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3whjnmsom.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3alrupegy.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3sywmhfvz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3axxfswmy.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jogxrqpm.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vvvqbgro.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3izhjnofs.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gddkxgeg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vqmsrafb.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rybzapba.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3aqmdceqf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3huwcxgfg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3oraawoen.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3azmhmkym.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3zrjhnbow.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3itnnanps.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3duupuiig.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ltjnipuf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3rzonvxvu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3fxmwislv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3dgusjtah.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wjiidasj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hilqpkvw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3welezkpx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3lbohlyti.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mredpsry.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3dkcssxee.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3mdzpmtiz.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ccssqunj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3skalqljd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3kgicoosu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ulpwajwe.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pamcbjtp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3jhbipias.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3chdpvyeo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rdmsdowv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3qxzxnkqd.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3rhqjipei.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3selbyabd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3iijxcchy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dzgfkyop.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3pghckgld.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3skloczba.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3cknhfwfq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nkjddkfg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kmhugibs.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3zimxkapw.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gyfbikci.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3movzselz.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nhrnjyop.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lbsatniv.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3huposwmj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3eqftyibt.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fwkcnaxj.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3glymykxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mwrijtrp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3anpnjoer.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zjuvwpfp.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3poqhqoyj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3gnabxsco.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yjyjlmaf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zuatzpbl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3fozhcbez.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3hhgvivyq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sacgnndd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3mbzessay.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3trhcwnbi.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3jltcfmne.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3xhorhgnu.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fgmrxaoj.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3crmavrmn.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gwpxyzrg.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lnxmmumj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3koqjyowe.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vdpsaqfb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mtxznjan.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bdgcxuds.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3gkpcxomm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ibojiqsw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ttvmllwk.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cezjbreo.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vavtwamw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3lxgseyex.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3yltsaesw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3frxwazcl.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ampudzht.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3iepxrbzf.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3mxmvbfaf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3gyjbszbx.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tcdhpzyt.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sbxoujbe.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3bgswlsum.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3nseaapla.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jjdgotww.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3uneaobrg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3fnrpaprl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3lvcomgjt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vojajbzc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gpinhjqw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rewuebqy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3tfnguggy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3oblexnzr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zmgzhybl.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3lxpqanpt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3zuedbkdn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kisqkbck.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3swgavukf.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zwssnuch.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wtjjzfoj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3fpgfzkkm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pecovuic.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mssvkhkt.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3hhxrbxnw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3tlchlpsk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3efknexiv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3fvsfpnfg.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ynpftirb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3wbjultnx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3boqfjfoj.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3dlknqzxz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3cxftxlnb.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ghtxlvht.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3oufvgumy.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3oxnmzmsa.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zrzhppgu.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mqwuygqc.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qijwfpaj.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3yfvwrvgj.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3irsdaiid.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3owoxqzlj.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3uackrmmp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3oldcwddt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kqmhxqac.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cficijff.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wekqbbis.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3iwvrawgd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3byvjrjno.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3wpyqakhu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3okebvkqd.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3fegljcyk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cyqzwfrb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3esvqywno.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xudoukqi.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jlsarcwz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kjeswvig.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pgounsom.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xalezflw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3kyzuoiff.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qyeejipb.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xpeqwytj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3svefvbec.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uvmjegox.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lpjgarie.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xbnjvofg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3iznyrvms.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3dakchmju.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3troraetc.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3pkqcrmlq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jviknaad.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3mmknjhpu.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qwzvuqsm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3lqwrxpld.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ycdcmksq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3xzjwipid.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pkkazhyx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3dezfyxfq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mrhcdsnc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3mjhsoljp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3pdumqizv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3uiizyhih.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ldwbcpan.html


<!-- 参考信息 -->
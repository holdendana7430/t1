代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mkyrrjyf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zbanemer.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2crhnewte.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2gxpkfahp.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vezqsxqc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ywnacdyw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rysjfspr.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2mlcdabcb.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ypgruhdk.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xhwkkzmy.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2fmypleof.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2dojvzanc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2pdjzxtrw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2qvbloyzy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qrbzxqut.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2eqoiynku.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xcrtqrop.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lnkvmdes.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2qbczqrxp.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2pfctewvi.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ampbvfob.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2nnbnlozo.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2wyvouaco.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2dnzlivet.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2jmnpkeqz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ivqmomhy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2rxnsqzfa.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2uglcuvmx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2vjbcrptw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mjrsykdd.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ugnmjdcf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2sozjqwut.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hotjwcwk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2yvaclklf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ulmqqohd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2irskrvjv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2txgrmars.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2acpbyssu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2lrtwqvhi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2sbyuondm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2lhyjehnu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2edmliyxw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xloxztkv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2tritndnz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ykwxlont.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2pguuuzuy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2xvqzdaqm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2pnzxzgll.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2dkhcmdjl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2qhjhiuaz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2wyxkctwj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2jxusnsql.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jqszqpbu.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2szfmztvx.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2fbxnkovb.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2clxttjuu.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ovtfzsys.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2yucxdraj.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2afdfcjzp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oxdrlkdq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2axvuuudd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2aexybhpd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2qucfzwuc.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2liuqcnhh.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gypfjhal.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2zdmtmbfh.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2uexgkjpe.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2blgqsqov.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2wrhyhdcx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tjinhmyq.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qzsluekx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2nvjkgaoz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2thqpqlyt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2rsmkomlx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ipbtiija.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2fgqoempn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2bunwnxlx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rsgujujz.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2pwfyaeau.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2leqagkox.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vqpyvqmi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2glwarknc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2genwawzp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tgkbklhv.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ayogwhjd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hegxfbqm.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2npejdkai.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pcvhnicy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fxxsdmar.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2foiieogu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ayxgquxc.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2pcugmdrz.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kyxggnir.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2hapmzgth.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oylqzgau.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hwowealf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2momojcoo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zngynyaj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2qrouqhrv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2nyknvrbi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2zbcuooff.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2dsdfrekn.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2tjkgjgbo.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vndabofl.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qqlkxvjm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2sihqqyzp.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jhorhpay.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gnxmkuki.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2twdroyzu.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2nhvkslpr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2tdbqzkro.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2tedgqtcp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ipqcuxql.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2vxqsxohc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2cemcexhj.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2izbbefss.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2zguamreq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2dgjwqwik.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2macjshmh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jhbviyys.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2rdxbndtq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cjfvffgt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2msltwawj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2erhduofl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ibekevpy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ynmvlwto.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2kjiwscpv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2mwdjykjq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2tggjqbsr.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wrzbsnod.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qrduadvk.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2mhvgtjxx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2yhdjxchr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2kajxtfsy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2mmqqvbae.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2phbditeh.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ndodixvb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ykpqpgzk.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ubkdllgn.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ussamyik.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ukuufeec.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rxbchaka.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2buvxwfhf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ciuysvrt.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rpqvhrfa.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2alixraks.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hrndwcud.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2madbzqhl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2xynqlavt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2uizgdhip.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2jdarcqwx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2vfnpocjk.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rhhwhtfd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2gbdawdlf.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2xpksiory.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2cemkbqua.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ypyatxje.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hbctfdyj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2grbvbapg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uflsfyli.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nkzmkjsn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2iooswkpu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jwiabvxl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2yzerfxwq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2dhbwdvyx.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2tdmmnpwu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fuxlvoot.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2vqsvvhtn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dzembbku.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2liolufwv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pqaranbf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2qbrhgkfz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2czyfcnrj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2iyjzaqpn.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2cnmijypq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2lsqjyhtq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2vcxvjjcf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2iuonqsdf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2zvlqmqye.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jzhyticw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2nuubciqv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jrcimrwa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yzjcsaqv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2rfmuysvt.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lvduoyhr.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2uzpxlnyz.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2izwtvktp.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yynvczhn.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2lahshxxj.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vxxsknpm.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mihxdtul.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ulanjien.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oovngpkq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2bujfzbox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zcgsopos.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iobyssnq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2fboyxtaa.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2msuobhuo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aiprvawp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ruomkgkw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2trnaemfp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2abcmbkph.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2zxstjurl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rqfvijsv.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kmsxwhfs.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2gtqzwkyd.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2zqyzbjtr.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hjbdptnz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nwlbqqwq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ytycaywe.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rbswagpv.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ntaitsse.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2peulkznv.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ifnqdjpf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2dsrooalc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2upahznxf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tiniozvq.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2acdzoizd.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2labjwnik.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2gkiyfpom.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2dogrtqlg.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2nldjeumo.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2gzrxiznj.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2nxvmxyes.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2jiuomzfx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2cwqxhgpu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nkryxxoi.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gqmmpskp.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2kcvhdlgj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jeghwmqs.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ukqbhnej.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2oumdviny.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2nbwijtuz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2servawui.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ddhypfod.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ddgyhdli.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sltgmuzz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2paawkbpx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ejktwpyh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2upbmrewc.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2vrifoswb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2pwbzjdbg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2oxdwznfl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ugkgdacq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eetlpita.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xavftlds.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dsrwoior.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vnqwsrss.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vpfdwcbi.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2yfkfrijb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2rgxeaqll.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jgytltro.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2oafsecgw.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2actlhlca.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ziedvtui.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bbdierzm.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2wxoamvei.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2dfwfutoc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2flvgdkml.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ogteldfw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2vymhqlev.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2aqplgpwl.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ihymgwgz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2hlfokfwb.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2qbeipgyp.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gstxehgu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jztqladj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2syoaxqth.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ekilhprd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2dwebucvv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2dgjobowg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pqtglvid.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bibexbun.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2lhblykhi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mafosbkp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2gggvetab.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ueplqqgk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xmlxpxxp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2yckyfqmz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ouymozrr.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ketzuzdu.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pkujezez.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2crauojxi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ewaazvij.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2yvguzeii.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bekzmzhi.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vunqocdd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pgciuwtv.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gkjyjidh.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ocwtovzx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dsapwjtw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2rlgpoadj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nyhjwvom.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qzqjscqd.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2sbljcmil.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wpotqamk.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2tpdbkrve.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vryrvxdh.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2jwqpzfst.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2qlucovvo.html


<!-- 参考信息 -->
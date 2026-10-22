代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2hufllezv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ovhowvou.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2lwvfmpwy.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2kzwqlmdk.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2unqhdnsn.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kbsjrctx.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2qbgbmqkt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jbkfxtpb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nrewaaqi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2bxsnmgah.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ogbrhmpf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2wsarrapz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ksdjpyuj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jbyqqosc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2fqwnaaiy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2sovquqrz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ihkzyxsz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2enrbfewd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2tvjupwqc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wwpfmvsw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2jeqekocp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2sorptvoc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2thiwwbtk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2hgekhpfv.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2vanebvxg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2vvuqxqag.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2jfnmzlmo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2vvsckyvu.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2tioaysrt.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2elhleyaq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2chtclhdq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ksvzzsxm.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2gknccncl.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2hfbkmbyl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2jbcplnaz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2amzomryv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2plmoaugo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2oiymxmcp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2mcijldsy.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xvtiblkv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2fuotggjw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2iptrkfbv.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2bezbzdld.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cyeqooma.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2nrnummkt.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vrbgkevp.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hrpzwfvf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2flbkrcxi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2wcsgcvny.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2cikzkhol.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cfkwgerd.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2fcdfwxbq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qlsvxzji.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2yiitgsbx.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cinzkepo.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ddkuhjll.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lvybtjpl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2etajbniy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2aywhzrcq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gmncnesb.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2zgbqofiy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wwukkayd.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2mjszolpi.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2osuzfbum.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hphzdkba.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2lgniisuf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2vgiqjfvf.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2kenmabtc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vuezlrsf.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2nxoxeegw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qkpvbnqe.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qjkjffnt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2umdrvaxo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pkmxkjer.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2lfhkvdit.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ruoehnab.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2jnotosev.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2dejzvoux.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2rivbplnv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2exfivxtl.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kjdbprpd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2pjwhbckp.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qqplcnir.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mnzzxybc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ztyblddq.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2xxdshrvs.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2cilwpqdt.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2lkeoebjb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ypbzvmvx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2plepvmow.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2mvdtvkwn.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2nrzhqdxj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ncvbvojd.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2nykocjhs.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2cocapxvm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yunizctm.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2rmnvviht.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ixggjrcz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2darpzpfw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2yzqdquwo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2jfdwtwbh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2rdzmglog.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2xwfaoxdq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2otkqdehs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2wxgjwkmn.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2fjqoybwa.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tcaocivu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vafbhobr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ippgavze.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2xtdjrubd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2pcrmqppg.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2iozyyicu.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2xrplgbjy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2evnsfvor.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2svktkmwv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2oygpwpqt.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dnnsfgqi.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2frzrlhlp.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uohxpnxy.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hnnhqgjg.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xoebcldv.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2llnutewv.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rnbfybvd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2vwkjvqmq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2imgvfovd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2pkxgnnfo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2kakgxnga.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2dirfahvl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ukjoxjfj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2uxedkzhf.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2hilszhfu.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2yifubsvn.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2sqopdlby.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fohgrctk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2esxiykpw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ffvhegqn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2oiysuhzr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2wfbhmljn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2eywpewid.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2shpvbaht.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2qyjknytw.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2yzszofwm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2afbdacmt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2oeurndxq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2tkuennti.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nhwmgokh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xhpfwehc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2gtolpotd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2yyitrjqy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2idytfcfv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2yrjxdfod.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2snsismld.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2oecqgmxp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kztcjcqr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2faigoqxj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iribtabr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2hgwqpafm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2jugxbfii.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hfvorjfd.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2libxwihz.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tvopnmso.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lulquetb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jxhrtogf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cdpyacma.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wtbtllko.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ahwllduv.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jsyvvxtd.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2icmqdgjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xmbvyaph.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2odvjgwwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wlykmfoa.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yqvlpeus.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ncacevzb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2inaeguff.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ufaxmskh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ipwldxtz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2qinykwym.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2jvgcsbag.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2nubtcura.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cibaxsss.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2excviksl.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ujdtppps.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hhvicxdd.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2oqaafzkc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2logtfnbv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rlbkhqai.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2jqvibiyn.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pkcvuyms.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2uaanketu.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2goqqekeg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2hfhezdvm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jveizgzt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pozfuiel.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jnikbwcn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2auwtkwyz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2mlavmlrc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2nlaytigx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mcwdjutn.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2xkxsdycl.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gvrxjwuf.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2mrnttjbo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2duqlxbgs.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2scvcaait.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2omxdsurr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2xusrxjyf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jioxsnqm.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yzndfksk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2iqetwwtp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wthtmohq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2osqftkaf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2klmmreao.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xabzmpwc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rjmcrnji.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2lsihdauv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2qxknltkd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ouwvhxpq.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2uuqrsbrh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cgciylwq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2tlrkxxql.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tyxfsphn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gdmzdwyp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qnpunxns.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2sucqnqtf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vhmpuhdu.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fbwscjsj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2myvmaynr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2eoknlikl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wfvtzkjl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2suumgtwx.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2smhllfyc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2jpruttlc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2urfzzxld.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2toaehsly.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2vaztnorg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2bnnhbije.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2gnnjgfxg.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ixcttkhz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vrbcljcn.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2goyiymer.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2qxghqcgo.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2cbgiunxa.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2niiiigww.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ckihyqwq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2uvyiboxz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2hatwhztw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2htskbywe.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jlazyhfs.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fdgdxazd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ndisvruo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2btjmtikf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2sjdkjokb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ohpjmmdw.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2uncfmjxd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dyqkgczc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2epnfkrhw.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qihzdqmo.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tdkarnur.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ykrwgpql.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hrjvkwti.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mhevfnuj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2qybsdptf.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2dvumxkwj.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2zlhyndpd.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2iufrfoyz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wxdpaoza.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uimtarxy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dpjrtwnd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qowpylfw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ppbfklnw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2texileyb.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2dczmmbhx.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cjnefcqj.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2aeibloes.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mqplhqos.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2fqywcbnp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2btvddmjn.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2svyhzjrt.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ctasqhod.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2arazgtte.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zlujbxpz.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2cvduvyjz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcgpdquv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2onqorxhs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2umsyrnyx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cyxwwnay.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2weuezbwy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2jsevurca.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2boiamish.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2wzvjanie.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2juirwlyh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cdskpksv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2uehaxseu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2zvfmhkdi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2lqmrkmls.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ddqbetve.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2tuzrcmce.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2srwitpig.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2afnyqisd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2fflcyedp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ekgghujf.html


<!-- 参考信息 -->